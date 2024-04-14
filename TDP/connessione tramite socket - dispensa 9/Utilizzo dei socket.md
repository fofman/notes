I [[Socket]] sono stati sviluppati come estensione del modello UNIX di I/O su file. tramite i socket abbiamo quindi 4 operazioni:
- open: apertura di un file
- read: lettura di un file
- write: scrittura su file
- close: terminazione nell'utilizzo
Questo modello permette di comunicare trattando le connessioni come file, usando quindi gli stessi metodi e concetti di programmazione che conoscono dalla gestione dei file locali.

> [!EXAMPLE] Esempio della semplicità
> In un linguaggio come python i dati vengono manda e riceve dati come stringhe che è effettivamente lo steso formato con cui leggiamo e scriviamo su file

---
Infine per realizzare una connessione si richiedono i dati che andranno a comporre L'[[Association]], ovvero:
- gli indirizzi
- il protocollo e il numero di porta
- il tipo di protocollo ([[TCP]]/[[UDP]])
---
Con l'utilizzo delle socket rese disponibili tramite delle API otteniamo un'astrazione user-friendly dei meccanismi basilari per l'implementazione di programmi client/server. Un socket è un'estremità per la comunicazione di due processi.
I socket non sono altro che un'interfaccia fra i livelli superiori e quelli inferiori che ci permettono di scrivere dei programmi senza preoccuparci di ciò che avviene nei livelli sottostanti.
Esistono 2 modi principali per la comunicazione in rete, orientato alla connessione e non orientato alla connessione.
I due modelli sono:
- [[Stream socket]] orientato alla connessione e utilizza il protocollo TCP.
- [[Socket a datagrammi]] non orientato alla connessione e utilizza il protocollo UDP.
- Raw socket

