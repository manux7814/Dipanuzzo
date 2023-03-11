# Archivio (o file)
è un insieme di dati correlati identificato da un nome, memorizzato
permanentemente su un supporto di memoria di massa di un elaboratore e avente vita
indipendente dal/dai programmi utilizzati per la creazione e/o modifica
In un file i dati sono normalmente raggruppati in unità logiche denominate registrazioni o record.

# File sequenziale
i singoli record sono registrati uno di seguito all'altro, nell'ordine in cui sono stati
inseriti. Per accedere ad uno specifico record, bisogna "scorrere" tutti quelli che lo
precedono.l'operazione di ricerca può essere facilitata se i record risultano essere ordinati in
funzione del campo base rispetto al quale di effettua la ricerca.

# File ad accesso diretto
ogni singolo record è individuato da un numero che ne
rappresenta la posizione all'interno del file: quando i record sono inseriti sequenzialmente, il numero
è assegnato incrementando il numero dell'ultimo record memorizzato

# File indicizzato
nella struttura del record del file viene individuato un campo (o insieme di
campi) denominati chiave, i cui valori identificano univocamente i singoli record. In questo tipo di
organizzazione, oltre ad un file primario ad accesso diretto in cui sono memorizzati i record in
ordine di inserimento, viene gestito un ulteriore file indice contenente una tabella delle chiavi:
questa viene utilizzata dal codice che effettua l'accesso al file che la gestisce come un albero
binario di ricerca mantenendola costantemente ordinata secondo un criterio lessicografico.
La ricerca di uno specifico record avviene, a partire da un valore fornito in input, consultando la
tabella delle chiavi (ricerca rapida) e utilizzando la posizione de record per accedere al file
primario.

# Sistema informativo
viene utilizzato da un'organizzazione sia
pubblica che privata per il conseguimento di specifici obiettivi che
possono essere di due tipologie:

Operativo: tutte le organizzazioni hanno la necessità di gestire dati
funzionali alle loro attività operative (infrastrutture, dipendenti, materiali,
strumenti, ecc.) e da cui provengono informazioni "di servizio".

Decisionale: per poter prendere decisioni relative alle attività di
programmazione, controllo e valutazione un'organizzazione deve basarsi
su informazioni denominate "di governo"

E' un insieme strutturato di procedure e di risorse umane e materiali
finalizzate

• alla raccolta
• all'archiviazione
• all'elaborazione
• alla comunicazione
dei dati allo scopo di ottenere le informazioni necessarie ad un'organizzazione
per gestire sia le attività operative che di governo

# Sistema informatico
Con lo sviluppo delle tecnologie informatiche si sono ottenuti vantaggi
enormi per la gestione delle informazioni parallelamente alla loro
evoluzione e diffusione favorite anche dal progressivo abbassamento dei
costi – ne hanno reso sempre più conveniente l'impiego.

Un SISTEMA INFORMATICO è il sottoinsieme di un sistema
informativo dedicato al trattamento "automatico" di informazioni
derivanti dalla gestione di dati archiviati in formato digitale

# DBMS 
è un insieme di strumenti software che è in grado di gestire dati strutturati, 
è un sistema software in grado di gestire grandi collezioni di dati integrate, condivise e persistenti assicurando
loro affidabilità e privatezza.
deve essere efficiente ed efficace.
#### Caratteristiche 
- Gestire base di dati
- Persistenza e consistenza dei dati
- Privatezza e sicurezza dei dati
- Integrità dei dati
- Supporto alle transazioni
- Gestione del dizionario dei dati


# Indipendenza fisica
è la possibilità di modificare l'organizzazione fisica
dei dati senza dover modificare l'organizzazione logica 
e i programmi che lavorano sul db

# Indipendenza logica 
è la possibilità di modificare lo schema logico senza
dover modificare i programmi non interessati alla modifica

# Modello gerarchico
Ha caratterizzato i primi DBMS, sviluppati verso la
metà degli anni 60

I dati sono organizzati inrecord connessi tra di loro
secondo una struttura ad albero
Dunque, ciascun record può avere un unico padre

Possono esserci più record, su alberi diversi, che rappresentano la
medesima informazione
Ciò da luogo a problemi di ridondanza e di continui controlli sulla
consistenza dei dati
La manutenzione di un database gerarchico è complessa. Ad esempio:

- La cancellazione di un record comporta l’eliminazione di tutti i record
dipendenti da esso
- L’aggiornamento di un dato richiede la modifica di altri record per garantire la
consistenza del database

# Modello reticolare
È stato ideato negli anni 70 deriva da quello gerarchico ma lo
generalizza superando la rigidità della struttura ad albero
A differenza del modello gerarchico, un record può avere
uno o più record padre evitando così il problema legato alla
ridondanza dei dati
La gestione delle informazioni nei database costruiti secondo il
modello reticolare è comunque complessa

# Modello relazionale 
Fu proposto da Codd nel 1970 con una pubblicazione scientifica passata
alla storia dell’informatica
Il primo DBMS relazionale risale al 1981 ma inizia a prendere piede sul
mercato a metà anni 80
Ancora oggi, nonostante l’ingresso da qualche anno dei modelli ad
oggetti, il modello relazionale risulta quello più accreditato e
maggiormente utilizzato
Prende il suo nome dal concetto matematico di relazione
Le relazioni matematiche hanno una rappresentazione naturale per mezzo
di tabelle

# Regole di derivazione
- ogni Entità diventa un Archivio (Tabella)
- ogni Attributo di una Entità diventa il nome di un campo dell’archivio
- ogni campo eredita le caratteristiche (tipo e vincoli) dell’attributo dell’entità da cui deriva
- l’Identificatore univoco di una entità diventa Chiave Primaria
- L’associazione 1:1 definisce
o un archivio unico il cui tracciato record contiene i campi corrispondenti agli attributi della prima e seconda entità.
- Oppure due archivi differenti in cui nel primo viene aggiunto un campo che contiene i valori dell’identificatore della seconda entità che prende il ruolo di chiave esterna di collegamento ma senza valori ripetuti.
- L’associazione 1:N definisce due archivi differenti in cui nel secondo viene aggiunto un campo che contiene i valori dell’identificatore della prima entità che prende il ruolo di chiave esterna di collegamento e che può contenere valori anche ripetuti.
- L’associazione N:N definisce, oltre ai due archivi derivati dalle due entità, una nuova tabella che contiene gli identificatori univoci delle due entità e gli eventuali altri attributi dell’ associazione stessa compresa un identificatore univoco per essa.

# Ciclo di vita di un sistema informatico
Bisogni degli utenti -> raccolta richieste -> definizione requisiti
-> progettazione concettuale -> progetto concettuale -> realizzazione
-> progetto logico e fisico -> manutenzione/evoluzione

# Tipi di attributi
- semplici
- composti
- opzionali
- multipli
- derivati

# Relazione
Una relazione, è un legame logico che permette di aggregare informazioni cioè un insieme di colonne e righe, cioè attributi o campi dato insieme ai rispettivi dati o valori che vi compaiono

# DDL (Data Definition Language) 
DDL serve a creare, modificare o eliminare gli oggetti in un database. Sono i comandi DDL a definire la struttura del database e quindi dei dati ivi contenuti. Ma non fornisce gli strumenti per modificare i dati stessi: per tale scopo di usa il DML. L’utente deve avere i permessi necessari per agire sulla struttura del database e questi permessi vengono assegnati tramite il DCL (Data Control Language).

# DML (Data Manipulation Language)
DML fornisce i comandi per inserire, modificare, eliminare o leggere i dati all’interno delle tabelle di un database. La struttura di questi dati deve già essere stata definita tramite il DDL. Esempi di comandi sono SELECT,INSERT, UPDATE, DELETE ecc.

# DCL (Data Control Language)
DCL serve a fornire o revocare agli utenti i permessi necessari per poter utilizzare i comandi DML e DDL, oltre agli stessi comandi DCL (che gli servono per poter a sua volta modificare i permessi su alcuni oggetti).

# DQL (Data Query Language) 
DQL serve per creare query sui database e sui sistemi informativi da parte degli utenti oltre a rendere possibile l’estrazione di informazioni dal database interrogando la base dei dati interfacciandosi dunque con l’utente e le sue richieste di servizio.

# Query
### Elenco dei generi di film con la media degli incassi, ordinati per genere
##### select film.genere, AVG(programmato.incasso) from film inner join incasso on film.CodiceFilm = programmato.CodiceFilm GROUP BY film.Genere

### Elenco degli attori che hanno recitato nei film proiettati dopo il 1-1-2022
##### select attore.nome from attore inner join interpreta on interpreta.CodiceAttore = attore.CodiceAttore inner join film on film.CodiceFilm = film. CodiceFilm inner join programmato on film.CodiceFilm = programmato.CodiceFilm where programmato.DataProiezione > 1-1-2022

### Il nome e la citta del cinema più capiente (AGGIUNGERE GROUP BY ORDER E LIMIT)
##### select cinema.Nome, MAX(cinema.Posti) as "capienza", cinema.Citta from cinema group by cinema.Citta order by capienza desc limit 1
