# GestionaleSpese
Applicativo sviluppato in Java che permette all'utente di gestire le proprie spese, dividendole per categoria, con la possibilità di gestirle, 
ovvero visualizzarle, modificarle, vederle o eliminarle, realizzato con JAVA e MySQL.

Requisiti
Java Development Kit (JDK) versione 20 o superiore
MySQL Server
Librerie JDBC per MySQL (solitamente fornite dal driver MySQL)

Importare il progetto in un IDE JAVA come Eclipse o Visual Studio Code

Assicurarsi che il server MySQL sia in esecuzione sulla propria macchina locale o sia accessibile.

Configurare le credenziali di accesso al database nel file DatabaseConnection.java.

Eseguire il file DatabaseSetup.java per creare il database e le tabelle necessarie.

Eseguire l'applicazione eseguendo la classe GestionaleMain.java.

Utilizzo
Una volta avviata l'applicazione sarà possibile:

Visualizzare le proprie spese e aggiungerne di proprie compilando i campi proposti nell'interfaccia grafica.
Visualizzare le categorie presenti. All'avvio saranno caricate 6 categorie che non saranno mai modificabili o eliminabili dall'utente,
ma sarà possibile aggiungerne di personalizzate dalla stessa tab in cui vi è la lista generale, inserendone il nome e una breve descrizione.
Sarà possibile filtrare nell'apposita tab le spese per data o categoria di appartenenza.
Infine è possibile eliminare o modificare una spesa o una categoria, in due tab separate, inserendo l'apposito ID e i dati necessari in caso di modifica.

N.B. Questa è una versione aplpha. Si prevendono future implementazioni come:
- il totale degli importi delle spese, sia per la visualizzazione generale che per il filtraggio
- nuove opzioni di filtraggio per anno e mese
- implementazione della stampa anche nelle operazioni di filtraggio
- impedimento dell'eliminazione di una categoria personalizzata se legata ad una spesa presente del database

Struttura del Progetto
Il progetto è strutturato come segue:
- src/GestioneSpese: Contiene il codice sorgente JAVA.
- GestionaleMain.java: Classe principale dell'applicazione che gestisce l'interfaccia grafica e le interazioni con il database.
- Categoria.java: Classe che rappresenta una Categoria.
- Spesa.java: Classe che rappresenta una Spesa.
- SpeseCRUD: Classe per l'accesso ai dati delle Categorie e delle Spese nel database.
- Pdf.Java: Classe che gestisce i metodi per la stampa dei PDF.
- DatabaseConnection.java: Classe per la gestione della connessione al database.
- DatabaseSetup.java: Classe per la creazione delle tabelle e l'inserimento di dati di esempio nel database.
