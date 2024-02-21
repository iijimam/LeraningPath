# InterSystems 製品で Python アプリケーションを記述する

> オリジナル：[Writing Python Applications with InterSystems](https://learning.intersystems.com/course/view.php?id=1943)

既存の Python コーディングスキルを活用して、InterSystems® アプリケーションを強化します。クライアントの Python アプリケーションを接続する方法、InterSystems ObjectScript コードに Python を組み込む方法、あるいは、Python ライブラリの呼び出しに重い処理が必要な場合に別のサーバを使用して呼び出しを最適化する方法について説明します。

![](/assets/WritingPythonAppWIthInterSystems.png)

0. [事前準備](#0-事前準備)
1. [はじめに](#1-はじめに)
2. [クライアントの Python アプリケーションから InterSystems IRIS への接続](#2-クライアントの-python-アプリケーションから-intersystems-iris-への接続)
3. [Python を ObjectScript と並行して実行する](#3-pythonをobjectscriptと並行して実行する)
4. [Python で InterSystems IRIS アプリケーションを構築する]

## 0. 事前準備
Pythonの基本的なコーディング経験があることを前提としています。

## 1. はじめに
インターシステムズのアプリケーションで Python ライブラリを活用する方法をご覧ください。pyodbc を使用して既存の Python アプリケーションを接続したり、Embedded Python を使用して Python と ObjectScript を並行してコーディングしたりできます。また、InterSystems Native API または外部言語サーバを使用して、Python による完全な InterSystems アプリケーションを構築することもできます。

- [Overview of Python in InterSystems Products (1m)](https://learning.intersystems.com/mod/page/view.php?id=11611)

## 2. クライアントの Python アプリケーションから InterSystems IRIS への接続

Python アプリケーションをインターシステムズ製品に接続するための最も一般的なオプションである pyodbc の使用方法について説明します。

- [ドキュメント:](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETODBC_support_pyodbc)

    参考として以下日本語ビデオどう？

    - [【はじめての InterSystems IRIS】セルフラーニングビデオ：アクセス編：Python から PyODBC を使って IRIS に接続してみよう](https://jp.community.intersystems.com/node/478616)

## 3. Python を ObjectScript と並行して実行する

Embedded Python を使用して、ObjectScript と並行して Python ライブラリを呼び出します。

- [ビデオ（英語／日本語字幕あり）:What Is Embedded Python?](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonOverview)

- [演習環境付き演習（ビデオは英語／日本語字幕あり）：Embedded Python QuickStart](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonQS)

- [オンラインラーニング（英語）：Parsing Images and Charting Data with Embedded Python](https://learning.intersystems.com/course/view.php?id=2126)

    同じじゃないけど、このコースをベースに作った記事

    -[Embedded Python を使ってレシート（JPG）の中身を IRIS に登録してみました](https://jp.community.intersystems.com/node/513136)

- [ドキュメント:デモ ： 組み込み Python の使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AFL_epython)

- [ドキュメント（英語）：Using Embedded Python](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GEPYTHON)

    このリンクは2023.1にはない。（情報増えてる？）


## 4. Python で InterSystems IRIS アプリケーションを構築する

また、InterSystems Python SDK を使用して、Python から InterSystems IRIS クラス・インスタンスをリモートで作成および操作できます。また、外部言語サーバを使用して、InterSystems 製品から外部プロセスで実行されている Python コードを呼び出す方法をご覧ください。

- [ビデオ（英語）:Using the Native API for Python](https://learning.intersystems.com/enrol/index.php?id=1110)

    以下日本語ビデオは？
    - [【はじめての InterSystems IRIS】セルフラーニングビデオ：アクセス編：Python の NativeAPI に挑戦](https://jp.community.intersystems.com/node/478611)

- [演習環境付き演習（英語／ビデオに日本語字幕あり）:Python QuickStart](https://learning.intersystems.com/enrol/index.php?id=1113)

    InterSystems IRIS® データ・プラットフォームは、リレーショナル・テーブルまたは多次元ストレージを介した InterSystems IRIS データベースへの直接アクセスを提供する 2 つの軽量な Python API をサポートしています：

    - PyODBC を使用すると、アプリケーションはデータを迅速に取得、更新、削除できます。
    - Python Native API を使用すると、アプリケーションは、ObjectScript のメソッドやルーチンを呼び出すだけでなく、InterSystems IRIS 内の基礎となるデータ構造 (グローバルとして知られている) に直接アクセスできます。
    
    ビデオでアプリケーションを InterSystems IRIS に接続する方法を確認し、以下の演習で PyODBC と Native API for Python を使用して InterSystems IRIS に接続してみてください。

- [ドキュメント:外部言語の操作](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BEXTSERV_coding)

- [演習環境付き演習（英語／ビデオに日本語字幕あり）Interacting with Data in Python Using Multiple Data Models](https://learning.intersystems.com/course/view.php?name=PythonMultiModel)
    
    InterSystems IRIS® データ・プラットフォームのマルチモデル・アーキテクチャをお試しください。InterSystems IRIS のマルチ・モデル・アクセスは、グローバルと呼ばれるデータ構造によって実現されています。これにより、データの重複を回避しながら、柔軟なデータ・アクセスが可能になります。

    Python では、Native API を使用して InterSystems IRIS に接続し、グローバルを使用してデータを操作できます。もう 1 つのオプションは、PyODBC で接続し、業界標準の SQL を使用してデータにアクセスする方法です。この場合、データはリレーショナル・テーブルとしてモデル化されます。