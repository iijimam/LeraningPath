# InterSystems ObjectScript入門
オリジナル：[Getting Started with InterSystems ObjectScript](https://learning.intersystems.com/course/view.php?id=289)
InterSystems ObjectScript の基本的な構文を学び、このプログラミング言語の主要な要素について紹介します。

**Credlyのバッジあり**

![](/assets/ObjectScript-LP.png)

1. [ObjectScript 入門](#1-objectscript-入門)
2. [コマンドと関数について](#2-コマンドと関数について)
3. [データタイプと変数について](#3-データタイプと変数について)
4. [クラス定義の作成](#4-クラス定義の作成)
5. [確認](#5-確認)


## 1. ObjectScript 入門
ObjectScriptの概要を読み、変数、式、コマンドなど、このプログラミング言語の主な機能のいくつかをインタラクティブなオンラインコースで学びます。

- [ドキュメント：ObjectScriptの概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_intro)

- [オンラインラーニング：InterSystems ObjectScript Basics（英語）](https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics)

    オンラインラーニングを通して以下の内容を学習できます。
    - InterSystems ObjectScript における変数の型付け方法
    - 変数の型に関する詳細情報をドキュメントから検索する方法
    - 変数の設定、変数の内容の確認、および変数のメモリからの削除を行うための set、write、kill の使用方法
    - 算術演算と組み込み関数を使用して変数を操作する
    - 論理演算子を使用して変数を比較する
    - if/else 文を評価する。
    - do を使ってメソッドを実行する
    - ループを使用する

    《上記内容をカバーできる日本語コンテンツ》
    - [ObjectScriptクックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)


## 2. コマンドと関数について
演算子と式を詳しく見てみましょう。システム関数を使用して操作を素早く実行する方法を学び、コマンドで後置条件式を使用する方法を確認します。

- [ドキュメント：演算子と式](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_operators)

- [ビデオ：Using System Functions in ObjectScript（英語）](https://learning.intersystems.com/course/view.php?name=OSFunctions)

- [ビデオ：Controlling Command Flow with Postconditional Expressions（英語）](https://learning.intersystems.com/course/view.php?id=2131)
   
    If 文を使用せずに単一のコマンドに条件を追加する方法を説明しています。
    InterSystems ObjectScript では、ほとんどの単一行コマンドの後ろに高知条件を追加することで、コマンド・フローを制御できます。これらの式は、コマンドが実行されるべきかどうかを決定します。

《上記内容をカバーできる日本語コンテンツ》
- [ObjectScriptクックブック：演算子](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%BC%94%E7%AE%97%E5%AD%90)

※後置条件はクックブックにない。関数はCookBook.mdにいくつかある

## 3. データタイプと変数について
ObjectScript でよく使用されるデータ型や、さまざまなカテゴリの変数とその使用方法について学びましょう。

- [ビデオ：Exploring Data Types in ObjectScrip（英語）](https://learning.intersystems.com/course/view.php?name=ObjectScriptDataTypes)

- [ドキュメント：多次元配列](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_mdarrays)

- [ビデオ：Using Variables in ObjectScript（英語）](https://learning.intersystems.com/course/view.php?id=2133)

《上記内容をカバーできる日本語コンテンツ（[ObjectScriptクックブック](https://github.com/Intersystems-jp/ObjectScriptCookBook/)）》
- [ObjectScriptの基本のき！：変数](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#3-%E5%A4%89%E6%95%B0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)

- [注意点](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%B3%A8%E6%84%8F%E7%82%B9)

- [現在日付と時刻の取得](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E7%8F%BE%E5%9C%A8%E6%97%A5%E4%BB%98%E3%81%A8%E6%99%82%E5%88%BB%E3%81%AE%E5%8F%96%E5%BE%97)

- [リスト](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E3%83%AA%E3%82%B9%E3%83%88)



## 4. クラス定義の作成
ObjectScript の基本を学んだところで、Visual Studio Code で最初のクラス定義を作成します。

- [オンラインラーニング:Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)


以下動画から、クラス定義の作成からインスタンス生成、保存までの流れを確認できます。
- [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）](https://jp.community.intersystems.com/node/478606)


## 5. 確認