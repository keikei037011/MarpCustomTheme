# MarpCustomTheme

Marpのカスタムテーマを作成するためのリポジトリ

## 前提

VScodeに以下の設定がされていること

1. Vscodeの拡張機能として[Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)がインストールされていること

1. Markdown Preview Enhancedを入れている方は以下の設定を実施していること
  
    ```json:setting.json
    {
    "markdown-preview-enhanced.hideDefaultVSCodeMarkdownPreviewButtons": false
    }
    ```

1. MarkdownでHTMLタグを使えるように下記を設定しておくこと

    ``` json:setting.json
    {
    "markdown.marp.enableHtml": true
    }
    ```

## カスタムテーマの適用方法

1. mytheme.cssを./theme/mytheme.cssに格納
1. setting.jsonに以下を記載
    ```
    "markdown.marp.themes": [
    "./theme/mytheme.css"
    ]
    ```