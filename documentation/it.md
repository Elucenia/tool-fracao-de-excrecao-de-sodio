<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · it · no clinical/professional/rights approval -->

# Frazione di escrezione del sodio (FENa)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/fracao-de-excrecao-de-sodio)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sodio urinario

`una`

mEq/L · intervallo: 1–300

### Sodio sierico

`pna`

mEq/L · intervallo: 100–180

### Creatinina urinaria

`ucr`

mg/dL · intervallo: 1–500

### Creatinina sierica

`pcr`

mg/dL · intervallo: 0,2–20

### Uso di diuretici nelle ultime 24 h?

`diuretico`

- `0` — No
- `1` — Sì

## Edizione del metodo

FENa/Espinel 1976; Miller 1978, 100×UNa×PCr/(PNa×UCr); campioni simultanei

## Formula documentata

FENa (%) = (Na urinario × creatinina sierica) ÷ (Na sierico × creatinina urinaria) × 100.

Usare urine e sangue simultanei, prima di diuretici o liquidi se possibile.

## Limiti e popolazione

Le evidenze di Miller 1978 riguardano l’oliguria acuta e hanno mostrato che gli indici urinari non sempre distinguono le cause prerenali dalla necrosi tubulare. Il risultato da solo non stabilisce l’eziologia della disfunzione renale. Condizioni cliniche, momento del campionamento e farmaci devono essere considerati secondo la fonte della versione utilizzata.

## Riferimenti

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

FENa < 1%: suggerisce azotemia prerenale (tubulo preservato, con ritenzione di sodio)


### 2

FENa tra 1 e 2%: zona intermedia, interpretare con il quadro clinico


### 3

FENa > 2%: suggerisce necrosi tubulare acuta (lesione renale intrinseca)

Con diuretico nelle ultime 24 h, la FENa aumenta anche nello stato prerenale: preferire la frazione di escrezione dell’urea.

