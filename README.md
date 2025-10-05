# Esercizi-Epicode-M5-W18

Ho scelto i file:	olist_orders_dataset, olist_order_items_dataset, olist_products_dataset, olist_order_reviews_dataset, olist_customers_dataset; li ho selezionati in modo da rendere il file non troppo pesante.
Ho preparato lo star schema, poi ho creato una tabella chiamata Calendar e ho creato le varie colonne tipo: anno, mese, meseDesc, trimestre, trimestreDesc.
Ho creato alcune DAX, tipo: ContOrdini = COUNTA(olist_order_items_dataset[order_item_id]), ContOrdini% = DIVIDE([ContOrdini] - [ContOrdiniPY], [ContOrdiniPY]), ContOrdiniPY = CALCULATE(olist_order_items_dataset[ContOrdini], PARALLELPERIOD('Calendar'[Date], -12, MONTH)); lo stesso fatto per i ricavi totali.
