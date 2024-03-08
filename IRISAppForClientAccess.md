# クライアントアクセスのための InterSystems IRIS を利用したアプリケーションの構成

オリジナル：[Configuring InterSystems IRIS Applications for Client Access](https://learning.intersystems.com/course/view.php?id=1975)

> 自分メモ：【IRISを利用したWebアプリケーションの構成】　ってしたほうがわかりやすくないか？

InterSystems IRIS® データ・プラットフォーム・アプリケーションを Web アプリケーションのバックエンドとして機能させるためのセットアップ方法をご紹介します。

REST経由でアクセスする InterSystems IRIS アプリケーションを外部システムやユーザからデータにアクセスできるようにする方法と、データ交換の簡単に行うためにアプリケーションでJSONデータの入力／生成を行う方法を学習します。

Webアプリケーションのバックエンドとして InterSystems IRIS を使用する知識を前提とし、オブジェクトと SQL の使用経験が必要です。必要に応じて、[「InterSystems を使用したサーバサイド・アプリケーションの構築」ラーニング・パス (5h) ](https://learning.intersystems.com/course/view.php?id=2369)をご覧ください。


    【自分メモ】オンラインコースに含まれる内容  
    アーキテクチャ（NS／DB、マッピングも含まれてた）
    VSCodeを使ってクラス定義作成とデータ作成まで
    ObjectScriptの基本
    SQLの基本
    複数のクラスを使ったアプリの処理に合わせた定義練習（データ作成＋メソッド作成）

上記オンライン（[「InterSystems を使用したサーバサイド・アプリケーションの構築」ラーニング・パス (5h) ](https://learning.intersystems.com/course/view.php?id=2369)）の代わりなるものは以下

- [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)
- [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）](https://jp.community.intersystems.com/node/478606)
- [ObjectScript クックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)

- [InterSystems Objectのトレーニングコース（２日間）](https://www.intersystems.com/jp/intersystems-object/)
---



![](/assets/IRISAppForClientAccess.png)


1. [RESTサーバのセットアップ](#1-restサーバのセットアップ)
2. [JSONデータの入力と生成](#2-jsonデータの入力と生成)
3. [APIの管理](#3-apiの管理)

## 1. RESTサーバのセットアップ
InterSystems IRIS で RESTful サービスをセットアップして、Web アプリケーションなどの外部システムからIRIS内のデータにアクセスできるようにする方法を説明します。

### USオリジナルがさしてるページ

Experience　https://learning.intersystems.com/course/view.php?id=2158

オンラインコース　https://learning.intersystems.com/course/view.php?name=REST%20Services

オンラインコースはIRISのRESTサーバの動作の仕組みからExperienceのAngularアプリの説明をしてる＋ビジネスサービスにREST呼び出しをする方法も含まれてる

    《自分メモ》：フロントのWebアプリ付きの体験なら以下がいい（でも説明がない。あるけど2019のDoc）
    リポジトリ　https://github.com/intersystems/FirstLook-REST

    日本語Docだとここ　https://docs.intersystems.com/iris20191/csp/docbookj/Doc.View.cls?KEY=AFL_rest
    （新バージョンだとないからコミュニティに手順書いて公開するのもいいかも）

### セルフラーニング
> 自分メモ：フロントのWebアプリはないけどけど以下ビデオはどうだろう

- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS で作成する REST サーバの仕組み](https://jp.community.intersystems.com/node/479546)

    IRIS で作成する RESTサーバの仕組みを解説します。

- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）手動で作成するディスパッチクラス](https://jp.community.intersystems.com/node/479551)

    RESTサーバに必要なディスパッチクラスを手動で用意する方法を解説します。


- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    RESTサーバに必要なREST ディスパッチクラスを API ファーストの手順で作成する方法を解説します。（OpenAPI 2.0に基づいて作成したアプリケーション定義を使用してディスパッチクラスを作成する手順を解説します）

- [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)


### 講師付きトレーニング

- RESTサーバの作成（1日）
- ObjectScript の使い方（1 日）



## 2. JSONデータの入力と生成

> USがさしてるページ：https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS

セルフラーニングビデオならある
[【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS での JSON の操作](https://jp.community.intersystems.com/node/480106)


## 3. APIの管理

> USがさしてる概要ページ　https://learning.intersystems.com/course/view.php?name=What%20is%20IAM　　＋　オンラインコース　https://learning.intersystems.com/course/view.php?id=1747

    IAM概要とハンズオンがあるといい
    概要説明ページに翻訳つけるだけでもいいかも？？

コミュニティのページを指すのはどうか？

- [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)