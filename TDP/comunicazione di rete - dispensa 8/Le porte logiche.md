#### Che scopo hanno?
Un computer ha una sola porta fisica per la connessione ma più applicazioni necessitano di utilizzare la rete. Proprio per identificare i diversi processi si usano queste porte.

---
Ogni processo in rete deve essere identificato in modo unico tramite i socket.
Le porte logiche sono individuate da 2 byte e sono quindi 2^16 ovvero 65536. Queste porte logiche si dividono in 3 categorie.

| Range porte | Denominazione                |
| ----------- | ---------------------------- |
| 0-1023      | Well-Known Ports             |
| 1024-49151  | Registered Ports             |
| 49152-65535 | Dynamic and/or Private Ports |
- Well-Known Ports: sono riservate ad applicazioni particolari che permettono il corretto funzionamento di funzioni essenziali
- Registered Ports: porte registrate presso IANA per determinati servizi, possono comunque essere usate a piacimento dagli utenti
- Dynamic and/or Private Ports: Porte libere che possono essere usate liberamente dagli applicativi

> [!important] N.B.
>Non basta solo il numero di porta per identificare in modo univoco un processo che usa una connessione. Più processi possono usare la stessa porta.
>Per identificare un processo applicativo in modo univoco viene impiegato l'utilizzo dei socket.
>Il risultato è detto [[Association]]
>



