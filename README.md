# Words of Power - Veridion Side Challenge (HACKITALL 2025)

Acest repository este un fork al proiectului original dezvoltat în echipă în cadrul hackathon-ului HACKITALL (Martie 2025) pentru challenge-ul propus de Veridion.

Scopul aplicației a fost dezvoltarea unui sistem automat capabil să concureze într-un joc extins de "Piatră, Foarfecă, Hârtie", folosind un set masiv de cuvinte și reguli semantice.

## Contribuția mea
Deși am lucrat într-o echipă de doi oameni, responsabilitatea mea principală în acest proiect a fost **arhitectura și implementarea logicii de decizie**. Am dezvoltat sistemul capabil să analizeze cuvântul adversarului și să selecteze contra-atacul optim.

Principalele mele implementări includ:
* **Analiză Semantică (NLP):** Am integrat bibliotecile `nltk` și `WordNet` pentru a extrage dinamic sinonime și a mapa tematici de tip *counter* (ex: apă vs. foc, lumină vs. întuneric).
* **Euristica de Selecție:** Am construit algoritmul care identifică vulnerabilitățile cuvântului primit (analiza vocalelor unice, a lungimii și a caracterelor speciale) pentru a alege clasa de cost potrivită.
* **Optimizarea Deciziei:** Am implementat o funcție bazată pe greutăți (`weighted_choice`) care prioritizează cele mai eficiente cuvinte din punct de vedere al costului, maximizând șansele de câștig pe termen lung.
