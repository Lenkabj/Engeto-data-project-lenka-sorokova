## Otázka č.5: Má výška HDP vliv na změny ve mzdách a cenách potravin? Neboli, pokud HDP vzroste výrazněji v jednom roce, projeví se to na cenách potravin či mzdách ve stejném nebo násdujícím roce výraznějším růstem?


Výsledný dotaz som si zostavila pomocou Common Table Expression (CTE). Vytvorila som si 3 dielčie pomocné tabuľky - medziročné percentuálne zmeny HDP, miezd a cien, ktoré som nakoniec v daných rokoch porovnala. 

Z dát dostupných pre túto analýzu môžeme pre dané obdobie vypozorovať, že vývoj HDP, miezd a cien je v čase podobný.
Čo sa však týka citlivosti poklesu miezd pri výraznejšom spomalení HDP (-5%) rok 2009, mzdy rástli jak v tom istom roku, tak aj v roku nasledujúcom a jediný pokles miezd bol za celé sledované obdobie zaznamenaný len v roku 2013. Z toho sa dá usudzovať, že vývoj miezd okrem HDP ovplyvňujú aj iné ekonomické a celospoločenské faktory.
Pokiaľ by sme sledovali vývoj cien, najvýraznejší rast cien bol pri súčasnom poklese HDP v roku 2012 a 2013.

Na odpoveď, či sa rast DPH prejaví na cenách alebo mzdách toho istého roku alebo v tom ďalšom, by bolo vhodné previesť analýzu kvartálne. Výraznejší rast HDP v 1.kvartále môže ovplyvniť mzdy a ceny ešte v tom istom roku. Kdežto, ak by HDP výraznejšie vzrástlo v druhej polovici roka, reakcia miezd a cien by mohla byť badateľná až v roku nasledujúcom.
