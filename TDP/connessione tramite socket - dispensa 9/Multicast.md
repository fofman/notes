un insieme di processi in rete viene definito multicast. Un messaggio di un processo vesto un gruppo multicast viene recapitato a tutti i dispositivi del gruppo.
Viene utilizzato per: usernet news (pubblicazione e diffusione di notizie in tempo reale), videoconferenze, giochi multigiocatore, DNS, messaggistica, app P2P.

L'implementazione richiede:
- schema di indirizzamento
- supporto che registra i partecipanti nella rete
- ottimizzazione dell'uso della rete tramite multicast router

Per svolgere questo lavoro il protocollo più usato è IGMP (Internet Group Management Protocol) e serve per la gestione dei gruppi multicast.

In un gruppo multicast si ha la possibilità di unirsi, uscire, spedire a un gruppo e riceve messaggi indirizzati al gruppo.

La gestione dei gruppi è dinamica:
- un host può unirsi o abbandonare il qualsiasi momento
- Non bisogna per forza essere in un gruppo per inviare messaggi ad esso
- i membri non sono vincolati dall'architetura fisica (non deovno essere fisicamente nella stessa rete)

Per il multicast viene usata la classe D (iniziano con 1110), e varia da 224.x.x.x a 239.x.x.x (non hanno subnet).

I gruppi possono essere permanenti o temporanei, quelli permanenti vengono registrati presso IANA e quelli temporanei hanno bisogno di un protocollo per gestire il conflitto di per attribuzione degli indirizzi ed esistono finché ci sono host nel gruppo.
E' connectionless e viene usata per comunicare contemporaneamente con molte connessioni