# Readglide 法務文書

iOS アプリ「Readglide」（テレプロンプター）のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/naruberio/teleprompter-app（Private）

## 公開 URL

独自ドメイン `readglide.naruberio.com` で公開している（KAN-1085。`CNAME`・`_config.yml` の `url`。DNS は naruberio-site の NaruberioAppPages）。
旧 URL（`https://naruberio.github.io/readglide-legal/…`）は GitHub が同じパスへ 301 で転送するので（https への転送は Pages の「Enforce HTTPS」が有効なときだけ。切り替え後に `https_enforced` を確かめる）、アプリと App Store Connect の URL は変えていない。

- `sitemap.xml` は jekyll-sitemap が作る。`robots.txt` がその在りかを示し、Search Console（ドメインのプロパティ `naruberio.com`）と
  Bing Webmaster Tools に登録する

公開 URL:

- プライバシーポリシー: https://readglide.naruberio.com/privacy
- 利用規約: https://readglide.naruberio.com/terms
- サポート: https://readglide.naruberio.com/support

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語（既定）: `privacy.md` / `terms.md`

他言語は順次追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `teleprompter-app` の `docs/legal/` も合わせて更新する（両者は同一内容のミラー）。

プライバシーポリシー・利用規約の 4 ページ（`privacy*.md` / `terms*.md`）は、ここで直接直さない。`teleprompter-app` の `docs/legal/` を直してから、同リポジトリの `scripts/build_legal_pages.py` で作る（手順は `teleprompter-app` の `docs/legal/README.md`）。`support.md` と `index.md` はこのリポジトリで直接直す。

## サポート連絡先

konpei.work@gmail.com
