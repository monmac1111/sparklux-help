# sparklux-help

[Sparklux](https://apps.apple.com/) — macOS 用 HDR 動画プレイヤーの**ヘルプとプライバシーポリシー**。

公開先: **https://monmac1111.github.io/sparklux-help/**

| | URL |
|---|---|
| ヘルプ（日本語）| https://monmac1111.github.io/sparklux-help/ja/help/ |
| プライバシーポリシー（日本語）| https://monmac1111.github.io/sparklux-help/ja/privacy/ |
| Help (English) | https://monmac1111.github.io/sparklux-help/en/help/ |
| Privacy Policy (English) | https://monmac1111.github.io/sparklux-help/en/privacy/ |

App Store Connect の **サポート URL** と **プライバシーポリシー URL** にこれらを登録する。

## 直し方

`docs/` の Markdown を直して push すれば、GitHub Actions が組んで配信する。

⚠️ **HTML はコミットしない。**写しは必ず片方が腐る。ビルドは CI に任せる。
⚠️ `mkdocs build --strict` なので、**リンク切れがあるとビルドが落ちる**。

## 手元で見る

```bash
pip install mkdocs-material && mkdocs serve
```
