# .well-known

GitHub Pages（Jekyll）で [Well-Known URI](https://www.rfc-editor.org/rfc/rfc8615) リソースを公開するためのリポジトリです。

## 含まれるファイル

- **`apple-app-site-association`** — iOS の Associated Domains / Universal Links 用（JSON）
- **`clip/<screen-id>/index.html`** — App Clip / Universal Link 用のフォールバック（Jekyll の `layout: clip_landing` と YAML の `clip_screen_id` で生成）

`clip/...` を増やすときは、[my-toybox の `ClipScreenCatalog.availableRoutes`](https://github.com/Koshimizu-Takehito/my-toybox/blob/main/Packages/Sources/MyToyboxScreens/ClipScreenCatalog.swift) に追加した `Screen.rawValue` と同じディレクトリ名で `index.html` を置き、既存ページと同様の Front Matter を付けること。

ビルド設定は [`_config.yml`](_config.yml)（`jekyll-theme-midnight`）を参照してください。

### App Store（ランディング・Smart App Banner）

サイト上の **「App Store で見る」** と Safari の **Smart App Banner** に使う数値 ID は、[App Store Connect](https://appstoreconnect.apple.com/) → 対象アプリ → **App 情報** に表示される **Apple ID**（10 桁前後の数字）です。取得後、`_config.yml` の `mytoybox.app_store_id` に文字列で設定してください（例: `"1234567890"`）。

空のままでは、バナー・主ボタンは出ず、プレースホルダ文言のみ表示されます。

## ライセンス

[MIT License](LICENSE)
