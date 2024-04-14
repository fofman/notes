SOAP (Simple Object Access Protocol) è un ==protocollo== per lo scambio di messaggi per l'invocazione di servizi in ambito web basandosi su un ==modello client-server== con chiamate RPC che veniva già utilizzato da protocolli come CORBA, DCOM e RMI.
## Ciclo di vita
1. **Pubblicazione**: il fornitore del servizio deve creare un ==documento WSDL== ovvero un documento XML che contiene la descrizione dei servizi che offre, quindi il nome dei metodi, i dati attesi in entrata e in uscita. Dopo la creazione del documento WSDL esso dovrà essere pubblicato in un registro che rispetto lo ==standard UDDI== che agisce da pagine gialle per il servizio che può essere rintracciato tramite ==chiamate di discovery==.
2. **Ricerca**: un cliente ==interroga il registro UDDI== per scoprire i servizi, in caso il cliente conosca già il servizio che gli serve può saltare questa fase.
3. **Ritorno WSDL**: se la ricerca ha successo ==viene restituito il documento WSDL== contenente i metodi per usare il servizio.
4. **Richiesta e risposta SOAP**: il client interroga il server tramite il componente ==stub== e il server tramite ==skeleton==, gestendo così la comunicazione in modo automatico.
### Compilazione
I due componenti stub e skeleton servono da adattatori fra il linguaggio di programmazione impiegato e lo standard per la comunicazione in modo da utilizzare un formato fisso che devono rispettare tutti.
##### struttura
La struttura dei messaggi XML è formata da:
- **Envelope**: contiene ==Header== e il ==Body==.
- **Header**