---
icon: diff-ignored
order: 45
---

# /bulkdelete
!!!success
このコマンドを使用するには、`メッセージの管理`権限を保有している必要があります。
!!!

## 概要
コマンドを実行したチャンネルのメッセージを、新しい順に指定した数だけ削除します。
複数のメッセージをすばやく削除することができるため、スパムの削除等に役立ちます。

![](/static/features/bulkdelete/1.png)

!!!warning
DiscordAPIの仕様上、このコマンドでは**2週間前に投稿したメッセージ**を削除することはできません。
また、このコマンドでは一度に**100件**までメッセージを削除することができます。
!!!

## 引数

引数       | 説明
:---       | :---:
`messages` | 削除するメッセージの数 (`2`～`100`まで)