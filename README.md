# .well-known

GitHub Pages（Jekyll）で [Well-Known URI](https://www.rfc-editor.org/rfc/rfc8615) リソースを公開するためのリポジトリです。

## 含まれるファイル

- **`apple-app-site-association`** — iOS の Associated Domains / Universal Links 用（JSON）。App Clip 向けパスは **`/my-toybox-clip/*`**（[my-toybox-clip](https://github.com/Koshimizu-Takehito/my-toybox-clip) プロジェクトサイト）に一致。

App Clip / Universal Link 用の**ランディングページ**（`/<screen-id>/`、Smart App Banner 等）は **[my-toybox-clip](https://github.com/Koshimizu-Takehito/my-toybox-clip)** リポジトリで管理します。新規デモはそちらに `index.html` を追加し、[my-toybox の `ClipScreenCatalog`](https://github.com/Koshimizu-Takehito/my-toybox/blob/main/Packages/Sources/MyToyboxScreens/ClipScreenCatalog.swift) と `Screen.rawValue` を同期してください。

ビルド設定は [`_config.yml`](_config.yml)（`jekyll-theme-midnight`）を参照してください。

### App Store（このリポの `index` の Smart App Banner）

ルート [`index.html`](index.html) のバナー用 **Apple ID** は `_config.yml` の `mytoybox.app_store_id` です（[App Store Connect](https://appstoreconnect.apple.com/) → アプリ → **App 情報**）。

## ライセンス

[MIT License](LICENSE)
