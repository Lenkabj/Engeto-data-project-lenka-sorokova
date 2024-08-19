## Výzkumná otázka: Kolik je možné si koupit litrů mléka a kilogramů chleba za první a poslední srovnatelné období v dostupných datech cen a mezd?

Pre zistenie odpovede na túto otázku som si najprv zobrazila primárnu tabuľku.
Následne som na základe pomocných SQL dotazov zistila prvé a posledné porovnateľné obdobie cien a miezd.
Následne som si spravila dielčie dotazy na kúpnu silu v roku 2006 a v roku 2018 pomocou WITH a tie som cez LEFT JOIN spojila a vyselektovala potrebné stĺpce.

Výsledkom je zistenie:

v roku **2006** sme si mohli kúpiť **1313 ks - Chléb konzumní kmínový** a **1466 l - Mléko polotučné pasterované**
a
v roku **2018** sme si mohli kúpiť **1365 ks - Chléb konzumní kmínový** a **1670 l - Mléko polotučné pasterované**

To znamená, že u obidvoch vybraných kategórií kúpna sila vzrástla.
