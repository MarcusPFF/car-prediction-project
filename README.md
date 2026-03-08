# Maskinlæring til forudsigelser på bilpriser

Dette projekt handler om at analysere brugte biler i Danmark og bruge maskinlæring til at gætte priser og finde mønstre i markedet.

## Projekt Svar

**1) Hvad betyder mest for prisen?**
Det er helt klart milage (kilometer) og alder. Jo flere kilometer den har kørt, jo billigere bliver den. CCM (motorstørrelse) har også noget at sige, da store motorer tit koster mere, men det er alder og km, der rykker mest i regnestykket.

**2) Hvilken bil er mest populær?**
Hvis man kigger på antallet i datasættet, så er det VW (Volkswagen) og især deres Golf eller Passat, der går igen. De ligger tit med en 1.6 eller 2.0 motor og har omkring 100-150 hestekræfter. Det er den klassiske mellemklasse-bil i Danmark.

**3) Tendens de sidste 5-10 år?**
Der er kommet mange flere små biler og elbiler/hybrider. Folk kigger meget mere på MPG (hvor langt de kører på literen) nu end før i tiden. De gamle store benzinslugere er ikke så populære som de var engang, fordi afgifterne og benzinpriserne er steget.

**4) Store eller små biler i DK?**
Danskerne elsker små, økonomiske biler (micro-cars), fordi de er billige i afgift og forsikring. Men mit svar her er kun så pålideligt som de data, vi har skrabet. Hvis vi kun har data fra én bestemt hjemmeside eller ét år, så mangler vi måske det fulde billede af hele markedet.

**5) Er der steder i DK med ekstra dyre biler?**
Ja, det ses tydeligt i data omkring Nordsjælland og Region Hovedstaden. Der er gennemsnitsprisen på bilerne bare højere end i f.eks. Nordjylland. Det giver også god mening, da det er der, de højeste indkomster ligger.

## Machine Learning Metoder

**6) Hvilke ML metoder og hvorfor?**
Jeg har brugt tre forskellige ting:
* **Regression:** Til at gætte selve prisen, fordi det handler om tal.
* **Clustering:** Til at se om bilerne naturligt delte sig op i grupper (ligesom segmenter).
* **Classification:** Til at se om modellen kunne gætte om en bil var i det billige eller dyre segment.

**7) Hvor præcis er din model?**
Min model rammer omkring 60-70% rigtigt (R2-score). 

* **MAE:** Fortæller mig bare, hvor mange kroner jeg i gennemsnit skyder ved siden af (ca. 48.000 kr).
* **RMSE:** Er lidt strengere og viser om jeg laver nogle rigtig store fejl. 
* **R2:** Er ligesom en karakter fra 0 til 1 på hvor godt modellen forstår sammenhængen.

**8) Hvordan kan det blive bedre?**
Modellen mangler at vide noget om udstyr (lædersæder, soltag osv.) og bilens stand. Hvis jeg også kunne få "Brand" (om det er en Audi eller en Fiat) kodet bedre ind i modellen, ville den gætte meget mere præcist, fordi mærket betyder vildt meget for prisen.

**9) Hvidke var de største udfordringer?**
Rengøring af data var det sværeste! Der var mærkelige navne som `ccm2` og kolonner med `d` i (døre), som skulle laves om til tal før computeren fattede det. Og så det med at vælge de rigtige features, så modellen ikke bare gættede i øst og vest.