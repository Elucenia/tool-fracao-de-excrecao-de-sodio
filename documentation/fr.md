<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · fr · no clinical/professional/rights approval -->

# Fraction d’excrétion du sodium (FENa)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/fracao-de-excrecao-de-sodio)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Sodium urinaire

`una`

mEq/L · intervalle: 1–300

### Sodium sérique

`pna`

mEq/L · intervalle: 100–180

### Créatinine urinaire

`ucr`

mg/dL · intervalle: 1–500

### Créatinine sérique

`pcr`

mg/dL · intervalle: 0,2–20

### Prise de diurétique dans les dernières 24 h ?

`diuretico`

- `0` — Non
- `1` — Oui

## Édition de la méthode

FENa/Espinel 1976 ; Miller 1978, 100×UNa×PCr/(PNa×UCr) ; prélèvements simultanés

## Formule documentée

FENa (%) = (Na urinaire × créatinine sérique) ÷ (Na sérique × créatinine urinaire) × 100.

Prélevez urine et sang simultanément, avant diurétique ou remplissage si possible.

## Limites et population

Les données de Miller 1978 concernent l’oligurie aiguë et ont montré que les indices urinaires ne distinguent pas toujours les causes prérénales de la nécrose tubulaire. Le résultat n’établit pas seul l’étiologie de la dysfonction rénale. Les conditions cliniques, le moment des prélèvements et les médicaments doivent être considérés selon la source de la version utilisée.

## Références

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

FENa < 1 % : suggère une azotémie prérénale (tubule préservé, rétention de sodium)


### 2

FENa entre 1 et 2 % : zone intermédiaire, à interpréter avec le contexte clinique


### 3

FENa > 2 % : suggère une nécrose tubulaire aiguë (atteinte rénale intrinsèque)

Avec un diurétique dans les dernières 24 h, la FENa augmente même en état prérénal : privilégier la fraction d’excrétion de l’urée.

