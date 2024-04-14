I computer connessi in rete che devono comunicare fra loro devono avere delle regole per consentire il corretto dialogo, queste regole prendono nome di protocollo di comunicazione.

> [!important] Definizione
> Con protocollo di comunicazione si intendono tutte le regole necessarie per permettere a due interlocutori di comprendersi

- Il protocollo stabilisce tutti gli aspetti della comunicazione dal logico al fisico.
- I protocolli sono organizzati secondo una gerarchia che prevede che ogni protocollo di un determinato livello si appoggi a dei protocolli nel livello inferiore per fornire un servizio di qualità.

> [!example] Esempio di protocollo
> Il protocollo è un insieme di regole che fa affidamento anche a protocolli nei livelli sottostanti, un esempio è http che gestisce l'interpretazione ma fa affidamento al protocollo TCP per la comunicazione che a sua volta farà affidamento ad protocollo nel livello sottostante


![[Pasted image 20240405162349.png]]

Ad ogni livello i dati prendono nomi diversi:

| Livello      | Nome dato |
| ------------ | --------- |
| Applicazione | Messaggio |
| Trasporto    | segmento  |
| Rete         | datagram  |
| Collegamento | frame     |
I protocolli di comunicazione standard usati sono [[TCP]] e [[UDP]]