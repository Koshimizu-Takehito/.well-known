# .well-known

GitHub Pages（Jekyll）で [Well-Known URI](https://www.rfc-editor.org/rfc/rfc8615) リソースを公開するためのリポジトリです。

## 含まれるファイル

- **`apple-app-site-association`** — iOS の Associated Domains / Universal Links 用（JSON）
- **`clip/<screen-id>/index.html`** — App Clip / Universal Link 用 URL のフォールバック表示（静的 HTML）

`clip/...` のページを増やすときは、[my-toybox の `ClipScreenCatalog.availableRoutes`](https://github.com/Koshimizu-Takehito/my-toybox/blob/main/Packages/Sources/MyToyboxScreens/ClipScreenCatalog.swift) に追加した `Screen.rawValue` と同じパス名で置くこと。

ビルド設定は [`_config.yml`](_config.yml)（`jekyll-theme-midnight`）を参照してください。

## ライセンス

[MIT License](LICENSE)
