**software progettato per supportare interoperabilità tra elaboratori con caratteristiche diverse in un contesto distribuito**.

Nel corso degli anni il web si è evoluto portando la necessità di standardizzarlo soprattutto sul lato dell'integrazione. Gli applicativi erano costruiti in maniera indipendente sregolata e con la diffusione di architetture completamente distribuite nasce la necessità di stabilire regole per l'utilizzo.

I primi esempi sono:
- Corba: standard multipiattaforma per linguaggi orientati agli oggetti
- Java RMI: standard per java
- DCOM: tecnologia proprietaria di Windows

La necessità era però quella di avere la totale interoperabilità tra sistemi e piattaforme diverse, permettendo di far comunicare processi in rete diversi fra loro indipendentemente dalla loro architettura hardware e software.
I primi esempi di realizzazione RPC sono basati su XML come linguaggio di markup per lo scambio permettendo di usare qualsiasi linguaggio di programmazione.

> [!NOTE] RPC
> RPC sta per Remote Procedure Call, ovvero un processo attivato da un computer diverso da quello da cui si esegue il programma (ad esempio le API)

## Caratteristiche di un web service
Un web service deve essere:
- auto-descrittivo: possiede una descrizione per l'utilizzo dei metodi
- auto-contenuto: i metodi sono utilizzabili indipendentemente dalla piattaforma, quindi senza requisiti.
## Vantaggi
- per chiamate al database, un web service può restituire i risultati senza permetterci di fare direttamente delle chiamate.



