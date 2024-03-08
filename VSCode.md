# VS Codeを使用したInterSystemsサーバサイドの開発

> オリジナル[Developing on an InterSystems Server Using VS Code](https://learning.intersystems.com/enrol/index.php?id=1678)

**Credlyある**

VS Code を使用した InterSystems® 製品の開発方法をご紹介します。複数の InterSystems サーバでの作業、クライアントサイドまたはサーバサイドでのクラス編集、InterSystems 端末へのアクセスなどをご覧ください。

![](/assets/VSCode.png)

1. [VSCodeのインストールと設定](#1-vscodeのインストールと設定)
2. [ワークスペースの設定](#2-ワークスペースの設定)
3. [InterSystems Serverで開発する](#3-intersystems-serverで開発する)]
4. [あなたの知識の評価](#4-あなたの知識の評価)

## 1. VSCodeのインストールと設定

- [ドキュメント（英語）：Installation](https://docs.intersystems.com/components/csp/docbook/DocBook.UI.Page.cls?KEY=GVSCO_install)

- [ビデオ（英語）：Install and Use ObjectScript Extensions for VS Code](https://learning.intersystems.com/enrol/index.php?id=1458)

    《２つのビデオの代用として以下使えるかも》
    - [記事：VSCodeを使ってみよう](https://jp.community.intersystems.com/node/482976)

- [オンラインコース（英語）:Installing VS Code and Configuring InterSystems Server Connections](https://learning.intersystems.com/course/view.php?id=1782)

    Visual Studio Code で最新の InterSystems 拡張機能を検索します。VS Code を使用して、InterSystems サーバに接続し、クライアントサイドおよびサーバサイドのソースコードを編集できます。

    （演習環境なしでコンテナ　containers.intersystems.com/intersystems/iris-community:latest-em　使ってる）

## 2. ワークスペースの設定

- [ドキュメント（英語）:Configure the InterSystems VS Code Extensions](https://docs.intersystems.com/components/csp/docbook/DocBook.UI.Page.cls?KEY=GVSCO_config)

    《代用として以下使えるかも》
    - [記事：VSCodeを使ってみよう:2、サーバへ接続する ](https://jp.community.intersystems.com/node/482976#2)

- [ビデオ（英語）:Configuring VS Code Workspaces for Multiple ObjectScript Connections](https://learning.intersystems.com/enrol/index.php?id=1783) 
    InterSystems ObjectScript Extension Pack を使用して VS Code を構成し、複数のサーバ接続をサポートする方法を説明します。ワークスペース構成の基本を確認し、システムに必要な構成を決定してから、シングルフォルダおよびマルチルートのワークスペースに関する手順に従ってください。

    このビデオでは、2 つの構成を紹介します：

    マルチルートのワークスペースと仮想フォルダを使用して、複数の InterSystems IRIS® データプラットフォームのネームスペースまたはサーバにまたがってコードを表示し、サーバ側で編集を行います。
    複数の VS Code ワークスペース（それぞれ固有のアクティブな接続を持つ）を使用して、複数のネームスペースまたはサーバーのコードを表示し、クライアント側でコードを編集します。また、単一フォルダのワークスペースでサーバー側の編集を有効にすることもできます。

    **日本語のビデオ作るか字幕付けたらいいかと思う**

    >ユーザ／ワークスペース／フォルダ単位のどの設定になるのかを説明しててわかりやすい。（サーバ側編集のIRISが多い環境だとマルチルートワークスペース使うと１VSCodeで作業できて便利。シングルフォルダワークスペースはクライアント側で編集＋同期の開発をしたい場合に最適）


## 3. InterSystems Serverで開発する

- [ビデオ（英語）：Working with InterSystems Classes in VS Code](https://learning.intersystems.com/course/view.php?id=1778)

    《代用として以下使えるかも》
    - [記事：VSCodeを使ってみよう:3、クラス定義を作ってみる](https://jp.community.intersystems.com/node/482976#3)

- [オンラインコース（英語）:Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)

    クラス定義の構造と基本構文、および VS Code での InterSystems クラス定義の開発方法を学習します。また、プロパティ、パラメータ、メソッドなどのクラス・メンバの定義方法についても学習します。

    このコースには、4 つの指導レッスンといくつかのクイズ問題が含まれています。ビデオはフルスクリーンモードで見るのが最適です。

- [コミュニティ：Accessing the IRIS Terminal: A Comprehensive Guide for Visual Studio Code Users](https://community.intersystems.com/post/accessing-iris-terminal-comprehensive-guide-visual-studio-code-users)
 
    翻訳したらいいかも

- [ビデオ（英語）:VS Code Debugger for InterSystems ObjectScript](https://learning.intersystems.com/course/view.php?id=1795)

    デバッガの仕組みを話してる。字幕付けてもいいかも

    《代用として以下使えるかも》
    - [記事：VSCodeを使ってみよう:5、デバッグの実行](https://jp.community.intersystems.com/node/482976#5)

    - [記事：VSCode：プロセスにアタッチしてデバッグする方法](https://jp.community.intersystems.com/node/489221)

## 4. あなたの知識の評価