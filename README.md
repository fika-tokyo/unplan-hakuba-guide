# UNPLAN Village Hakuba — 現地ガイドサイト

UVH（UNPLAN Village Hakuba）宿泊者向けの静的ガイドサイト。

- 公開URL（現行）: https://unplan-hakuba-guide.netlify.app/ ※作成者のNetlify上。会社管理への移行作業中
- 構成: 素のHTML 5ページ（**CSS/JSはHTML内に直書き**）＋ `images/`（ローカル画像8点）
  - `index.html` … トップ（日英トグル）
  - `stay.html` / `stay-en.html` … 宿泊のご案内（日 / 英）
  - `hakuba.html` / `hakuba-en.html` … 白馬ガイド（日 / 英）
- フォント: Google Fonts（Outfit / Noto Sans JP）をCDN参照
- 一部の写真は unplan.jp（WordPress）の画像を外部URLで参照

## 編集方法
各HTMLを直接編集 → `main` に push（公開先を接続後は自動反映）。
**日本語版・英語版は別ファイル**なので、内容を変えるときは両方を直す。

## 由来・残作業
- 2026-06-22、公開中サイトからファイルを取り込み、会社組織 [fika-tokyo](https://github.com/fika-tokyo) に取り込み。
- 作成者に確認予定: 元ソース（変換前ファイル）の有無 / 冬ガイド（Coming Soon）の素材 / 旧Netlify公開の停止・引き継ぎ。
