# Vibes Lab — 共通サイト

公開URL: https://tooyotta.github.io/vibeslab/

- `privacy/` — 全アプリ共通のプライバシーポリシー（日英）。共通方針＋アプリ別の項目
- `support/` — 全アプリ共通のサポート（連絡は GitHub Issues）
- `terms/` — 全アプリ共通の利用規約（日英）。共通の条件＋アプリ別の条件（UGC・医療でない・ライセンス等）。App Store では Apple 標準 EULA と併用
- App Store Connect のURL欄には、アプリごとにアンカー付きで入れる
  - プライバシー: `https://tooyotta.github.io/vibeslab/privacy/#<app>`
  - サポート: `https://tooyotta.github.io/vibeslab/support/#<app>`
  - 利用規約（説明文の末尾・アプリ内リンク用。ASC の EULA 欄は Apple 標準のまま）: `https://tooyotta.github.io/vibeslab/terms/#<app>`

## アプリを足すとき
1. `privacy/index.html` の「アプリ別」に `<section class="app" id="<app>">` を日英2か所追加（使う機能／保存／端末の外に出るもの）
2. `support/index.html` に同じ id でサポート項目を追加
3. 固有の条件（UGC・AI・第三者コンテンツ・医療/法律でない等）があれば `terms/index.html` にも同じ id で日英追加
4. `index.html` のアプリ一覧に追加
5. 最終更新日を更新して push（Pages に自動反映）

ストアに出していない Web 版アプリは、公開するときに足す（通信先が多いもの: michikusa は開発者の Worker 経由で位置情報を送る、等。正確に書くこと）。
