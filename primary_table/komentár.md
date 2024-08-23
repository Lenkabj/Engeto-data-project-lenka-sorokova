Primárna tabuľka - **t_lenka_sorokova_project_SQL_primary_final tls1**

Aby bolo možné zodpovedať na výskumné otázky, vytvorila som si primárnu tabuľku **t_lenka_sorokova_project_SQL_primary_final**, ktorá vznikla spojením tabuliek **czechia_payroll, czechia_payroll_industry_branch, czechia_price a czechia_price_category**.

V prvej fáze som sa oboznámila s vyššie uvedenými tabuľkami. To zahŕňalo základnú analýzu dát, pochopenie vzťahov medzi tabuľkami, zistenie nulových hodnôt, duplicít. 
Z týchto tabuliek som si vyselektovala len tie dáta, ktoré mi umožnia odpovedať na zadané otázky.
Tvorbu primárnej tabuľky som si rozložila na menšie celky (postupovala som podľa výskumných otázok), ktoré som nakoniec spojila dohromady.

V prvej otázke sa rieši rast miezd v odvetviach v priebehu rokov. 
Vychádzala som z tabuliek **czechia_payroll** a **czechia_payroll_industry_branch**.

Výsledok prvej časti primárnej tabuľky:

`SELECT
	cpay.industry_branch_code AS industry_code,
	cpib.name AS industry,
	round(avg(cpay.value), 2) AS average_wage,
	cpay.payroll_year AS in_year
FROM czechia_payroll cpay
LEFT JOIN czechia_payroll_industry_branch cpib 
	ON cpay.industry_branch_code = cpib.code
WHERE 1=1
	AND cpay.value_type_code = 5958
	AND cpay.calculation_code = 200
	AND cpay.industry_branch_code IS NOT NULL
GROUP BY cpay.industry_branch_code,
	 cpib.name,
	 cpay.payroll_year
ORDER BY cpay.industry_branch_code ,cpay.payroll_year;`
		 
Dáta boli uvedené štvrťročne, posledný rok 2021 len 2 štvrťročia, preto som si vytvorila priemernú ročnú mzdu a časové rozhranie je 2000 - 2021.  
Podmienky v klauzule WHERE:
`kód 5958 - zaistí obmedzenie výsledkov na priemernú hrubú mzdu na zamestnanca
kód 200 -  prepočítaný na počet zamestnancov na plný úväzok
industry_branch_code IS NOT NULL - nezobrazí mi priemer miezd za všetky odvetvia, došlo by tak k duplicitám`

K analýze ďalších otázok, som potrebovala pripojiť tabuľky **czechia_price** a **czechia_price_category**. 
V klauzule WHERE pribudla ďalšia podmienka `region_code IS NULL` - vyselektuje len priemernú cenu za všetky sledované regiony.
Informácie o cenách máme k dispozícii za obdobie 2006 - 2018.

A tak vznikla finálna primárna tabuľka:
(https://github.com/Lenkabj/Engeto-data-project-lenka-sorokova/blob/main/primary_table/t_lenka_sorokova_project_SQL_primary_final)
