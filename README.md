I componenti
con lista component puoi creare, visualizzare, modificare e infine eliminare un utente appena inserito

Le Funzionalità
Visualizzazione della lista dei clienti: La proprietà customers: Client[] contiene l'elenco dei clienti recuperati dal servizio. Il metodo getClient invoca il ClientService per ottenere la lista dei clienti.

Aggiunta di un nuovo cliente: Il metodo onSubmit consente di aggiungere un nuovo cliente quando selectedClientId è nullo. Se il modulo risulta valido, i dati del nuovo cliente vengono inviati al servizio attraverso addClient().

Modifica di un cliente esistente: Il metodo onEdit carica i dati di un cliente nel modulo per consentire le modifiche. userForm.patchValue inserisce i dati del cliente selezionato nel modulo. onSubmit gestisce anche l'aggiornamento del cliente 

Cancellazione di un cliente: Il metodo onDelete richiede una conferma prima di procedere con la cancellazione di un cliente. Se la conferma viene fornita, il metodo chiama onDeleteClient() nel servizio per rimuovere il cliente.
