**Trasmissione affidabile, duplex e ordinata.**
Nel caso di una comunicazione tramite stream socket vi deve essere un primo attore, il server, che offre un servizio ed è in linea teorica sempre raggiungibile (quindi sempre acceso). Un client può richiedere una connessione al server. La gestione del socket è molto simile ai file, infatti ci sono le solite azioni:
- apertura (del canale)
- lettura
- scrittura
- chiusura
I passaggi sono quelli tipici visti per l'architettura client/server:
- Un server è posto in ascolto su una porta
- Un client richiede una connessione
- Il server manda dei parametri necessari per la connessione