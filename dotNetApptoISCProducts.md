# .NETアプリケーションとInterSystems製品の接続
> オリジナルラーニングページ：[Connecting .NET Applications to InterSystems Products](https://learning.intersystems.com/course/view.php?id=968)

ADO.NET、XEP、Entity Framework、または Native API（Native SDK for .NET） を使用して、.NET アプリケーションを InterSystems IRIS® データプラットフォームやその他のインターシステムズ製品およびテクノロジに接続する方法をご説明します。

（他の言語からの接続については、別のラーニングパスがあります。《ここにリンク》）


![](/assets/dotNetAppToISCProducts.png)

1. [このラーニングパスの内容](#1-このラーニングパスの内容)
2. [ADO.NETを使用したリレーショナルテーブルへアクセスする方法](#2-adonetを使用したリレーショナルテーブルへアクセスする方法)
3. [高いスループットのデータインジェスチョンのためのXEP使用方法](#3-高いスループットのデータインジェスチョンのためのxep使用方法)
4. [Native API（Native SDK for .NET）でのデータアクセス](#4-native-apinative-sdk-for-netでのデータアクセス)
5. [Entity Frameworkを使用してデータベースと.NETオブジェクトとのマッピング]()
6. [.NETの接続](#6-netの接続)
7. [Object Gatewayを使用してInterSystems IRISから.NETのコードを実行する](#7-object-gatewayを使用してintersystems-irisからnetのコードを実行する)





## 1. このラーニングパスの内容
各 API の利点を確認し、.NET アプリケーションをインターシステムズ製品に接続するための手段を確認します。

- [.NET 概要（日本語字幕ありのビデオがリンク先）：5分](https://learning.intersystems.com/course/view.php?id=1059)

- [Designing a .NET Connection Strategy（オンラインラーニング：英語）：30分](https://learning.intersystems.com/course/view.php?name=.NET%20Connection%20Strategy)

メモ：対応する説明資料あるけどコースにしてない（C#.NET/VB.NET）

## 2. ADO.NETを使用したリレーショナルテーブルへアクセスする方法

Visual Studio プロジェクトで InterSystems ADO.NET マネージド・プロバイダを使用して、データに簡単にリレーショナル・アクセスできます。

詳細は、以下ドキュメントをご参照ください。

[機能紹介：ADO.NETとインターシステムズ製品](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AFL_adonet)

## 3. 高いスループットのデータインジェスチョンのためのXEP使用方法

XEP を使用して、高性能でリアルタイムのオブジェクトを迅速に格納できます。

- [ビデオ：Using XEP with .NET(8m)](https://learning.intersystems.com/course/view.php?name=Using%20XEP%20with%20.NET)

    日本語字幕を選択できます。

- [ドキュメント：InterSystems XEPによる.NETオブジェクトの永続化](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETXEP)

## 4. Native API（Native SDK for .NET）でのデータアクセス
Native API を使用してIRISのグローバル変数にデータを格納したり、InterSystems IRIS のメソッドまたはルーチンを呼び出します。

- [ビデオ：Using the Native API for .NET](https://learning.intersystems.com/course/view.php?name=Native%20API%20for%20.NET)

    日本語字幕を選択できます。

- [ドキュメント：Native SDK for .NET の概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETNAT_about)

- [コミュニティ：Native SDK (NativeAPI) for .NET を使用する簡単なサンプルのご紹介](https://jp.community.intersystems.com/node/559276)

## 5. Entity Frameworkを使用してデータベースと.NETオブジェクトとのマッピング
Entity Framework Providerの使用方法を確認し、Code FirstアプローチとDatabase Firstアプローチの使用方法を学びます。

- [ドキュメント：Entity Framework Provider の使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNET_eframe)

- [ビデオ：Using Entity Framework with InterSystems IRIS Data Platform](https://learning.intersystems.com/course/view.php?name=Entity%20Framework)

    日本語字幕を選択できます。

## 6. .NETの接続
各接続方法の利点を確認するため、実際に練習してみよう。

[オンラインコース：Stock Trading with .NET（英語）](https://learning.intersystems.com/course/view.php?name=.NET%20Financial%20Play)

## 7. Object Gatewayを使用してInterSystems IRISから.NETのコードを実行する

.NET ゲートウェイを使用して、InterSystems ObjectScript を使用して .NET オブジェクトをどのように操作できるかを実際に操作して確認してください。

[ドキュメント：外部言語動作](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BEXTSERV_coding)
