=============
Registrazione
=============

|product| offre la possibilità di tenere sotto controllo i parametri critici di funzionamento tramite 
il :index:`Centro Servizi` Nethesis, accessibile con la coppia utente/password all'indirizzo https://register.nethesis.it.
Come prima operazione, per ogni |product| installato, è necessario effettuare la 
registrazione per permettere una corretta identificazione nella comunicazione con la console web.

Accedere all'interfaccia web del server (https://server:980), fare click su :guilabel:`Gestione pacchetti` e seguire la procedura guidata:

* Inserire le credenziali rivenditore utilizzate presso il sito https://register.nethesis.it
* Selezionare un server esistente oppure scegliere la creazione di nuovo server
* In caso di creazione assicurarsi di inserire un nome che faciliti l'identificazione del server. Si consiglia anche di immettere una descrizione
* Associare un cliente esistente al nuovo server oppure compilare i campi per la creazione di nuovo cliente
* Confermare i dati immessi per terminare la procedura di registrazione

Al termine sarà possibile installare il software aggiuntivo.

L'installazione di software aggiuntivo dall'interfaccia web è permessa esclusivamente solo ai possessori delle credenziali rivenditore.
L'utilizzo di :command:`yum` da linea di comando permette di aggirare questa limitazione. Pertanto si sconsiglia di consegnare la password di :dfn:`root` all'utente finale.

Il modulo utenti consente di utilizzare l'utente :dfn:`admin` per accedere all'interfaccia web con privilegi amministrativi. 
L'utente :dfn:`admin` potrà quindi configurare l'intero sistema ma non potrà installare software aggiuntivo. 
Per maggiori informazioni, vedi :ref:`admin-user`.


:index:`Codice server`
======================

Il :dfn:`codice server` permette di identificare in modo univoco il server all'interno del Centro Servizi Nethesis (http://register.nethesis.it).
Nel dettaglio del server presente sul Centro Servizi Nethesis sono presenti due pulsanti chiamati 
:guilabel:`Libera Chiave` e :guilabel:`Elimina Server`, ognuno dei quali ha una funzione ben specifica.

:index:`Elimina Server`
-----------------------

Il pulsante :guilabel:`Elimina Server` serve per eliminare dal Centro Servizi Nethesis i server non più utilizzati o erroneamente creati.

:index:`Libera chiave`
----------------------

Il pulsante :guilabel:`Libera Chiave` serve per permettere ad un altro server di registrarsi con una chiave già utilizzata, 
il suo utilizzo tipico è in caso reinstallazione. Può capitare che sia necessario reinstallare il server per sostituire 
dell'hardware o per installare una versione più recente. 

In assenza dell'opzione :guilabel:`Libera Chiave` sarebbe necessario eliminare il vecchio firewall e crearne uno con una nuova chiave, 
in questo modo tra l'altro si perderebbero anche i dati relativi allo storico della macchina in questione. 
Tramite il pulsante :guilabel:`Libera Chiave` è invece possibile registrare il server appena ripristinato con la stessa chiave 
che c'era prima del ripristino, senza dover modificare altro.
