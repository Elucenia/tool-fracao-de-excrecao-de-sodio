<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · zh · no clinical/professional/rights approval -->

# 钠排泄分数（FENa）

[条件、来源与许可](https://elucenia.org/zh/tools/fracao-de-excrecao-de-sodio)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 尿钠

`una`

mEq/L · 范围: 1–300

### 血清钠

`pna`

mEq/L · 范围: 100–180

### 尿肌酐

`ucr`

mg/dL · 范围: 1–500

### 血清肌酐

`pcr`

mg/dL · 范围: 0.2–20

### 过去 24 h 是否使用利尿剂？

`diuretico`

- `0` — 否
- `1` — 是

## 方法版本

FENa/Espinel 1976；Miller 1978，100×UNa×PCr/(PNa×UCr)；同时采样

## 已记录的公式

FENa (%) = (尿Na × 血清肌酐) ÷ (血清Na × 尿肌酐) × 100。

尽可能使用同时采集、利尿剂或补液前的尿液及血液样本。

## 限制与适用人群

Miller 1978的证据涉及急性少尿，并显示尿液指标并不总能区分肾前性病因与肾小管坏死。结果本身不能确定肾功能障碍的病因。应按照所用版本的来源考虑临床状况、采样时间和药物。

## 参考文献

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
