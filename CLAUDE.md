# Tick Timer

## プロジェクトの目的
calisthenicsのISOホールド計測用のWebアプリ。
広告なし、無制限カウント。YouTubeの代替。

## 配信先
GitHub Pages（リポジトリ直下のindex.htmlを配信）

## 制約
- 1ファイル完結（index.html のみ）
- 外部依存なし（ただしGoogle FontsのCDNは可）
- ビルドステップなし（プレーンHTML/CSS/JS）
- モバイル/デスクトップ両対応

## コーディング方針
- バニラJS（フレームワーク不使用）
- AudioContextはユーザー操作後にresume()
- タイマーは performance.now() でドリフト補正
- アクセシビリティ: キーボード操作対応（Space=toggle, R=reset）

## デザイン方針
- ダークテーマ、機能美、ミニマル
- カウンター表示は遠目でも見える大きさ（calisthenicsで床から見るため）
- 不要な装飾は省く

## Definition of Done
- [ ] index.htmlを開いてStartボタンで動作する
- [ ] スマホのSafari/Chromeで動作確認済み
- [ ] 1時間以上連続動作してもズレない
- [ ] GitHub Pagesに配置して公開URLで動作する