# loto6-cycle-analysis
ロト6の解析サイト(Javascript版)
# ロト6,7 周期性分析 v2（論理合成つき）

このプロジェクトは **ロト6,7 の抽選データを対象に、周期性やパターンを可視化・分析するためのWebアプリケーション** です。  
フロントエンドのみで動作し、PCやスマートフォンのブラウザ上で利用できます:contentReference[oaicite:0]{index=0}。

## 主な機能

- **通常分析**  
  最新回と直近 N 回のデータを比較し、出現パターンを可視化。

- **ずらし検証**  
  各開催回ごとに直前 N 回の出現傾向を解析。

- **予測 v2（論理合成つき）**  
  - 複数の「窓」（直近 N 回など）を選択して AND/OR/差/NOT の論理合成が可能。  
  - 多数決ロジックやスコア付き一覧による候補選定。  
  - 式ビルダー機能（例: `(N=6 & N=9) - N=12` など）。

- **組合せ統計**  
  過去データに基づき、指定サイズの数値組合せの出現回数を集計・ランキング表示。

- **データ入力**  
  - CSV またはテキスト形式でのデータ読込に対応。  
  - サンプルデータ読込ボタンあり。  
  - スマホでも操作しやすいUI。

## 技術スタック

- HTML5 / CSS3 / JavaScript
- [Tailwind CSS](https://tailwindcss.com/)  
- [Bootstrap 5.3](https://getbootstrap.com/)  
- [Chart.js](https://www.chartjs.org/)  

外部ライブラリは CDN 経由で読み込んでいます:contentReference[oaicite:1]{index=1}。

## ファイル構成
/
├─ index.html # メイン画面
├─ images/
│ ├─ loto_analysis_logo.png
│ └─ loto_favicon_16x16.png


- `index.html` : アプリ本体
- `images/loto_analysis_logo.png` : ロゴ画像
- `images/loto_favicon_16x16.png` : ファビコン

## 利用方法

1. このリポジトリをクローンまたはダウンロード
2. `index.html` をブラウザで開く
3. 「データ入力」セクションからサンプルやCSVを読み込み、各機能を実行

## GitHub Pages で公開する場合

リポジトリの **Settings → Pages** から `main` ブランチ / ルート (`/`) を指定してください。  
公開URLは `https://ユーザー名.github.io/リポジトリ名/` になります。

---

© 2025 ロト6 周期性分析 v2

