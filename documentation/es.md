<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · es · no clinical/professional/rights approval -->

# Fracción de excreción de sodio (FENa)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/fracao-de-excrecao-de-sodio)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Sodio urinario

`una`

mEq/L · intervalo: 1–300

### Sodio sérico

`pna`

mEq/L · intervalo: 100–180

### Creatinina urinaria

`ucr`

mg/dL · intervalo: 1–500

### Creatinina sérica

`pcr`

mg/dL · intervalo: 0,2–20

### ¿Uso de diurético en las últimas 24 h?

`diuretico`

- `0` — No
- `1` — Sí

## Edición del método

FENa/Espinel 1976; Miller 1978, 100×UNa×PCr/(PNa×UCr); muestras simultáneas

## Fórmula documentada

FENa (%) = (Na urinario × creatinina sérica) ÷ (Na sérico × creatinina urinaria) × 100.

Use orina y sangre simultáneas, antes de diuréticos o aporte de volumen cuando sea posible.

## Límites y población

La evidencia de Miller 1978 se refiere a oliguria aguda y mostró que los índices urinarios no siempre separan las causas prerrenales de la necrosis tubular. El resultado no establece por sí solo la etiología de la disfunción renal. Las condiciones clínicas, el momento de las muestras y los medicamentos deben considerarse según la fuente de la versión utilizada.

## Referencias

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
