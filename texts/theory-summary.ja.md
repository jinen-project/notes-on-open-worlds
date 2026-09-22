# 理論対応要約

本論の実装対応は、世界基底論、差異形式論、現象形態成立論の三部構成を崩さないことを前提とする。

## 第一部　世界基底論

世界基底論は、世界を記述するための基底を与える。
実装上は、`core/` のうち、最小形式、あらわれ、世界構造に対応する領域として扱う。

- 最小形式 -> `core/minimal-form/`
- あらわれ -> `core/appearing/`
- 世界構造 -> `core/world-structure/`

## 第二部　差異形式論

差異形式論は、第一部で与えられた基底を、差異化、同一化、形式化の観点から再記述する。
実装上は、`core/difference-form/` に対応する。

- 差異化 -> `differentiation.ts`
- 同一化 -> `identification.ts`
- 形式化 -> `form-expression.ts`
- 差異形式論の統合 -> `difference-form.ts`

## 第三部　現象形態成立論

現象形態成立論は、第一部と第二部を前提として、現象形態がどのように成立し、局所位置として取り扱い可能になるかを扱う。
実装上は、`phenomenal-form/` に対応する。

- 現象形態運動 -> `phenomenal-form/motion/`
- 現象形態 -> `phenomenal-form/form/`
- 現象形態工学 -> `phenomenal-form/engineering/`

## 実動作領域

理論の実動作は、次の領域に分かれる。

- 観測 -> `runtime/observe/`
- 判断 -> `runtime/judge/`
- 関与 -> `runtime/act/`
- 四相ループ -> `runtime/loop/`
- 入出力境界 -> `interface/contracts/`
- 局所位置化条件 -> `interface/local-position/`
- 記録 -> `logs/`

## 一文要約

レポジトリは、理論の三部構成をそのまま `core / phenomenal-form / runtime` へ対応させ、最小実装単位は「局所入力に対して余白・位置・関係を読み、差異化と同一化を判定し、関与可能性を返す単位」とする。
