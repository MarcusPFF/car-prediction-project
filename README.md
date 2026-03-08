# Maskinlæring til forudsigelser på bilpriser

Dette projekt handler om at analysere brugte biler i Danmark og bruge maskinlæring til at gætte priser og finde mønstre i markedet.

### 1) Which are the most decisive factors, forming the price of a car?
Alder og milage er de ting der betyder mest for prisen. Jo ældre bilen er og jo flere kilometer den har kørt jo mindre koster den. Motorstørrelsen spiller også en rolle men den er ikke lige så vigtig som de to andre ting.

### 2) Which make and model of a car is most popular, according this data source? Which are its technical characteristics?
VW er det mærke der optræder mest i data med modeller som Golf og Passat. De har tit motorer på 1.6 eller 2.0 liter og er kendt for at være stabile biler i mellemklassen.

### 3) Is there any obvious tendency in the preference of the car models during the past 5-10 years?
Folk vælger flere små biler og biler der kører langt på literen nu. Brændstoføkonomi er blevet vigtigere end store motorer på grund af priser og afgifter. Der er også kommet flere elbiler og hybrider ind i billedet.

### 4) Do people in Denmark prefer big or small cars? How reliable is your answer of this question?
Danskerne er glade for små biler da de er billigere i afgift og forsikring. Svaret er rimelig sikkert men det afhænger af om vores data dækker hele markedet eller kun en bestemt del.

### 5) Are there any locations in Denmark, where the expensive cars are preferred choice by the owners?
Dyre biler er mest udbredte i Nordsjælland og omkring København. Det hænger sammen med at indkomsten generelt er højere i de områder.

### 6) Which machine learning methods did you choose to apply in the solution and why?
Jeg brugte regression til at gætte priser da det handler om tal. Jeg brugte clustering til at finde grupper af biler der ligner hinanden og klassifikation til at vurdere om en bil er billig eller dyr.

### 7) How accurate are your solutions of prediction? Explain the meaning and the difference between the various quality measures?
Modellen kan forklare ca 61 procent af prisen. MAE viser den gennemsnitlige fejl i kroner mens RMSE straffer de store fejlskud hårdere. R2 scoren viser hvor god modellen samlet set er til at forstå data.

### 8) What could be done for further improvement of the accuracy of the models?
Præcisionen ville blive bedre hvis man tog bilens mærke og mængden af udstyr med i modellen. Ting som lædersæder eller soltag har stor betydning for prisen i den virkelige verden.

### 9) Which were the challenges in the project development?
Det sværeste var at rense data og få styr på alle de mærkelige tegn i kolonnerne. Det tog lang tid at få tallene gjort klar så modelerne kunne læse dem uden fejl. Eksempelvis "cmm2" skulle laves om til ccm
