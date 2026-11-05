# NaturaSì Relex Category Optimizer (V3.5.0 BETA)
**Category Optimizer** è una Single-Page Application (SPA) avanzata, sviluppata per supportare gli Store Planner e i Category Manager nell'ottimizzazione dell'assortimento e nella parametrizzazione del software di Supply Chain **RELEX Solutions**.

## Architettura del Motore V3.5.0 (Integrazione Catalogo ECR 2.0)
Questa major release aggiorna la matrice del motore d'intelligenza artificiale, abbandonando l'euristica generica per integrare la classificazione ufficiale del portafoglio prodotti EcorNaturaSì:
1. **Assegnazione Ruoli Strategici:** I 4 ruoli (Traffico, Destinazione, Servizio, Impulso) sono ora assegnati in base a specifiche combinazioni di Reparto, Sottocategoria e fasce prezzo definite (es. Paste/Bevande vegetali base = Traffico, Macrobiotica = Servizio, Pet Care monoporzione = Impulso).
2. **Capitale Protetto Esteso:** La protezione della logistica contro l'Overstock (Vetrina o limitazione a 1 Collo) è stata allargata a tutte le referenze di "Servizio" del nuovo albero (oli monovarietali, mieli speciali, integratori, cosmesi curativa).
3. **Rollout Scientifico:** L'impianto prodotti sfrutta ora l'analisi ABC/XYZ calcolata in origine, escludendo i rami secchi a livello di rete e limitando l'ingombro finanziario in avvio.
4. **Scudi di Razionalizzazione (Tab 3) e Anti-Zombie (Tab 4):** Prodotti dormienti vengono disattivati chirurgicamente rispettando la vita utile della loro categoria.

## Utilizzo
L'applicazione è fruibile direttamente come Web App desktop da browser.
1. Carica il file esportato da RELEX (formato `.xlsx`) tramite il pulsante in alto a destra.
2. Seleziona le giornate di consegna settimanali del punto vendita.
3. Consulta e naviga i 5 moduli operativi (Setup, Diagnostica, Razionalizzazione, Sviluppo Assortimento, Rollout).
4. Utilizza i pulsanti di copia rapida sincronizzati per incollare i parametri direttamente in RELEX.

## Autore e Copyright
Progetto ideato, architettato e ingegnerizzato da **Massimo Maggipinto**, dipendente di EcorNaturaSì S.p.A.
Il Know-How logico e commerciale insito nell'applicazione è di proprietà intellettuale aziendale.
