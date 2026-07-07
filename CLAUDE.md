# CLAUDE.md — UNPLAN Village Hakuba 現地ガイドサイト

## このリポジトリは何か
UNPLAN Village Hakuba（白馬）の**宿泊者向け現地ガイド**サイト。素のHTML（フレームワーク無し）。
公式 unplan.jp とは別物で、宿泊者に向けた情報表示ページ。予約・公式・Instagram は外部リンクへ誘導する。

## 公開とデプロイ（最重要）
- ホスティング = **GitHub Pages**。公開URL: https://fika-tokyo.github.io/unplan-hakuba-guide/
- リポジトリ: https://github.com/fika-tokyo/unplan-hakuba-guide
- push アカウント: **Tsugaike-fika**（編集権限付与済み）
- **main ブランチに push すると、1〜2分で自動的に本番サイトへ反映**される
- ⚠ 旧 **Netlify版（unplan-hakuba-guide.netlify.app）はもう使わない**。Netlifyには触らない・デプロイしない。更新はこのGitHubリポジトリだけで行う（2か所を更新すると食い違うため）

## ファイル構成
日本語ページと英語ページが**別ファイル**になっている（全7ページ）：

| 内容 | 日本語 | 英語 |
|---|---|---|
| トップ | index.html（日英トグル併記） | （同左） |
| 宿泊案内 | stay.html | stay-en.html |
| 白馬ガイド | hakuba.html | hakuba-en.html |
| グリーンシーズン詳細 | green-season.html | green-season-en.html |

- `images/` … サイト内で使う画像（相対パス `images/xxx.jpg` で参照）
- CSS/JS は基本的に各HTML内に直書き。地図は green-season で Leaflet(CDN) を使用

## 編集時のルール
- ⚠ **日本語ページを直したら、対応する英語ページ（-en.html）も必ず直す**（逆も同様）。片方だけ直すと言語切替で内容が食い違う
- 画像を足すときは `images/` に置き、相対パスで参照する
- 編集が終わったら **commit → push**（= 自動で本番反映）

## 既知の未完成
- **冬（Winter）ガイドは hakuba.html 内で "Coming Soon" のまま**。素材が用意でき次第に追加する

## ブランド・トーン
- UNPLAN / FIKA。落ち着いた自然体のトーン。
- 動的機能（予約・問い合わせ・写真）は持たず外部に逃がす：予約=go-uvh.reservation.jp ／ 問い合わせ=unplan.jp/contact ／ 写真=Instagram
