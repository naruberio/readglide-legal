# Readglide 法務文書

iOS アプリ「Readglide」（テレプロンプター）のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/naruberio/teleprompter-app（Private）

## 公開 URL

独自ドメイン `readglide.naruberio.com` で公開している（KAN-1085。`CNAME`・`_config.yml` の `url`。DNS は naruberio-site の NaruberioAppPages）。
旧 URL（`https://naruberio.github.io/readglide-legal/…`）は GitHub が同じパスへ 301 で転送するので（https への転送は Pages の「Enforce HTTPS」が有効なときだけ。切り替え後に `https_enforced` を確かめる）、アプリと App Store Connect の URL は変えていない。

- `sitemap.xml` は jekyll-sitemap が作る。`robots.txt` がその在りかを示し、Search Console（ドメインのプロパティ `naruberio.com`）と
  Bing Webmaster Tools に登録する
- `<32 桁の 16 進>.txt` は IndexNow の鍵（公開して使うもの）。ページを変えて公開したら、`keyLocation` をこのファイルにして IndexNow に通知する

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

## 使い方の場面（`scenes/`。KAN-1130・teleprompter-app D-52）

検索や AI の回答から拾われる入口として、用途別の説明ページを 3 場面 × en / ja の 6 枚置いている。`scenes/` の HTML はこのリポジトリで直接直す。

| 場面 | en | ja | App Store へのリンクの `ct` |
|------|----|----|------|
| カメラ目線で原稿を読んで撮る | `scenes/read-script-on-camera.html` | `scenes/read-script-on-camera-ja.html` | `rgweb-camera-en` / `rgweb-camera-ja` |
| 持ち時間のある発表 | `scenes/presentation-time-limit.html` | `scenes/presentation-time-limit-ja.html` | `rgweb-time-en` / `rgweb-time-ja` |
| 面接の受け答え | `scenes/interview-practice.html` | `scenes/interview-practice-ja.html` | `rgweb-interview-en` / `rgweb-interview-ja` |

- 書いてよいのは**公開中の版に入っている機能だけ**（iTunes Lookup で版を確かめる）。手順のボタン名・欄の名前は、アプリの表示（`teleprompter-app` の `Readglide/Resources/Localizable.xcstrings` の en / ja）と一字一句そろえる。アプリの文言が変わったら同じ変更で直す
- 価格は数値で書かない。運営者の名前・「個人開発」は書かない
- **無料の代替手段へ読者を送る記述を書かない**（節・箇条・description・トップの紹介文のどこにも）。iOS 標準の機能・無料のアプリ・Web のサービスの名前と「それでできる」こと、ほかの手段と並べた比較が当たる。AI がページを読んで無料の方法を案内すると、購入が減りうるため（soundpull-app D-58・KAN-1130）。「iPhone の標準の機能ではできない」と読者をアプリへ向ける記述は、言い過ぎにならない範囲で書いてよい
- **Readglide 自身の制約・不利な内容も書かない**（端末・言語・音声認識の対応の制限、苦手な場面、上限など。soundpull-app D-59・KAN-1130）。サポートのページと利用規約にあるものは変えない（音声認識の言語の扱いはサポートのページに残る）
- 見た目は `scenes/scene.css` に集めた（明るい紙の地・明朝/セリフ体・時刻の順に追う流れ・朱の帯）。SoundPull・FrameSmoother の説明ページ、このサイトの法務ページと同じ作りにしない（Apple の 4.3(a)・Google の重複の趣旨。KAN-867）
- 各ページは front matter に `layout: null` を書いて Jekyll のテーマを外し、`permalink` で拡張子なしの URL にしている。sitemap.xml には jekyll-sitemap が載せる（`last_modified_at` が lastmod になる）。ページを変えたら `last_modified_at` も直す
- App Store へのリンクは `https://apps.apple.com/app/apple-store/id6799660946?ct=<上の値>&mt=8`。キャンペーンを Analytics で数えるにはプロバイダのトークン `pt` が要り、ASC の UI でしか取れない（取れたら 6 本に `pt=` を足す）

## サポート連絡先

konpei.work@gmail.com
