# BankDB

- Progetto realizzato da Marco Cola [2079237] e Davide Martinelli [2077679] per il corso di Basi di Dati dell'a.a. 2023/2024.
- Per la descrizione del progetto vedi la [Relazione](Relazione.pdf)
  
### Accesso al Database da Terminale

Dopo aver [creato](/src/CreateTables.sql) e [popolato](/src/AllDataDump.sql) il DataBase,
- Aggiornare con la proprie credenziali la macro nel file .c per l'accesso a PostgreSQL
- Scaricare la cartella Dependencies
- Scaricare il file [codice.c](codice.c) nella stessa directory di Dependencies
- Da terminale posizionarsi nella Directory e compilare il codice con:
  
  ```c
  gcc codice.c -o codice -I /usr/include/postgresql -lpq

- il comando genera un eseguibile chiamato codice, da eseguire con il comando

  ```c
  ./codice
