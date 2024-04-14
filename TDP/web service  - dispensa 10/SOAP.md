SOAP (Simple Object Access Protocol) è un ==protocollo== per lo scambio di messaggi tra applicazioni realizzate con linguaggi e piattaforme diverse. SOAP ha un approccio basato su RPC, ovvero l'==invocazione di servizi remoti==.
## Ciclo di vita
1. **Pubblicazione**: il fornitore del servizio deve creare un ==documento WSDL== ovvero un documento XML che contiene la descrizione dei servizi che offre, quindi il nome dei metodi, i dati attesi in entrata e in uscita. Dopo la creazione del documento WSDL esso dovrà essere pubblicato in un registro che rispetto lo ==standard UDDI== che agisce da pagine gialle per il servizio che può essere rintracciato tramite ==chiamate di discovery==.
2. **Ricerca**: un cliente ==interroga il registro UDDI== per scoprire i servizi, in caso il cliente conosca già il servizio che gli serve può saltare questa fase.
3. **Ritorno WSDL**: se la ricerca ha successo ==viene restituito il documento WSDL== contenente i metodi per usare il servizio.
4. **Richiesta e risposta SOAP**: il client interroga il server tramite il componente ==stub== e il server tramite ==skeleton==, gestendo così la comunicazione in modo automatico.
### Compilazione
I due componenti stub e skeleton servono da adattatori fra il linguaggio di programmazione impiegato e lo standard per la comunicazione in modo da utilizzare un formato fisso che devono rispettare tutti.
##### struttura:
La struttura dei messaggi XML è formata da:
- ==**Envelope**==: contiene ==Header== e il ==Body==.
- **Header**: informazioni per routing e autenticazione.
- **Body**: contenuto utile.

La presenza di regole che aumentano la complessità di realizzazione ed e i tempi di elaborazione.
Oltre a questa struttura bisogna seguire standard di conformità, dettati dalle proprietà ACID:
- **(A) Atomicità**: i dati devono essere salvati 