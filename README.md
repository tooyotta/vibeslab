# Vibes Lab — 共通サイト

公開URL: https://tooyotta.github.io/vibeslab/

- `privacy/` — 全アプリ共通のプライバシーポリシー（日英）。共通方針＋アプリ別の項目
- `support/` — 全アプリ共通のサポート（連絡は GitHub Issues）
- App Store Connect のURL欄には、アプリごとにアンカー付きで入れる
  - プライバシー: `https://tooyotta.github.io/vibeslab/privacy/#<app>`
  - サポート: `https://tooyotta.github.io/vibeslab/support/#<app>`

## アプリを足すとき
1. `privacy/index.html` の「アプリ別」に `<section class="app" id="<app>">` を日英2か所追加（使う機能／保存／端末の外に出るもの）
2. `support/index.html` に同じ id でサポート項目を追加
3. `index.html` のアプリ一覧に追加
4. 最終更新日を更新して push（Pages に自動反映）

ストアに出していない Web 版アプリは、公開するときに足す（通信先が多いもの: michikusa は開発者の Worker 経由で位置情報を送る、等。正確に書くこと）。
