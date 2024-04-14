Un socket è un'interfaccia di programmazione che consente la comunicazione fra processi differenti. I processi possono essere sia in rete che locali.
I socket sono composti da una coppia di informazioni, l'indirizzo e la porta. Attraverso delle apposite API i sistemi operativi abilitano all'uso dei socket di rete.
## Caso d'uso per una comunicazione locale
Due processi che si trovano ==sulla stessa macchina== devono comunicare fra loro utilizzano l'interfaccia delle socket che in questo utilizzo vengono definite ==Unix-domain socket== (AF_UNIX).
AF sta per Address Family.
## Caso d'uso per una comunicazione in rete
Per la comunicazione in rete verranno usati i socket di tipo ==Internet== (AF_INET) e vengono quindi utilizzati per comunicazioni di ==host remoti==, non per forza sulla stessa rete.

> [!EXAMPLE] Esempio di socket
> 10.145.6.72:3400

Il numero dopo i due punti prende il nome di porta logica.
[[Le porte logiche]]
