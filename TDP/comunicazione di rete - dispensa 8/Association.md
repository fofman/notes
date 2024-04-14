L'association è una struttura che consente di identificare in modo univoco ogni singola connessione.

> [!EXAMPLE] Esempio di Association
> TCP, 192.168.1.2, 1500, 192.168.1.14, 21
> In questo esempio identifichiamo i seguenti elementi:
> - procollo da utilizzare
> - Indirizzo IP del mittente
> - Porta del mittente
> - Indirizzo IP del destinatario
> - Porta del destinatario

I server che sono gli erogatori di servizi sono sempre in ascolto in una determinata porta, i client sono innumerevoli e richiedendo lo stesso servizio passano nella stessa porta. In questo esempio si potranno identificare le connessioni singole con l'associazione, che ad esempio potrà distinguere le connessioni con i singoli client.