---
icon: diff-ignored
order: 48
---

# /embed (拡張)
!!!success
このコンテキストメニューを使用するには、`メッセージの管理`権限を保有している必要があります。
また、[ロール付与コンポーネント](#ロール付与セレクトメニューを追加)の作成を行うためには`ロールを管理`権限を保有している必要があります。
!!!

## 概要
[/embed](/features/embed.md)コマンドで送信した埋め込みを右クリックして、`アプリ`から`埋め込みを編集`を使用すると、埋め込み編集したり、ロール付与ボタンなどのコンポーネントを追加することができます！表示されたメッセージのセレクトメニューから、その埋め込みに対して行う操作を変更できます。

![](/static/features/embed/9.png)

!!!danger
Discordの仕様上、NoNICK.jsをサーバーからKickすると、Kickする前に送信した埋め込みは**再度導入しても編集できなくなります。**
NoNICK.jsを一時的にKickする場合は、埋め込みをダウンロードする等してバックアップを行うことをおすすめします。
!!!

## 埋め込みを編集
埋め込みの編集を行うことができます。編集できる項目および編集の仕方は、[カスタマイズ](/features/embed.md/#カスタマイズ)と同様です。

![](/static/features/embed/11.png)

## ロール付与(セレクトメニュー)を追加
項目の中から付与するロールを自由に選択できるセレクトメニューを追加します。
セレクトメニューはメッセージ1つにつき5個まで追加することができます。

![](/static/features/embed/10.png)

!!!warning
`ロール付与(ボタン)`または`URLボタン`と一緒に追加することはできません。  
!!!

### ① ロール追加・削除
セレクトメニューにロールを追加および削除します。ロールは最大で25個まで追加できます。

追加する際のモーダルの項目                                 | 説明
:---                                                       | :---:
ロールの名前またはID [!badge variant="danger" text="必須"] | -
セレクトメニュー上での表示名                               | - (省略した場合はロール名が使用されます)
ロールについての説明                                       | 説明は項目の下に表示されます
Unicode絵文字 または カスタム絵文字                        | 実行したサーバーのカスタム絵文字の名前かID<br>またはUnicode絵文字(一文字)

### ② プレースホルダー設定
未選択状態の際に表示されるテキスト(プレースホルダー)を設定します。

モーダルの項目       | 説明
:---                 | :---:
セレクトメニューのプレースホルダー | - (未記入の場合は初期値が使用されます)

### ③ 選択モード切り替え
項目の最大選択数を2種類から切り替えます。

モード             | 説明
:---               | :---:
選択モード: 単一   | 選択できる項目は一つのみになります。
選択モード: 複数   | 全ての項目を選択できるようになります。

### ④ セレクトメニューを追加
設定したセレクトメニューを追加します。

## ロール付与(ボタン)を追加
クリックするとロールを付けたり外したりすることができるロール付与ボタンを追加します。
ボタンはURLボタンも含め、メッセージ1つにつき25個まで追加することができます。

![](/static/features/embed/12.png)

!!!warning
`ロール付与(セレクトメニュー)`と一緒に追加することはできません。  
!!!

### ① ボタンを作成・追加
メッセージにボタンを追加します。ボタンの色は[色の変更](#-色の変更)ボタンの色が使用されます。

モーダルの項目                                 | 説明
:---                                                       | :---:
ロールの名前またはID [!badge variant="danger" text="必須"] | -
ボタン上での表示名                                         | - (省略した場合はロール名が使用されます)
Unicode絵文字 または カスタム絵文字                        | 実行したサーバーのカスタム絵文字の名前かID<br>またはUnicode絵文字(一文字)

!!!
`ボタン上での表示名`を空欄にして`Unicode絵文字 または カスタム絵文字`で絵文字を指定すると、絵文字のみのボタンを追加することができます。
!!!

### ② 色の変更
追加するボタンの色を変更します。
色は`Primary(青)`、`Success(緑)`、`Danger(赤)`、`Secondary(灰)`の4種類から切り替えることができます。

## URLボタンを追加
クリックすると特定のURLに移動させることができるURLボタンを追加します。
ボタンはロール付与ボタンも含め、メッセージ1つにつき25個まで追加することができます。

![](/static/features/embed/13.png)

!!!warning
`ロール付与(セレクトメニュー)`と一緒に追加することはできません。  
!!!

モーダルの項目                            | 説明
:---                                      | :---:
URL [!badge variant="danger" text="必須"] | -
ボタンのテキスト                          | -
Unicode絵文字 または カスタム絵文字       | 実行したサーバーのカスタム絵文字の名前かID<br>またはUnicode絵文字(一文字)

!!!
`ボタンのテキスト`を空欄にして`Unicode絵文字 または カスタム絵文字`で絵文字を指定すると、絵文字のみのURLボタンを追加することができます。
!!!

## コンポーネントを削除
メッセージに既に追加されているコンポーネントを削除することができます。
セレクトメニューからはコンポーネントを**一行単位**で、「全てのコンポーネントを削除」ボタンで全てのコンポーネントを削除します。
 
![](/static/features/embed/14.png)