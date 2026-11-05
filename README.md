## ニューラルネットワーク・ビジュアルプレイグラウンド

ブラウザ上で層数・ニューロン数・活性化関数をUIで設定してXOR/円/螺旋問題の分類境界をリアルタイム可視化するNN学習デモ。

### 機能
- Canvas 2D による2D分類境界カラーマップ表示
- 問題セレクト: XOR / 円 / 螺旋（点群を描画）
- ネットワーク設定: 隠れ層数（1-3）・ニューロン数（2-8）・活性化関数（ReLU/Sigmoid/Tanh）
- バックプロパゲーション + SGD を純粋 JavaScript で実装
- 学習/停止トグルボタンで requestAnimationFrame ループ実行
- 損失曲線リアルタイム表示（Canvasグラフ）
- ネットワーク構造を SVG でノード・エッジ可視化（重み符号を色で表現）
- 精度・損失・ステップ数のリアルタイム表示

### 技術
- 静的SPA（index.html単体）
- Tailwind CSS CDN
- Canvas 2D API / requestAnimationFrame
- バックプロパゲーション: 純粋 JavaScript 実装（外部MLライブラリ不使用）
- SVG 動的生成（ネットワーク構造可視化）
