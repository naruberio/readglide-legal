# Readglide 法務文書

iOS アプリ「Readglide」（テレプロンプター）のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/naruberio/teleprompter-app（Private）

## 公開 URL

GitHub Pages 有効化後、以下の URL で公開されます:

- プライバシーポリシー: https://naruberio.github.io/readglide-legal/privacy
- 利用規約: https://naruberio.github.io/readglide-legal/terms
- サポート: https://naruberio.github.io/readglide-legal/support

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語（既定）: `privacy.md` / `terms.md`

他言語は順次追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `teleprompter-app` の `docs/legal/` も合わせて更新する（両者は同一内容のミラー）。

プライバシーポリシー・利用規約の 4 ページ（`privacy*.md` / `terms*.md`）は、ここで直接直さない。`teleprompter-app` の `docs/legal/` を直してから、同リポジトリの `scripts/build_legal_pages.py` で作る（手順は `teleprompter-app` の `docs/legal/README.md`）。`support.md` と `index.md` はこのリポジトリで直接直す。

## サポート連絡先

konpei.work@gmail.com
