# BankDB

- Progetto realizzato da Marco Cola [2079237] e Davide Martinelli [2077679] per il corso di Basi di Dati dell'a.a. 2023/2024.
- Per la descrizione del progetto vedi la [Relazione](Relazione.pdf)
  
### Accesso al Database da Terminale

Dopo aver [creato](/src/CreateTables.sql) e [popolato](/src/AllDataDump.sql) il DataBase,
- Aggiornare con le proprie credenziali le macro nel file .c per l'accesso al DB PostgreSQL
- Scaricare la cartella Dependencies, dopo aver installato la libreria [libpq](https://www.postgresql.org/docs/current/libpq.html):
  
  - ``sudo apt install libpq-dev``
    
  - nel caso si utilizzi Ubuntu installare anche libpq5:
    
  - ``sudo apt-get install libpq5``

- Scaricare il file [codice.c](codice.c) e posizionarlo nella stessa directory di Dependencies
- Da terminale posizionarsi nella Directory e compilare il codice con:
  
  ```c
  gcc codice.c -o codice -I /usr/include/postgresql -lpq

- il comando genera un eseguibile chiamato codice, da eseguire con il comando

  ```c
  ./codice
