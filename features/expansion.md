---
icon: dot
tag: [その他]
author: 
- name: NoNICK
  avatar: https://media.discordapp.net/attachments/958791423161954445/975266759529623652/-3.png?width=663&height=663
order: 93
---
# メッセージURL展開
メッセージに含まれるメッセージURLを検知し、そのメッセージのコンテンツや添付ファイルを表示してくれる機能です。リンクを辿らなくてもメッセージの内容を素早く閲覧することができます。 <br>(開発・提供 `akki256.#0256`)

!!!success
この機能は、`/setting`→`🔗リンク展開機能`から、機能を有効に設定する必要があります。
!!!

![](/static/features/expansion_1.png)

また、添付ファイルが複数ある場合は左右のボタンを使用して、表示する項目を切り替えることができます。

![](/static/features/expansion_2.png)

!!!warning
**ボタンはメッセージURLの送信者のみが操作できます**。送信から一定時間が経ったり、BOTが再起動したりした場合でも、ボタンを操作することはできなくなります。<br>
(仕様上、「インタラクションに失敗しました」と表示されますが問題ありません。)
!!!