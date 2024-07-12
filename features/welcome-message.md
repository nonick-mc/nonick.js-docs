---
icon: dot
order: 100
---

# 入退室メッセージ
## 概要
サーバーにメンバーやBOTが参加したり脱退した際に、メッセージを送信する機能です。  
送信するメッセージは設定で変更することができ、参加した人に見てもらいたい情報を送信することもできます。

![](/static/features/welcome-message/1.png)

BOTが入退室した際は、通常と違う特別な埋め込みが送信されます。

![](/static/features/welcome-message/2.png)

## 設定
+++ 入室メッセージ
> メンバーがサーバーに参加した際にメッセージを送信します。

- [x] **有効化・無効化**  
入室メッセージの状態を切り替えます。

- [x] **送信先**  
メッセージを送信するチャンネルを変更します。 (テキストチャンネルである必要があります)  

- [x] **メッセージ**  
メッセージの内容を変更します。[構文](#構文)を使用できます。

- [x] **プレビュー**  
現在の入室メッセージを表示します。

+++ 退室メッセージ
> メンバーがサーバーから脱退した際にメッセージを送信します。

- [x] **有効化・無効化**  
退室メッセージの状態を切り替えます。

- [x] **送信先**  
メッセージを送信するチャンネルを変更します。 (テキストチャンネルである必要があります)  

- [x] **メッセージ**  
メッセージの内容を変更します。[構文](#構文)を使用できます。

- [x] **プレビュー**  
現在の退室メッセージを表示します。
+++

### 構文
各設定の**メッセージ**では、特別な構文を使用してメッセージを動的に作成することができます。  
サーバーの名前やメンバー数は、入退室が発生した際の状態を参照します。

構文 | 説明 | 例
--- | --- | ---
`![serverName]` | サーバーの名前 | NoNICK SERVER
`![memberCount]` | サーバーに参加しているメンバーの人数  | 1200
`![user]` | 入室・退室したメンバーのメンション | @nonick-mc
`![userName]` | 入室・退室したメンバーの名前 | nonick-mc
`![userTag]` [!badge variant="danger" text="非推奨"] | 入室・退室したメンバーの名前 (タグも含む) | nonick-mc#1017