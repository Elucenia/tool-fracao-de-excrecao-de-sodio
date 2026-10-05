<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · ja · no clinical/professional/rights approval -->

# ナトリウム排泄分画（FENa）

[条件・出典・許諾](https://elucenia.org/ja/tools/fracao-de-excrecao-de-sodio)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 尿中ナトリウム

`una`

mEq/L · 範囲: 1–300

### 血清ナトリウム

`pna`

mEq/L · 範囲: 100–180

### 尿中クレアチニン

`ucr`

mg/dL · 範囲: 1–500

### 血清クレアチニン

`pcr`

mg/dL · 範囲: 0.2–20

### 過去24 hに利尿薬を使用しましたか？

`diuretico`

- `0` — いいえ
- `1` — はい

## 方法の版

FENa/Espinel 1976；Miller 1978，100×UNa×PCr/(PNa×UCr)；同時採取

## 記載された計算式

FENa (%) = (尿中Na × 血清クレアチニン) ÷ (血清Na × 尿中クレアチニン) × 100。

可能なら利尿薬や補液前に同時採取した尿・血液を使う。

## 限界・対象集団

Miller 1978の証拠は急性乏尿についてのもので、尿の指標が常に腎前性の原因と尿細管壊死を区別するわけではないことを示しました。結果だけでは腎機能障害の原因は確定しません。臨床状態、採取時点、薬剤を、使用する版の出典に従って考慮する必要があります。

## 参考文献

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
