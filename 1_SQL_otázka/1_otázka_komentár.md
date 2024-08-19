## Výzkumná otázka: Rostou v průběhu let mzdy ve všech odvětvích, nebo v některých klesají?

Na zistenie odpovede 1. otázky som si pre prehľadnosť zobrazila mnou vytvorenú primárnu tabuľku, ktorá obsahuje všetky potrebné dáta.
Následne som si z tabuľky vyselektovala potrebné stĺpce a určila časové rozpätie 2000 - 2021. 
Finálny SQL dotaz je možno zobraziťzostaviť podľa toho, či chceme vidieť celkové ročné zmeny alebo len medziročné prírastky za jednotlivé odvetvia. Na základe SQL dotazov uvedených v zložke k 1.otázke môžeme vidieť, že okrem 3 odvetví (C - Zpracovatelský průmysl, Q - Zdravotní a sociální péče , S - Ostatní činnosti), došlo u všetkých minimálne raz za 21 rokov k medziročnému poklesu.
Na zistenie trendu medzi rokmi 2000 a 2021 som vytvorila dotaz pomocou klauzule WITH, ktorý nám jasne ukazuje, že mzdy vo všetkých odvetviach oproti roku 2000 vzrástli.
Najviac mzdy vzrástli v odvetví Q - Zdravotní a sociální péče, a to o skor 300%.

