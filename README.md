### INTRO LARAVEL-> full-stack framework

'The php framework for web artisans'
!= linguaggio programmazione
= framework in php

framework: insieme di script , librerie, pacchetti che semplificano il flusso di lavoro

### DESIGN PATTERNS- mvc

sono dei metodi, delle linee guida che ci guidano durante la scrittura del nostro codice.

### MVC

un design pattern architetturale
mi permette di organizzare il codice secondo 3 concetti:

1. Model: cattura il comportamento dell'applicazione in termini di dominio del problema, MODELLIZZA UN ASPETTO DELLA REALTA', trasformandolo in una classe e fornendo alla logica della nostra app i metodi per accedere ai dati utili ad essa > model= dati(tipo quelli del database)
2. View: tutto cio' che appare all'utente che visita la piattaforma creata , la rappresentazione di output delle info + interazione utente
3. Controller: e' la logica dell'applicazione che fa da tramite tra il model(dati) e la view(output)in entrambe le direzioni.
   il controller, quindi, puo prendere i dati di Model e passarli a View e li attua m,odificando lo stato degli alrti due componenti

- il ponte tra i primi 2 aspetti

logica di business separata dalla logica di presentazione

Laravel segue questa architettura alla lettera MVC attraverso ad uno scheletro di cartelle e files precisi

- uscito da poco Laravel 11, anche se il rpogramma Laravel 10

le cartelle che frequenteremo piu spesso nei prox mesi
-app
-database
-resources
-routes

### DESCRIZIONE

Per prima cosa, creiamo un nuovo progetto Laravel 10, utilizzando questo comando:

composer create-project laravel/laravel:^10.0 laravel-primi-passi ok

Al termine dell'installazione, entriamo nella cartella del progetto cd laravel-primi-passi e avviamo l'artisan serve con uno di questi due comandi: php artisan serve oppure php -S localhost:8000 -t public
ok 

NB. devi essere nella cartella di progetto (quella con tutti i file) per poter avviare il comando artisan serve altrimenti.
NB2. quando installi laravel digitando il comando composer assicurati che abbia terminato l'installazione e che non si sia bloccato. Puoi capirlo controllando se nella cartella laravel-primi-passi c'é la cartella vendor se questa non épresente é probabile che l'instllazione non sia andata a buon fine a causa di qualche estensione di PHP mancante. In questo caso, guarda la registrazione.

### COMPOSER
simile npm, il nostro file delle dipendenze qui si chiama composer.json

in composer.lock e' presente delle librerie installate

come in npm abbiamo i node_modules, in php abbiamo i vendor
npm-> node_modules # dipendenze lato front-end
composer-> vendor # dipendenze lato back-end

ovviamente non serve pushare vendor

da ora MAMP lo tengo acceso per la questione server, ma il comando per avviare la mia app sara' 'php artisan serve', il comando nativo di php
questo comando mi apre un piccolo server in locale alla porta 8000 

### comandi laravel : php artisan/php list per vederli tutti , se ci aggiungi help prima del comando, lo spiega
-server locale -> php artisan serve
-creazione files php di qualsiasi tipo
-correzione bug
-aggiornamento 

# rapid prcesso reindirizzamentio da url a una determinata view 
nella cartella rooutes

in web.php definisco le logiche per i collegamenti tra pagine richieste tutte le rotte
ROUTE:: class di laravel stessa
richiamo metodo statico get

### BLADE
e' un template engine php

