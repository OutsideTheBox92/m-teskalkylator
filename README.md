# Möteskostnadskalkylator

En enkel, fristående möteskostnadskalkylator som visar hur mycket ett möte faktiskt kostar i pengar – per tillfälle, per månad och per år.

Syftet är att göra möteskostnaderna synliga, så att chefer, teamledare och projektgrupper kan fatta mer medvetna beslut om möteslängd, frekvens och deltagarlista.

## Funktioner

- Ange:
  - Titel på mötet
  - Antal deltagare
  - Genomsnittlig månadslön per person (brutto)
  - Möteslängd (i minuter)
  - Hur ofta mötet hålls (engångs, veckovis, varannan vecka eller månadsvis)
  - Valfri kommentar/kontext
- Kalkylerar:
  - Kostnad per möte
  - Kostnad per deltagare
  - Kostnad per månad (för återkommande möten)
  - Kostnad per år (för återkommande möten)
- Sparar varje beräkning i en lista i webbläsaren (localStorage)
  - Visar tidigare möten med kostnad per möte och per år
  - Möjlighet att ta bort enskilda sparade beräkningar
- Kopiera en textsammanfattning som kan klistras in i till exempel mejl, presentationer eller beslutsunderlag.

All beräkning sker i webbläsaren. Ingen data skickas till någon server.

## Beräkningar och antaganden

För att göra kalkylen enkel men användbar används följande antaganden:

- **Månadslön per person (brutto)** anges av användaren.
- **Sociala avgifter** antas vara 31,42 % av bruttolönen.
- **Arbetstid per månad** antas vara 160 timmar.

Utifrån detta räknas:

1. Månadskostnad per person inkl. sociala avgifter:
   > månadslön × (1 + 0,3142)
2. Timkostnad per person:
   > månadskostnad / 160
3. Kostnad per möte:
   > timkostnad × möteslängd (i timmar) × antal deltagare

För återkommande möten beräknas årskostnad och månadsmedel baserat på valt intervall (veckovis, varannan vecka eller månadsvis).

Dessa antaganden är förenklade, men räcker för att illustrera storleksordningen på vad möten faktiskt kostar.


## Användningsområden

- Underlag till diskussioner om möteskultur och effektivisering.
- Visualisera vad återkommande möten faktiskt kostar per år.
- Använd som stöd i:
  - Ledningsgruppsmöten
  - Retrospektiv och förbättringsarbete
  - Budget- och resursdiskussioner

Kalkylatorn är inte tänkt att avskaffa möten, utan att bidra till mer genomtänkta, fokuserade och värdeskapande möten.
