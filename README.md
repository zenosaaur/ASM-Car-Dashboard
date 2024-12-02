# Menu Cruscotto Auto in Assembly

Progetto realizzato come parte del corso di **Architettura degli Elaboratori - Laboratorio** presso l'Università degli Studi di Verona (Anno Accademico 2022/2023).

## Descrizione

Questo progetto consiste nello sviluppo di un programma in Assembly che simula il menù di controllo di un cruscotto auto, con due modalità principali:

- **Utente (User)**: Accesso limitato alle funzionalità di base.
- **Supervisore (Supervisor)**: Accesso a funzionalità aggiuntive tramite l'inserimento del codice `2244`.

Il menù è navigabile tramite le frecce direzionali (su/giù/destra) e il tasto invio.

### Funzionalità

1. **Setting automobile**
2. **Data e ora**
3. **Blocco automatico porte (ON/OFF)**
4. **Back-home (ON/OFF)**
5. **Check olio**
6. **Frecce direzionali (solo Supervisore)**:
   - Numero di lampeggi modalità autostrada (2-5)
7. **Reset pressione gomme (solo Supervisore)**

La modalità supervisore aggiunge opzioni avanzate come il controllo dei lampeggi e il reset della pressione gomme.

### Requisiti

- Ambiente di sviluppo con supporto per linguaggio Assembly.
- Utilizzo dello stack per il passaggio di parametri tra funzioni.
- Terminale per l'inserimento dei comandi.

### Struttura del Progetto

Il progetto è organizzato nei seguenti file Assembly:

- `menu.s`: Funzione principale che gestisce il menù.
- `menuList.s`: Visualizzazione delle opzioni del menù.
- `isSupervisor.s`: Controllo accesso modalità supervisore.
- `getArrow.s`: Gestione dell'input da tastiera.
- `blinksManager.s`: Configurazione dei lampeggi.
- Vari file di utility per la gestione delle stringhe e della stampa.

### Diagramma di Flusso

Il programma segue una logica iterativa basata su cicli `while` e utilizza uno schema di controllo con strutture `switch` per navigare tra le opzioni del menù.

### Modalità di Esecuzione

1. Compilare i file Assembly utilizzando un assembler compatibile.
2. Eseguire il programma passando eventuali parametri (es. codice supervisore).
3. Utilizzare il terminale per navigare e modificare le opzioni del menù.

## Autori

- Mezzacasa Cristian (VR489474)
- Zeni Davide (VR486320)

## Licenza

Progetto sviluppato per scopi accademici. Non destinato all'uso commerciale.
