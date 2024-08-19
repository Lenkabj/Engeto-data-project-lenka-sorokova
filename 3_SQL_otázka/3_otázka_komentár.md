## Výzkumná otázka: Která kategorie potravin zdražuje nejpomaleji (je u ní nejnižší percentuální meziroční nárůst)?

Pri zisťovaní odpovede na túto otázku som si opäť dopomohla pomocnými tabuľkami CTE (WITH).
Najprv som si zobrazila celú primárnú tabuľku, z ktorej som následne vyselektovala potrebné dáta a určila časové rozpätie.
Následne som si pomocnou tabuľkou *previous_year_prices* zistila ceny za minulý rok, ďalšou pomocnou tabuľkou *percentage_yearly_changes*, som si zistila aké sú percentuálne ročné zmeny, a poslednou pomocnou tabuľkou *average_percentage_changes* som si zistila priemernú percentuálnu ročnú zmenu u jednotlivých kategórií za celé obdobie.
Nakoniec som si z poslednej vytvorenej pomocnej tabuľky vybrala potrebné stĺpce a výsledky zoradila podľa priemernej percentuálnej zmeny.

Výsledok je, že najpomalšie zdražuje **Cukr krystalový** - dokonca rast je záporný.
Z hľadiska rastu/ poklesu ceny je z dostupných dát najstabilnejšia kategória Rajská jablka červená kulatá (minimálny pokles ceny) a Banány žluté (minimálny rast ceny).
