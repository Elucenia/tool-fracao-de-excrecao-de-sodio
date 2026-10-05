<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · pt-BR · no clinical/professional/rights approval -->

# Fração de excreção de sódio (FENa)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/fracao-de-excrecao-de-sodio)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sódio urinário

`una`

mEq/L · intervalo: 1–300

### Sódio sérico

`pna`

mEq/L · intervalo: 100–180

### Creatinina urinária

`ucr`

mg/dL · intervalo: 1–500

### Creatinina sérica

`pcr`

mg/dL · intervalo: 0,2–20

### Usou diurético nas últimas 24 h?

`diuretico`

- `0` — Não
- `1` — Sim

## Edição do método

FENa/Espinel 1976:Miller 1978,100×UNa×PCr/(PNa×UCr); amostras simultâneas

## Fórmula documentada

FENa (%) = (Na urinário × creatinina sérica) ÷ (Na sérico × creatinina urinária) × 100.

Use amostras de urina e sangue colhidas no mesmo momento, antes de diurético ou de volume, sempre que possível.

## Limites e população

A evidência de Miller 1978 refere-se à oligúria aguda e mostrou que índices urinários nem sempre separam causas pré-renais de necrose tubular. O resultado não estabelece sozinho a etiologia da disfunção renal. Condições clínicas, momento das amostras e medicamentos precisam ser considerados conforme a fonte da versão utilizada.

## Referências

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
