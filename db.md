## Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

DB_NAME: concessionario

Table name: auto


- id | INDEX | INT | PK | AUTO_INCREMENT | NOTNULL   
- targa | INDEX | CHAR(7) | UNIQUE | NULL   <!-- AA000AA -->
- marca | VARCHAR(10) | NOTNULL
- modello | VARCHAR(15) | NOTNULL
- alimentazione | VARCHAR(10) | NOTNULL    <!-- benzina, metano, gpl, disel, elettrico... -->
- cilindrata | SMALLINT | NOTNULL
- carrozzeria | VARCHAR(15) | NULL      <!-- SUV, fuoristrada, berlina, crossover... -->
- kilometri | SMALLINT | NULL
- cavalli | SMALLINT | NOTNULL
- kilowatt | SMALLINT | NOTNULL
- porte | CHAR(1) | NULL
- cambio | VARCHAR(15) | NULL       <!-- manuale, automatico, sequenziale... -->
- posti | CHAR(2) | NULL
- trazione | VARCHAR(15) | NULL        <!-- anteriore, posteriore, integrale... -->
- prima_immatricolazione | YEAR | NOTNULL
- stato | VARCHAR(20) | NULL        <!-- come nuovo, KM0, leggermente usurato, molto usurato... -->
- prezzo | MEDIUMINT | NULL         
- è_trattabile | TINYINT | NULL        <!-- valore binario 1 = si, 0 = no -->
- colore | VARCHAR(15) | NULL      
- foto_1 | VARCHAR(255) | NULL | DFAULT('https:foto-di-default-.jpg')     
- foto_2 | VARCHAR(255) | NULL
- foto_3 | VARCHAR(255) | NULL
- foto_4 | VARCHAR(255) | NULL
- foto_5 | VARCHAR(255) | NULL
- note | TEXT
