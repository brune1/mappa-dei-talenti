# Mappa dei Talenti

Una versione fatta da me di un test sui punti di forza, ispirato a CliftonStrengths, con una dashboard per vedere i risultati. L'ho costruita insieme a Claude (un modello di intelligenza artificiale) per capire come funzionano questi test prima di spendere dei soldi per quelli originali.

> **Questo test non ha validità scientifica.** È uno spunto di riflessione, non una misura psicologica e non sostituisce il test ufficiale di Gallup né una valutazione professionale.

**[Prova la dashboard online](https://brune1.github.io/mappa-dei-talenti/)**

## Perché l'ho creato

I test originali sui punti di forza sono a pagamento. Prima di spendere, volevo un'idea generale di come funzionano: come si passa da una serie di scelte a una classifica di talenti e che tipo di analisi se ne può ricavare. Ho preferito costruirne una versione mia, accettando in partenza che non abbia la stessa validità dell'originale.

Pubblico il progetto per mostrare **come ragiono** e **come uso l'IA per risolvere problemi di tutti i giorni**. Non serve a dimostrare la qualità tecnica della dashboard.

## Come l'ho realizzato con l'IA

Il lavoro è partito da un unico prompt scritto con cura, che trovi per intero in [`prompt/prompt-iniziale.md`](prompt/prompt-iniziale.md). Gli elementi su cui ho puntato:

1. **Obiettivo e contesto.** Ho spiegato a cosa serve il risultato (orientarmi nella mia carriera, non farmi valutare da qualcuno) e cosa volevo ottenere.
2. **Un ruolo chiaro.** Ho chiesto a Claude di comportarsi come un coach di carriera: concreto, empatico, orientato all'azione, senza gergo inutile.
3. **Un vincolo importante.** Le domande ufficiali di Gallup sono proprietarie: ho chiesto affermazioni originali e una dichiarazione esplicita, nella dashboard, che l'esito è indicativo.
4. **Passaggi e formato espliciti.** Coppie di affermazioni a scelta forzata, scala a 5 livelli, una domanda alla volta, calcolo dei punteggi, classifica, grafico dei 4 domini e analisi finale con sezioni definite.
5. **Un criterio di qualità.** L'analisi è ben fatta se è specifica sui risultati, spiega il perché delle conclusioni e lascia azioni concrete.

Claude ha scritto le affermazioni del test e costruito la dashboard. Anche la pubblicazione su GitHub è stata preparata con la sua guida, passo per passo.

## Come funziona

- **34 coppie di affermazioni originali.** In ogni coppia scegli quale ti descrive meglio e quanto, su 5 livelli (da "molto la prima" a "molto la seconda").
- **34 temi in 4 domini:** Esecuzione, Influenza, Costruzione di relazioni, Pensiero strategico. Ogni tema compare in due coppie.
- **Punteggio da 0 a 8 per ogni tema.** In caso di parità, l'ordine dipende dalla nettezza delle scelte e il pari merito è segnato con "=".
- **Risultati:** classifica completa dei 34 temi (con filtro per dominio), grafico dei 4 domini e un'analisi per la carriera calcolata dai punteggi.

## Come usarlo

1. Apri la [dashboard online](https://brune1.github.io/mappa-dei-talenti/). In alternativa scarica il progetto e apri `index.html` con un doppio clic: si apre nel browser, senza installare nulla.
2. Scegli **"Vedi i risultati dell'esempio"** per un esempio già compilato, oppure **"Inizia il test"** per rispondere tu.
3. Le tue risposte restano salvate solo nel tuo browser e puoi interrompere e riprendere quando vuoi.

## Perché i risultati mostrati sono un esempio

Per tutelare la mia privacy, questa versione pubblica non contiene il mio test effettivo ma un **esempio simulato**:

1. Ho tenuto fuori dal progetto le mie risposte e i miei risultati reali.
2. Ho inventato un profilo fittizio, con alcuni talenti molto marcati e altri quasi assenti.
3. Le 34 coppie sono state compilate in automatico in base a quel profilo.
4. Punteggi, classifica e analisi si calcolano come per qualsiasi persona.

## Limiti

- **Nessuna validità scientifica.** Le affermazioni sono scritte da un'IA e non sono state validate con alcuno studio.
- **Pochi dati per tema.** Con solo due risposte per tema, molti punteggi risultano uguali e punteggi vicini non sono davvero distinguibili.
- **Analisi di base.** In questa versione l'analisi è calcolata dalla pagina a partire dai punteggi. La riscrittura personalizzata con Claude funziona solo quando la pagina è aperta dentro Claude.
- **Provata solo in un browser simulato.** Non l'ho verificata su browser reali né su telefono.

## Nota sui marchi

CliftonStrengths è un marchio di Gallup, Inc. Questo progetto è indipendente: non è affiliato a Gallup né approvato da Gallup, e non riproduce domande o testi ufficiali. Le affermazioni sono originali.

## Licenza

Distribuito con licenza [MIT](LICENSE): puoi usare, copiare e modificare il progetto mantenendo la nota di copyright.
