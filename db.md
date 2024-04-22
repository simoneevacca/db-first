## Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

DB_NAME: concessionario

Table name: auto


- id | INDEX | INT |    
- targa | INDEX | CHAR(7)   <!-- AA000AA -->
- marca | VARCHAR(10)
- modello | VARCHAR(15)
- alimentazione | VARCHAR(10)    <!-- benzina, metano, gpl, disel, elettrico... -->
- cilindrata | SMALLINT
- carrozzeria | VARCHAR(15)      <!-- SUV, fuoristrada, berlina, crossover... -->
- kilometri | SMALLINT
- cavalli | SMALLINT
- kilowatt | SMALLINT
- porte | CHAR(1)
- cambio | VARCHAR(15)       <!-- manuale, automatico, sequenziale... -->
- posti | CHAR(2)
- trazione | VARCHAR(15)        <!-- anteriore, posteriore, integrale... -->
- prima_immatricolazione | YEAR
- stato | VARCHAR(20)        <!-- come nuovo, KM0, leggermente usurato, molto usurato... -->
- prezzo | MEDIUMINT         
- è_trattabile | TINYINT        <!-- valore binario 1 = si, 0 = no -->
- colore | VARCHAR(15)      
- foto_1 | VARCHAR(255)     <!-- solo la prima foto è obbligatoria -->
- foto_2 | VARCHAR(255)
- foto_3 | VARCHAR(255)
- foto_4 | VARCHAR(255)
- foto_5 | VARCHAR(255)
- note | TEXT
