Il livello 4 Trasporto (Transport Layer in inglese) ha come compito di consegnare e ordinare i pacchetti per i livelli superiori. In questo caso il destinatario non è un host su una rete bensì un processo all'interno di un host.
Ogni host solitamente possiede una sola porta fisica che riceve dati in entrata che interessano più processi, è quindi necessario contraddistinguere i singoli pacchetti in base al processo a cui devono essere consegnati, questa tecnica viene chiamata ==multiplazione==. Per contraddistinguere i processi vengono utilizzate [[Le porte logiche|le porte logiche]].
Il livello 4 lavora su dei pacchetti chiamati *segmenti*.
Il livello 4 esegue la frammentazione per rispettare la lunghezza massima dei pacchetti includendo i dati per ricostruire il pacchetto all'arrivo.
I livello 4 può eseguire il controllo di flusso per protocolli connessi come [[TCP]].
