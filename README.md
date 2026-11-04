# NaturaSì Relex Category Optimizer (V2.5.5 BETA)
**Category Optimizer** è una Single-Page Application (SPA) avanzata, sviluppata per supportare gli Store Planner e i Category Manager nell'ottimizzazione dell'assortimento e nella parametrizzazione del software di Supply Chain **RELEX Solutions**.

## Architettura del Motore V2.5.5 (Revisione Certificata)
Questa release risolve definitivamente il disallineamento operativo ("effetto altalena") tra i moduli 3 e 4:
1. **Scudo Anti-Zombie in Sviluppo Assortimento (Tab 4):** Le referenze con giacenza non assortite (`isOrphan`) vengono promosse a "Giacenza Vendente" SOLO se registrano una rotazione solida accertata (almeno 1 pezzo a settimana oppure almeno 40 pezzi venduti in 365 giorni) e non sono dormienti da oltre 60 giorni. Tutte le code lente (1, 2, 5 o 10 pezzi/anno) vengono escluse da Tab 4 per evitare riordini accidentali a cartone.
2. **Scudo Prodotti Vivi in Razionalizzazione (Tab 3):** Nessun articolo attivo o con stock residuo viene proposto per lo spegnimento (`stato_relex: 'No'`) se ha venduto negli ultimi 30 giorni (`days <= 30`) o se registra una vendita annuale sana (almeno 20 pezzi nel Secco o 12 pezzi nel Non-Food), a prescindere dal fatto che appartenga a cluster facoltativi (`XXL`).
3. **Scudo Ruoli e Sbarramento Minimo sui Booster Dimensionali:** I booster `Deep` (+25%) e `Length 133` (+33%) si applicano unicamente alle categorie di Traffico e Destinazione ad alta rotazione (almeno 50 pezzi/anno o 1 pezzo a settimana).
4. **Color Blocking Selettivo:** Riservato a prodotti di Traffico dell'Area Secco e al reparto Cura Persona di Cosmesi.

## Utilizzo
L'applicazione è fruibile direttamente come Web App desktop da browser.
1. Carica il file esportato da RELEX (formato `.xlsx`) tramite il pulsante in alto a destra.
2. Seleziona le giornate di consegna settimanali del punto vendita.
3. Consulta e naviga i 5 moduli operativi (Setup, Diagnostica, Razionalizzazione, Sviluppo Assortimento, Rollout).
4. Utilizza i pulsanti di copia rapida sincronizzati per incollare i parametri direttamente in RELEX.

## Autore e Copyright
Progetto ideato, architettato e ingegnerizzato da **Massimo Maggipinto**, dipendente di EcorNaturaSì S.p.A.
Il Know-How logico e commerciale insito nell'applicazione è di proprietà intellettuale aziendale.
