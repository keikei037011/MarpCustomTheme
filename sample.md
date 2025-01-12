---
marp : true
theme : mytheme
paginate : true
---
<!--
class: title
footer: "共通フッター"
-->

<h1>Marp作成ガイド</h1>


<p>2025/01/01</p>
<p>Yamada Taro</p>



---
<!--
class: toc
-->

<div class="flex sa">
<div>

# 目次

1. [事前準備](#事前準備)
1. [MarkdownをMarpとして認識させる](#MarkdownをMarpとして認識させる)
1. [私がよく使う設定](#私がよく使う設定)
1. [自作CSS作成メモ](#自作CSS作成メモ)

</div>

---
<!--
class: content
_footer: "これは個別のフッタです"
-->

## サンプル1

- 要素1
    - スライド区切りは「---」を記載するだけ（簡単！）

- コードブロック

    ```
    {
    "markdown-preview-enhanced.hideDefaultVSCodeMarkdownPreviewButtons": false
    }
    ```

---
<!--
class: content
header: "事前準備"
-->

## サンプル2

- リンク表示
    1. [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)

---

## 表形式

| Name | Description |
|:-|:-|
| marp | marpの有効化 |
| theme	| テーマの指定(以後説明予定) |
| paginate | trueを指定した場合は、スライドにページ番号を表示 |
| header | ヘッダーの内容を指定 |
| footer | フッターの内容を指定 |

それ以外の設定は下記参照

https://marpit.marp.app/directives?id=local-directives-1

---
## 自作CSS作成メモ

1. mytheme.cssを./theme/mytheme.cssに格納
1. setting.jsonに以下を記載

```
"markdown.marp.themes": [
  "./theme/mytheme.css"
]
```

---
<!--
math: true
-->
## 引用ブロック

引用するときは、以下のように記載する

> 引用ブロックはこのように記載する

こんな感じですね

## インライン表示

- インライン表示は`XXX`で囲む


---
## 参考

- https://zenn.dev/kabec_dev/articles/9906c0b83d2ccb

https://manuhater.com/entry/marp-custom#f-

https://iroiroyaru.netlify.app/2021-05-14_marp/
https://marp-themes.nekast.com/entry/2024/03/23/195813

[【Marp】コピペで簡単！多段組みシンプルレイアウト](https://briboo-pc.hatenablog.jp/entry/2023/11/05/%E3%80%90Marp%E3%80%91%E3%82%B3%E3%83%94%E3%83%9A%E3%81%A7%E7%B0%A1%E5%8D%98%EF%BC%81%E5%A4%9A%E6%AE%B5%E7%B5%84%E3%81%BF%E3%82%B7%E3%83%B3%E3%83%97%E3%83%AB%E3%83%AC%E3%82%A4%E3%82%A2%E3%82%A6)

https://github.com/sindresorhus/github-markdown-css/blob/main/github-markdown.css

---