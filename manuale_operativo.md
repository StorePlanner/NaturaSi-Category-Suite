# Manuale Operativo: NaturaSì Relex Category Optimizer (V2.0)

Benvenuti nella guida ufficiale all'uso del **NaturaSì Relex Category Optimizer**. Questa applicazione è stata progettata per assistere gli Store Planner e il personale di negozio nella gestione quotidiana del riordino, incrociando i freddi dati statistici di RELEX con la realtà fisica e visiva dello scaffale (Visual Merchandising).

## 1. A Cosa Serve? (La Missione dell'App)

Molti sistemi di riordino ragionano solo sui numeri: se vendi un vasetto a settimana, il sistema ordina un solo vasetto. Tuttavia, uno scaffale con un solo pezzo comunica un senso di vuoto al cliente. D'altro canto, ordini manuali eccessivi fatti "per paura di rimanere senza" generano enormi sprechi (sfridi) e immobilizzano il capitale del negozio.

L'**Optimizer** funge da arbitro neutrale:

* **Traduce i dati in spazi:** Calcola quanti pezzi formano una "massa visiva adeguata" in base alle dimensioni del prodotto e ai multipli d'acquisto (colli).

* **Abbassa lo stress:** Trasforma ore di estrazioni, VLOOKUP e controlli incrociati in un'analisi automatica di pochi secondi.

* **Tutela i margini:** Taglia i rami secchi, svuota i magazzini da referenze in eliminazione e riduce lo spreco alimentare sui prodotti freschi.

Tutta l'elaborazione avviene **localmente sul tuo computer**: non serve connessione internet e nessun dato sensibile viene inviato all'esterno.

## 2. Come Funziona: Il Flusso di Lavoro (Workflow)

L'utilizzo dell'applicazione si articola in **4 semplici passaggi**:

1. **Estrazione da RELEX:** Scarica dal sistema RELEX il file Excel (`.xlsx`) contenente l'anagrafica e le metriche di vendita del tuo punto vendita.

2. **Caricamento (Drag & Drop):** Trascina il file Excel all'interno dell'app (oppure clicca sul tasto "Carica Export").

3. **Impostazione Calendario:** Nella barra in alto, seleziona i giorni esatti in cui il negozio riceve lo scarico merce (LUN, MAR, ecc.) e se la domenica è aperta o chiusa. L'algoritmo ricalcolerà immediatamente il fabbisogno logistico in base alle tue consegne.

4. **Copia & Incolla:** Naviga tra i 5 moduli, analizza i dati e usa i tasti **"Copia Codici"**, **"Copia MIN"** e **"Copia MAX"**. Torna su RELEX, seleziona la prima cella utile e fai "Incolla".

## 3. I 5 Moduli Operativi

L'interfaccia è divisa in 5 schede di lavoro (Tab), ciascuna identificata da un colore specifico.

### 🔵 1. Setup Parametri (Impostazione Base)

* **Cosa fa:** Elabora il cuore logistico e visivo del negozio per i prodotti **attivi**. Calcola il Minimo ideale (Fabbisogno + Scorta Visiva) e il Massimo (solo per i prodotti costosi).

* **Novità:** Applica il *Color Blocking*, ovvero uniforma automaticamente i minimi dei prodotti appartenenti allo stesso brand e linea, garantendo uno scaffale ordinato e senza salti visivi.

### 🟣 2. Diagnostica Assortimentale (Il Microscopio)

* **Cosa fa:** È il modulo di audit. Non ti mostra tutto il listino, ma filtra **solo le anomalie e gli errori**.

* **Cosa rileva:** Minimi troppo bassi su Top Seller, prodotti in giacenza ma inattivi, errori critici di configurazione del Massimo (es. Massimo inferiore al Minimo + Collo). Ti suggerisce l'azione correttiva esatta.

### 🔴 3. Razionalizzazione (Taglio dei Rami Secchi)

* **Cosa fa:** Isola i prodotti in esaurimento o che non generano più valore.

* **Tasti Operativi:**

  * `Attivi da Razionalizzare`: Filtra i prodotti a cui limitare le scorte (es. Vetrina *Max 1* per prodotti costosi o *Capping a 1 cartone* per svuotare il magazzino centrale).

  * `Deadstock`: Filtra i "morti certi". Articoli da spegnere definitivamente (`Assortimento: NO`).

### 🟢 4. Sviluppo Assortimento (Le Opportunità Gaps)

* **Cosa fa:** Scova i "Top Performer" di catena che nel tuo negozio sono inspiegabilmente spenti. Ti suggerisce di attivarli e include un tasto per generare automaticamente il file `.TXT` per la stampa dei frontalini a scaffale.

### 🟠 5. Rollout Negozio (Gestione Nuovi Inserimenti)

* **Cosa fa:** Elenca i prodotti non ancora attivi ordinandoli per "Priorità Aziendale" (Must Have, Core Brand, Top Seller). Assegna loro una massa visiva prudenziale per non intasare il magazzino durante un refitting.

## 4. Come Ragiona: Il Cuore dell'Algoritmo (Motore 2.0)

La versione 2.0 dell'Optimizer non fa calcoli piatti, ma analizza il database come farebbe un Category Manager esperto, applicando 5 logiche avanzate:

### A. I 4 Ruoli di Categoria

Incrociando l'Area (Fresco, Secco, Cosmesi) e il Prezzo di vendita, l'app assegna a ogni prodotto un Ruolo Strategico visibile a schermo:

1. `[🎯 Destinazione]` (es. Legumi vetro, Ortofrutta): Core business. Massima protezione contro spegnimenti affrettati.

2. `[🚀 Traffico]` (es. Basi pizza, Latte fresco): Prodotti ad altissima rotazione. Il minimo è calcolato per garantire tolleranza zero ai buchi a scaffale.

3. `[💎 Servizio]` (es. Cosmesi Dr. Hauschka, Vini bio): Prodotti premium ad alto margine. Scatta la **Regola Vetrina (Max 1)** per non immobilizzare liquidità in negozio.

4. `[⚡ Impulso]` (es. Snack, Cioccolato in cassa): Acquisti non pianificati. Subiscono soglie di inattività più severe se non ruotano.

### B. Matrice RELEX (ABC / XYZ)

L'app legge la classificazione RELEX del prodotto. Se un articolo è un Top di Fatturato (**Classe A**) o ha una domanda storicamente stabile (**Classe X**), riceve uno "scudo algoritmico": non verrà mai proposto tra i Deadstock per un banale rallentamento temporaneo delle vendite, proteggendo il fatturato del negozio.

### C. Fabbisogno Predittivo (Machine Learning)

Il calcolo delle scorte non guarda più solo al passato. L'app utilizza la `Previsione media giornaliera` calcolata dall'Intelligenza Artificiale di Sede. In questo modo, i Minimi si alzano *prima* dell'arrivo di un picco stagionale (es. lieviti a Pasqua o solari a giugno), prevenendo lo stock-out.

### D. Prevenzione dello Sfrido Alimentare

L'algoritmo monitora il campo `Scaduto`. Se un prodotto deperibile (es. Freschissimo) ha generato sfridi nei mesi precedenti, il sistema applica una sforbiciata del 50% al Minimo suggerito per limitare lo spreco, segnalandolo con il badge `[⚠️ Rischio Sfrido Storico]`.

### E. Gestione Speciale Stati di Sede (35 e 20)

* **Stato 35 (Rottura Fornitore):** I prodotti indisponibili dal polo non vengono puniti per i giorni di mancata vendita. L'app li "congela", pronti a ripartire al rientro della merce.

* **Stato 20 (Pre-Eliminati):** Se un prodotto a fine vita vende ancora, l'app non lo spegne brutalmente (bloccando la merce nel CEDI), ma applica un **Capping Logistico** (`Min: 0 | Max: 1 Cartone`). Questo permette al magazzino centrale di svuotarsi progressivamente senza intasare i punti vendita.

## 5. Avvertenze Tecniche e Tips

* **Modifica della Vista:** Cliccando sulle intestazioni di colonna, puoi ordinare i dati. Cliccando sull'icona a imbuto (▼) puoi filtrare i dati come in Excel.

* **Copia Singola Riga:** Cliccando col tasto destro sul numero di una riga, apparirà un menu per copiare solo quella specifica riga (utile per consultazioni veloci).

* **⚠️ Allerta Copia MASSIMI (Molto Importante):** Quando clicchi su "Copia MAX", l'app invierà un comando "vuoto" per cancellare i tetti massimi errati su RELEX. Tuttavia, le griglie dei gestionali spesso *ignorano* le celle vuote provenienti dagli appunti. Prima di incollare, **ricordati sempre di cancellare fisicamente la colonna su RELEX**, altrimenti i vecchi valori rimarranno bloccati. Un popup rosso ti ricorderà di farlo ad ogni operazione.

*Supporto Tecnico: Per anomalie o richieste di integrazione, fare riferimento alla funzione di estrazione dati e verificare la corretta esportazione delle colonne standard di RELEX.*