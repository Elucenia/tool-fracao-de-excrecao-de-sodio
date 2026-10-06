<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · en · no clinical/professional/rights approval -->

# Fractional excretion of sodium (FENa)

[conditions, sources and permissions](https://elucenia.org/en/tools/fracao-de-excrecao-de-sodio)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Urine sodium

`una`

mEq/L · range: 1–300

### Serum sodium

`pna`

mEq/L · range: 100–180

### Urine creatinine

`ucr`

mg/dL · range: 1–500

### Serum creatinine

`pcr`

mg/dL · range: 0.2–20

### Diuretic use in the last 24 h?

`diuretico`

- `0` — No
- `1` — Yes

## Method edition

FENa/Espinel 1976; Miller 1978, 100×UNa×PCr/(PNa×UCr); simultaneous samples

## Documented formula

FENa (%) = (urine Na × serum creatinine) ÷ (serum Na × urine creatinine) × 100.

Use urine and blood collected at the same time, before diuretics or fluid administration whenever possible.

## Limits and population

Miller’s 1978 evidence concerns acute oliguria and showed that urinary indices do not always separate prerenal causes from tubular necrosis. The result alone does not establish the cause of renal dysfunction. Clinical conditions, sample timing and medications must be considered according to the source of the version used.

## References

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

FENa < 1%: suggests prerenal azotemia (tubule preserved, retaining sodium)


### 2

FENa between 1 and 2%: intermediate zone, interpret with the clinical picture


### 3

FENa > 2%: suggests acute tubular necrosis (intrinsic renal injury)

With a diuretic in the last 24 h, FENa rises even in the prerenal state: prefer the fractional excretion of urea.

