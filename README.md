# KEYFLOW Analyzer

A keyboard layout analyzer with editable cost models (transition/static), fatigue recovery, and statistical efficiency metrics.

---

## Quick Start
Open the app in your browser:

- https://koyasi777.github.io/keyflow-analyzer/

## Features
- **Logical domain**
  - Layout editor (rename / mask / drag-swap)
  - Fingering assignment
  - Presets (QWERTY / Dvorak / etc.)
- **Physical domain**
  - Position cost (static)
  - Transition cost (dynamic)
  - Fatigue & recovery simulation (gap-based)
  - Repeat penalty (same key)
  - Weighting: Position vs Transition
- **Metrics**
  - Efficiency score (Cost/Key)
  - Cost distribution histogram
  - Stability metrics: Median / SD / 95th percentile
  - SFB rate, repeats, worst transitions
  - Finger/row load charts

## How to Use
1. Configure your layout and finger assignments:
   - **Logical** → Layout / Fingering
2. Tune the cost model:
   - **Physical** → Position Cost / Transition Cost / Logic
3. Paste corpus text (Romaji / alphanumeric recommended) and click **Analyze**.

## Import / Export
- Import/Export is available from the UI.
- **Logical** data and **Physical** config are exported separately:
  - Logical: layout + fingers + name
  - Physical: costs + baseCosts + gapConfig + repeatCosts + weights
- Copy/Paste JSON in the modal window.

## Notes
- The default cost model is a starting point. Tune it to match your keyboard, posture, and preferences.
- For Japanese evaluation, input **Romanized text** (Romaji).

## License
MIT

---

# 日本語 (Japanese)

編集可能なコストモデル（遷移/位置）と疲労回復モデルに基づき、統計的指標で配列効率を評価するキーボード配列アナライザです。

## クイックスタート
ブラウザで以下にアクセスするだけで起動します：

- https://koyasi777.github.io/keyflow-analyzer/

## 主な機能
- **Logical (配列設計)**
  - レイアウト編集（リネーム / マスク(無効化) / ドラッグ入れ替え）
  - 運指割当
  - プリセット（QWERTY / Dvorak / など）
- **Physical (物理設定)**
  - 位置コスト（Static）
  - 遷移コスト（Transition）
  - 疲労と回復のシミュレーション（交互打鍵=回復、gapベース）
  - 同キー連打ペナルティ
  - 位置/遷移の重み付け（スコア比率）
- **指標 (Metrics)**
  - 総合スコア（Cost/Key）
  - コスト分布ヒストグラム
  - 安定性指標（中央値 / SD(ムラ) / 95%タイル）
  - SFB率、連打、ワースト遷移
  - 指負荷/段負荷チャート

## 使い方
1. 配列と運指を設定します：
   - **Logical** → Layout / Fingering
2. コストモデルを調整します：
   - **Physical** → Position Cost / Transition Cost / Logic
3. 評価用テキスト（ローマ字/英数字推奨）を貼り付けて **Analyze** を実行します。

## Import / Export（JSON）
- UIから Import / Export できます。
- **配列データ（Logical）** と **物理設定（Physical）** は別々にエクスポートされます：
  - Logical: layout + fingers + name
  - Physical: costs + baseCosts + gapConfig + repeatCosts + weights
- モーダルに表示されるJSONをコピー/貼り付けしてください。

## 注意
- デフォルトのコストモデルは“たたき台”です。使用環境（キーボード/姿勢/好み）に合わせて調整してください。
- 日本語の評価は **ローマ字入力テキスト**を推奨します。

## ライセンス
MIT
