# SQL Project Engeto data academy - Dostupnost základních potravin široké veřejnosti.

# Úvod do projektu

Tento projekt som vypracovala po skončení kurzu Engeto - Datová akademie. Jeho úlohou je si precvičiť nadobudnuté vedomosti SQL jazyka a vyskúšať si prácu datového analytika v reále a na skutočných dátach.

# Zadanie projektu

Na analytickém oddělení nezávislé společnosti, která se zabývá životní úrovní občanů, se dohodli, že se pokusí odpovědět na pár definovaných výzkumných otázek, které adresují dostupnost základních potravin široké veřejnosti. Kolegové již vydefinovali základní otázky, na které se pokusí odpovědět a poskytnout tuto informaci tiskovému oddělení. Toto oddělení bude výsledky prezentovat na následující konferenci zaměřené na tuto oblast.

Potřebují k tomu ode mne připravit robustní datové podklady, ve kterých bude možné vidět porovnání dostupnosti potravin na základě průměrných příjmů za určité časové období.

Jako dodatečný materiál je potřeba připravit i tabulku s HDP, GINI koeficientem a populací dalších evropských států ve stejném období, jako primární přehled pro ČR.

**Datové sady, které je možné použít pro získání vhodného datového podkladu**

**Primární tabulky:**

    **czechia_payroll** – Informace o mzdách v různých odvětvích za několikaleté období. Datová sada pochází z Portálu otevřených dat ČR.
    **czechia_payroll_calculation **– Číselník kalkulací v tabulce mezd.
    **czechia_payroll_industry_branch** – Číselník odvětví v tabulce mezd.
    **czechia_payroll_unit** – Číselník jednotek hodnot v tabulce mezd.
    **czechia_payroll_value_type** – Číselník typů hodnot v tabulce mezd.
    **czechia_price** – Informace o cenách vybraných potravin za několikaleté období. Datová sada pochází z Portálu otevřených dat ČR.
    **czechia_price_category** – Číselník kategorií potravin, které se vyskytují v našem přehledu.

**Číselníky sdílených informací o ČR:**

    **czechia_region** – Číselník krajů České republiky dle normy CZ-NUTS 2.
    **czechia_district** – Číselník okresů České republiky dle normy LAU.

**Dodatečné tabulky:**

    **countries** - Všemožné informace o zemích na světě, například hlavní město, měna, národní jídlo nebo průměrná výška populace.
    **economies** - HDP, GINI, daňová zátěž, atd. pro daný stát a rok. 

**Výzkumné otázky**

   1. Rostou v průběhu let mzdy ve všech odvětvích, nebo v některých klesají?
   2. Kolik je možné si koupit litrů mléka a kilogramů chleba za první a poslední srovnatelné období v dostupných datech cen a mezd?
   3. Která kategorie potravin zdražuje nejpomaleji (je u ní nejnižší percentuální meziroční nárůst)?
   4. Existuje rok, ve kterém byl meziroční nárůst cen potravin výrazně vyšší než růst mezd (větší než 10 %)?
   5. Má výška HDP vliv na změny ve mzdách a cenách potravin? Neboli, pokud HDP vzroste výrazněji v jednom roce, projeví se to na cenách potravin či mzdách ve stejném nebo násdujícím roce výraznějším růstem?    
                                                                                                                 zdroj: https://engeto.cz/

## Výstup projektu

Výstupom sú dve finálne tabuľky a sada SQL dotazov, pomocou ktorých je možné na výskumné otázky zodpovedať.
**t_lenka_sorokova_project_SQL_primary_final** (pre dáta miezd a cien potravín za Českú republiku zjednotených na totožné porovnatelné obdobie – spoločné roky)
**t_lenka_sorokova_project_SQL_secondary_final** (pre dodatočné dáta o ďalších evropských štátoch)

Postupy, analýzy a komentáre k jednotlivých výskumným otázkam sú rozdelené do samostatných zložiek repozitára.
                                                                                                                 


