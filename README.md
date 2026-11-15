# Margrow 法務ページ

iOS アプリ「Margrow」（旧 FlipProfit。転売の在庫・利益の台帳）のプライバシーポリシー・利用規約・サポートを GitHub Pages で公開するリポジトリ。
アプリのコード: https://github.com/koheiomorijp/flip-profit（Private。naruberio へ移す予定）

## 公開 URL

| ページ | URL | App Store Connect の欄 |
|---|---|---|
| プライバシーポリシー | https://naruberio.github.io/margrow-legal/privacy-policy | Privacy Policy URL |
| サポート | https://naruberio.github.io/margrow-legal/support | Support URL |
| 利用規約 | https://naruberio.github.io/margrow-legal/terms | 説明文の末尾・アプリの設定画面 |
| 日本語版 | `/privacy-policy-ja` ・ `/terms-ja` | ja ロケール |

## 用途別のページ（KAN-1242・案）

AI 検索・Web 検索から人を呼ぶための、1 ページ 1 用途の説明ページ。`guides/` に置き、テーマ（minimal）は使わず `guides/ledger.css` で描く。

| 用途 | en（正本） | ja |
|---|---|---|
| 転売の利益を計算する | `/guides/resale-profit` | `/guides/resale-profit-ja` |
| 仕入れと在庫の台帳をつける | `/guides/inventory-ledger` | `/guides/inventory-ledger-ja` |

- 書くのは公開中の版（2.0.0）にある機能だけ。ボタン名は flip-profit の `i18n/en.ts`・`i18n/ja.ts` と一字一句そろえる。古物台帳は ja だけの機能なので ja 版にだけ書く
- 無料の代替手段・アプリ自身の制約・価格と課金の形は書かない（soundpull-app D-58・D-59 を全アプリに当てる）
- 見える手順・FAQ と JSON-LD（HowTo・FAQPage）は同じ文にそろえる。片方だけ直さない
- App Store のリンクは `ct=mgweb-<用途>-<言語>`（`pt` が無いので Analytics のキャンペーンには出ない。流入は Web Referrer で見る）
- sitemap は `jekyll-sitemap` が出す（`/margrow-legal/sitemap.xml`）。Search Console・Bing への登録は @大森 の UI 操作

## 決めごと

- 中身はアプリの提出版に合わせる。通信・権限・保存先を変えたら同じ作業でここも直す
- 公開中の FlipProfit 1.0 は旧 URL（`flip-profit.vercel.app`）を指している。Vercel には出さず、新しい版で上の URL に替える
  （flip-profit `docs/decisions.md` D-05）
- 言語は en（正本）と ja
- 連絡先: konpei.work@gmail.com
