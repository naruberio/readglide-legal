# Readglide 法務文書

iOS アプリ「Readglide」（テレプロンプター）のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/naruberio/teleprompter-app（Private）

## 公開 URL

GitHub Pages 有効化後、以下の URL で公開されます:

- プライバシーポリシー: https://naruberio.github.io/readglide-legal/privacy
- 利用規約: https://naruberio.github.io/readglide-legal/terms
- サポート: https://naruberio.github.io/readglide-legal/support

検索への登録:

- `sitemap.xml` は jekyll-sitemap が作る。Search Console の URL プレフィックス `https://naruberio.github.io/readglide-legal/` へ送信する
- `7833579911eb3524d6de4ae7e0c9fd6e.txt` は IndexNow の鍵（公開して使うもの）。ページを変えて公開したら、`keyLocation` をこのファイルにして通知する

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語（既定）: `privacy.md` / `terms.md`

他言語は順次追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `teleprompter-app` の `docs/legal/` も合わせて更新する（両者は同一内容のミラー）。

プライバシーポリシー・利用規約の 4 ページ（`privacy*.md` / `terms*.md`）は、ここで直接直さない。`teleprompter-app` の `docs/legal/` を直してから、同リポジトリの `scripts/build_legal_pages.py` で作る（手順は `teleprompter-app` の `docs/legal/README.md`）。`support.md` と `index.md` はこのリポジトリで直接直す。

## 使い方の場面（`scenes/`）

検索や AI の回答から拾われる入口として、用途別の説明ページを 3 場面 × en / ja / zh-Hans の 9 枚置いている。決まりと理由は `teleprompter-app` の `docs/decisions.md` が正本。`scenes/` の HTML はこのリポジトリで直接直す。

| 場面 | en | ja | zh-Hans | App Store へのリンクの `ct` |
|------|----|----|----|------|
| カメラ目線で原稿を読んで撮る | `scenes/read-script-on-camera.html` | `scenes/read-script-on-camera-ja.html` | `scenes/read-script-on-camera-zh-Hans.html` | `rgweb-camera-en` / `rgweb-camera-ja` / `rgweb-camera-zh` |
| 持ち時間のある発表 | `scenes/presentation-time-limit.html` | `scenes/presentation-time-limit-ja.html` | `scenes/presentation-time-limit-zh-Hans.html` | `rgweb-time-en` / `rgweb-time-ja` / `rgweb-time-zh` |
| 面接の受け答え | `scenes/interview-practice.html` | `scenes/interview-practice-ja.html` | `scenes/interview-practice-zh-Hans.html` | `rgweb-interview-en` / `rgweb-interview-ja` / `rgweb-interview-zh` |

- 書いてよいのは**公開中の版に入っている機能だけ**。手順のボタン名・欄の名前はアプリの表示（`Localizable.xcstrings` の en / ja / zh-Hans）とそろえる
- canonical・hreflang・`og:url`・JSON-LD の URL は今の github.io の URL で書く。独自ドメインへ移すときは一緒に直す
- 各ページは front matter に `layout: null` を書いてテーマを外し、`permalink` で拡張子なしの URL にしている。ページを変えたら `last_modified_at` と JSON-LD の `dateModified` も直す
- App Store へのリンクは `https://apps.apple.com/app/apple-store/id6799660946?ct=<上の値>&mt=8`。`pt` はまだ付けていないので、Analytics の Campaign には計上されない

## サポート連絡先

konpei.work@gmail.com
