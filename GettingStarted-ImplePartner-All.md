# インプリメンテーションパートナ向けInterSystems製品をはじめよう（全業種向け）

このラーニング・パスでは、InterSystems® の概要、InterSystems 製品とテクノロジのアーキテクチャと機能について説明します。このパスに従うことで、コードの記述、システム統合を構築し、アプリケーションに必要なコンポーネントを作成することを学習できます。

パートナーになることに興味がありますか？[インプリメンテーション・パートナー・プログラムの詳細](https://www.intersystems.com/jp/partners/implementation-partners/)をご覧ください。医療と金融のパートナーは、[インプリメンテーション・パートナー（医療）](https://learning.intersystems.com/course/view.php?id=1809) および[インプリメンテーション・パートナー（金融サービス）](https://learning.intersystems.com/mod/url/view.php?id=10341)のラーニング・パスで業界固有のコンテンツを見つけることができます。

>オリジナル[Getting Started with InterSystems for Implementation Partners (All Industries)
Note](https://learning.intersystems.com/course/view.php?id=1809)

![](/assets/GettingStartedWithImplePartner-All.png)

このラーニング・パスを終了することに加え、以下の講師付きクラスルームトレーニングコースに参加／個別開催の申し込みを行うことを強く推奨します。

[InterSystems Server システム管理1](https://www.intersystems.com/jp/intersystems-server-system-administration/)／[InterSystems Server システム管理2：セキュリティ管理編](https://www.intersystems.com/jp/intersystems-server-system-administration-2/) (合計6日間)


1. [InterSystems IRIS とは？](#1-intersystems-iris-とは)
2. [アプリケーションの構築](#2-アプリケーションの構築)
3. [他のシステムとの統合](#3-他のシステムとの統合)
4. [カスタムコンポーネントを使用したシステム統合の開発](#4-カスタムコンポーネントを使用したシステム統合の開発)
5. [他言語を使用したデータアクセス](#5-他言語を使用したデータアクセス)
6. [APIの管理](#6-apiの管理)
7. [既存システムからの移行](#7-既存システムからの移行)
8. [リアルタイム分析の構築](#8-リアルタイム分析の構築)
9. [機械学習の適用](#9-機械学習の適用)
10. [レポートの実行](#10-レポートの実行)
11. [パフォーマンスとスピードの最適化](#11-パフォーマンスとスピードの最適化)

## 1. InterSystems IRIS とは？

InterSystems IRIS®データ・プラットフォームは、信頼性の高い統一プラットフォームで、重要なアプリケーションを迅速に開発・配布することを可能にします。

- データ管理
- Interoperability（相互運用性）
- トランザクション処理
- 分析

[ビデオ（英語）InterSystems へようこそ](https://www.youtube.com/watch?v=v4uoejre5IU)

↑こんなビデオ日本でも作ったらいいのに

[ビデオ（英語／日本語字幕あり）What Is InterSystems IRIS?](https://learning.intersystems.com/course/view.php?id=2118)

## 2. アプリケーションの構築

InterSystems IRIS で ObjectScript を使用して高性能なアプリケーションを構築する方法を学習することで以下の内容を開発できるようになります。

- ビジネスルールとメッセージルータのコードでカスタム関数を作成する。
- カスタムコードによる高度なデータ変換の作成
- カスタム・プロダクション・コンポーネントの構築
カスタム・ビジネス・コンポーネントの構築方法の詳細については[「カスタムコンポーネントを使用したシステム統合の開発」](#4-カスタムコンポーネントを使用したシステム統合の開発)をご参照ください。

### オリジナル

- [ビデオ（英語）InterSystems Architecture Overview](https://learning.intersystems.com/course/view.php?name=Architecture%20Overview)

- [オンラインラーニング（英語）：Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)

- [オンラインラーニング（英語）:InterSystems ObjectScript Basics](https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics)

- [オンラインラーニング（英語）:InterSystems IRIS Objects Introduction](https://learning.intersystems.com/enrol/index.php?id=2225)

- [オンラインラーニング（英語）：InterSystems SQL Overview](https://learning.intersystems.com/enrol/index.php?id=960)

- [オンラインラーニング（英語）:Using JSON in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS)

- [演習環境付き演習：Learning Path Exercise: Building a Server-Side Application with InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Server-Side%20Application%20Exercise)

    InterSystems IRIS® データプラットフォームと InterSystems ObjectScript を使用して、小規模なデータベースアプリケーションを作成します。この演習では、InterSystems IRIS を使用したサーバサイド・アプリケーションの構築の学習パスで学習したすべてのスキルを結集して、大規模な書籍コレクションに関する情報を格納および取得するためのクラスを作成し、SQL を使用します。この演習は、既存の知識をテストするために学習パスを開始する前に、またはキャップストーン・プロジェクトとして最後にお試しください。

### 対応できそうな日本語コンテンツ

以下動画から、IRISの開発環境の作成方法、ネームスペース／データベースについて、IDEからIRISに接続する方法を確認できます。
- [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

以下コンテンツから、ObjectScriptの基本操作を確認できます。
- [ObjectScript クックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)

以下動画から、クラス定義の作成からインスタンス生成、保存までの流れを確認できます。
- [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）](https://jp.community.intersystems.com/node/478606)


InterSystems製品でのJSON操作については、以下記事をご参照ください。
-[【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS での JSON の操作](https://jp.community.intersystems.com/node/480106)


メソッド内でSQLを記述する方法については、以下のコンテンツをご参照ください。

- [ObjectScriptクックブック：7.メソッドやルーチンでSQLを実行する方法](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#7-%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%84%E3%83%AB%E3%83%BC%E3%83%81%E3%83%B3%E3%81%A7sql%E3%82%92%E5%AE%9F%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95)

トレーニングコースもご用意しています。
- [InterSystems Objectのトレーニングコース（２日間）](https://www.intersystems.com/jp/intersystems-object/)


### 認定テスト受験の準備が整ったら

インターシステムズ・ラーニング・サービスは、業界標準の認定試験を提供し、あなたがインターシステムズの技術を習得していることを証明します。当社の試験は、安全なオンライン試験監督とセルフサービス予約で提供されます。受験者は、いつでもどこでも、都合のよいときに試験を受けることができます。

※英語

[Exam: InterSystems IRIS Core Solutions Developer Specialist](https://www.intersystems.com/education/)

## 3. 他のシステムとの統合

多くの場合、データはフラット・ファイルかカスタム・フォーマットのどちらか送受信されます。このセクションでは、このようなデータを素早く取り込むことができる、ローコードまたはコード不要のユーティリティを紹介します。

- [体験環境付き演習：Receiving and Routing Data in a Production](https://learning.intersystems.com/course/view.php?name=Interop%20QS)

    この中のビデオは日本語字幕あり。この演習はレコードマップとBPL使う演習。コード書かない
    
    ここに演習概要説明あり（Interoperability QuickStartのところ）👉　https://www.intersystems.com/jp/quickstart/

    演習内容👉http://github.com/intersystems/Samples-Integration-RedLights

- [オンラインラーニング（英語）:Integration Architecture](https://learning.intersystems.com/course/view.php?id=908)

    InterSystems IRIS®データプラットフォーム、InterSystems HealthShare®、InterSystems Ensemble®の統合機能の基本的なアーキテクチャを学習します。これらのコンポーネントを通じてデータがどのように流れ、システム間の相互運用が可能になるかを学びます。

    このコースには、3 つのレッスンと数問のクイズが含まれています。ビデオはフルスクリーンモードでご覧ください。

    **上記内容をカバーできそうな日本語コンテンツ**
    
    - ビデオ：[Interoperability概要](https://www.youtube.com/watch?v=vo12UnH-c-s&list=PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s)
   
    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)

- [ビデオ（英語）：Record Mapper Introduction](https://learning.intersystems.com/enrol/index.php?id=1094)

    ↑のビデオほど細かくないのとシンプルなサンプルだけどFAQトピックでこんな日本語記事有→[レコードマップで何ができるか？](https://jp.community.intersystems.com/node/494326)

- [ビデオ（英語）:Using the Complex Record Mapper](https://learning.intersystems.com/enrol/index.php?id=1426)

    日本語無し

- [ビデオ（英語）Building BPL Business Processes (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2030)

    《サンプルと記事を読みながら学習する場合》
    ※オンラインラーニングのほうが説明が浅く広い（HL7系の話も少し含まれてる）

    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・プロセス）](https://jp.community.intersystems.com/node/483171)


- [ビデオ（英語）:Setting Up Business Rules](https://learning.intersystems.com/course/view.php?id=1295)

    このビデオの日本語字幕あってもいいかも＋日本語記事書いてサンプル掲載しても面白いかも。

- [オンラインラーニング（英語）:Data Transformations Basics](https://learning.intersystems.com/enrol/index.php?id=1170)

    グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。

    >メモ：前提知識にHL7が含まれている。HL7で流れるデータを使って変換書いてる。HL7によってるので、医療以外の人には良くなさそう

## 4. カスタムコンポーネントを使用したシステム統合の開発
FHIR® HL7® V2 コンポーネントなど、多くのビルド済みビジネスコンポーネントが開発者に提供されています。これだけでは不十分な場合は、カスタムコンポーネントを構築して、データの取り込み方法を完全にカスタマイズすることができます。

- [ビデオ（英語）：Building Custom Production Messages](https://learning.intersystems.com/course/view.php?name=Custom%20Messages)

    ↑字幕なし＋Atelier登場

    上記ビデオに対応しそうな記事👉　[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

- [オンラインラーニング（英語）：Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)

- [オンラインラーニング（英語）:Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)

    《サンプルと記事を読みながら学習する場合》
    ※オンラインラーニングのほうが説明が浅く広い（HL7系の話も少し含まれてる）

    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)
    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)


- [オンラインラーニング（英語）:Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)

    APIファーストのステップで作るCoffee Maker API

    《サンプルと記事を読みながらの学習なら》
    - [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    - [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)　

    ※このRESTサンプルはAPIファースト用のではないけど、直接呼出しのサービス作成には良い

- [ビデオ（英語）What is PEX?](https://learning.intersystems.com/enrol/index.php?id=1716)

    Production EXtension フレームワーク (PEX) を使用すると、ObjectScript を学習することなく、.NET または Java でカスタム相互運用性コンポーネントを構築できます。PEX を使用すると、使い慣れた言語でコーディングし、確立されたコードライブラリを活用して、プロダクションにコンポーネントを追加できます。PEX を使用してプロダクションを構築する方法については、オンラインコース（英語）[「Creating Interoperability Productions Using PEX」（1 時間）](https://learning.intersystems.com/course/view.php?name=PEXInteroperabilityProductions)を受講してください。


## 5. 他言語を使用したデータアクセス

InterSystems IRIS では、Java、Python、Node.js、.NET などの言語用の統合ツールを提供しています。JDBC を使用して Java を使用するシステムと InterSystems IRIS を統合する方法をご覧ください。

- [ビデオ（英語／日本語字幕あり）Using JDBC with InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=881)


## 6. APIの管理
InterSystems API Manager が提供するツールを参照してください：

- クライアント側の開発者が利用可能な API のドキュメントを公開する
- 実行されたコールに関するメトリックの提供
- スロットリングやセキュリティの構築

- [ビデオ（英語）:What is InterSystems API Manager?](https://learning.intersystems.com/course/view.php?name=What%20is%20IAM)

    日本語資料なら以下？

    - [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)


- [ビデオ（英語）:Installing InterSystems API Manager](https://learning.intersystems.com/enrol/index.php?id=1726)

    InterSystems API Manager バージョン 1.5+ のインストール手順、InterSystems IRIS® データベース・プラットフォーム・インスタンスとホスト・システムの準備方法、および API Manager インストール・キットで提供されるスクリプトの実行方法について説明します。

    ※古いけど同じ方法なのか？（2024年1月19日時点：IAM 3.4）

- [演習環境付き演習（英語）:Hands-On with InterSystems API Manager for Developers](https://learning.intersystems.com/course/view.php?name=IAMExercise)

    InterSystems API Manager を使用して、InterSystems IRIS® データ・プラットフォーム内のコーヒー・メーカー・アプリケーションの API を管理します。

    前提学習または経験 コンテナと Docker の基本的な知識。REST と HTTP リクエスト・レスポンス・ステータス・コードの基礎知識
    

## 7. 既存システムからの移行
既存システムからの移行の検討が必要ですか？

- [ドキュメント：TSQLの移行の計画と実行](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GTSQ_intro)


## 8. リアルタイム分析の構築
InterSystems IRISに組み込まれたInterSystems IRIS Business Intelligenceは、ほぼリアルタイムの分析を提供します。このデータを使って、ダッシュボードやピボットテーブルを作成し、スループットを分析したり、規制データを報告したりすることができます。レポート作成に関するリソースは、[「レポートの実行」](#10-レポートの実行)のセクションを参照してください。

- [ビデオ（英語）：InterSystems IRIS Business Intelligence Overview](https://learning.intersystems.com/enrol/index.php?id=1660)

- [ビデオ（英語）：Introduction to Cubes in Business Intelligence](https://learning.intersystems.com/enrol/index.php?id=1723)

- [ビデオ（英語）：InterSystems IRIS Business Intelligence: Architect](https://learning.intersystems.com/enrol/index.php?id=1752)

- [ビデオ（英語）:InterSystems IRIS BI: Analyzer](https://learning.intersystems.com/course/view.php?name=IRISBIAnalyzer)

    あっさりした説明だけど、コミュニティのこのビデオ使えるかどうか
    (アーキテクト画面使ったキューブの作成、アナライザ画面使ったピボットの作成、ダッシュボード画面使ったユーザポータル作成ある)

    [開発テンプレート（IRIS Analytics Template）の使い方のご紹介（第8回 InterSystems IRIS Analytics コンテスト）](https://jp.community.intersystems.com/node/484826)


## 9. 機械学習の適用
InterSystems IntegratedML は、SQL 開発者が、従来の専門知識やリソースを必要とせずに、機械学習のパワーを簡単に活用できるようにします。InterSystems IRIS の SQL 環境に直接組み込まれた IntegratedML により、開発者はアプリケーションで予測モデルを作成、トレーニング、テスト、実行することができます。

- [ビデオ（英語）:What Is IntegratedML?](https://learning.intersystems.com/course/view.php?name=What%20is%20IntegratedML)

    こっちのほうがいいような
    - [SQLから始める機械学習 ～　IntegratedMLのご紹介　～（2021年10月19日開催）](https://www.youtube.com/watch?v=3yLK9kBs4ic&list=PLzSN_5VbNaxC-z6_DKUZuO__zyudjLE-g&index=2)


- [ビデオ（英語）:Using IntegratedML with DataRobot](https://www.youtube.com/watch?v=pyaRlb2ExDU)

    同じ内容かわからないけど堀田さんのデモあり
    - [IntegratedMLとDataRobotの連携](https://www.intersystems.com/jp/integratedml-datarobot-demo/)

        ※この連携は今も有効なのか？

- [インフォグラフィック（英語）:Preparing Your Data for Machine Learning](https://learning.intersystems.com/course/view.php?name=Preparing%20Your%20Data)

    このインフォグラフィックは、データを準備するための基本的なステップと、IntegratedML がそのプロセスをどのように効率化できるかを示しています。データを準備することは、アプリで機械学習を活用するための重要なステップです。

- [インフォグラフィック（英語）:Common Supervised Machine Learning Algorithms](https://learning.intersystems.com/course/view.php?name=Machine%20Learning%20Algorithms)


    インフォグラフィックのところ、堀田さんの以下ビデオで良いような？
    - [機械学習101（2023年11月29日開催　インターシステムズ開発者ウェビナー）](https://www.youtube.com/watch?v=47bP5-AtBVU&list=PLzSN_5VbNaxC-z6_DKUZuO__zyudjLE-g)


- [演習環境付き演習（英語）:Hands-On with IntegratedML](https://learning.intersystems.com/course/view.php?name=HandsOnIntegratedML)

    チュートリアルでも良い？
    - [記事:機械学習を試せるチュートリアル：IntegratedML](https://jp.community.intersystems.com/node/537501)


## 10. レポートの実行
InterSystems Reports と InterSystems IRIS Adaptive Analytics は、レポートの作成、カスタマイズ、表示を可能にします。Adaptive Analyticsを使用することで、サードパーティのテクノロジーを簡単に接続し、さらなる分析を行うことができます。

- [ビデオ（英語）:Introduction to InterSystems Reports](https://learning.intersystems.com/enrol/index.php?id=1444)

    Logi Analytics が提供する InterSystems Reports は、データのビジュアルレポートを迅速に作成・表示できるレポート作成ツールです。このビデオでは、InterSystems Reports とそのコア・コンポーネントを紹介します。より詳細な情報については、Logi Report のドキュメントをご覧ください。

- [演習環境付き演習（英語）:Getting Started with InterSystems Reports](https://learning.intersystems.com/course/view.php?name=GettingStartedInterSystemsReports) 

- [ビデオ（英語）:InterSystems IRIS Adaptive Analytics Overview](https://learning.intersystems.com/course/view.php?id=1754)

    これは岩本さんの説明ビデオは？
    - [InterSystems IRIS Adaptive Analyticsのご紹介（2021年10月12日開催）](https://www.youtube.com/watch?v=8j6iqmT13XI&list=PLzSN_5VbNaxBlWFxRfrrrScerJrpo7xjr&index=3)

- [オンラインラーニング（英語）：InterSystems IRIS Adaptive Analytics Essential](https://learning.intersystems.com/course/view.php?name=AdaptiveAnalyticsEssentials)



## 11. パフォーマンスとスピードの最適化

アプリケーションのパフォーマンスを必要なだけ確保するためには、高性能なインジェストツールでシステムを構成するだけでなく、大量かつ高速なインジェストのためにシャーディングを設定し、フェイルオーバーのためにミラーリングを設定する必要があります。このセクションでは、これらの推奨事項の多くについて説明する。

- [ビデオ（英語）:InterSystems IRIS Speed Test: High-Volume Ingestion](https://learning.intersystems.com/enrol/index.php?id=1545)

    InterSystems IRIS®データ・プラットフォームの新しいオープン・ソース・ハイブリッド・トランザクション／アナリティカル・プロセッシング（HTAP）スピード・テスト・デモの使用方法をご紹介します。InterSystems IRIS が、リアルタイムのアプリケーション・クエリに答えながら、いかに大量のデータを取り込むことができるかをご覧いただけます。このビデオでは、HTAPスピードテストを使って、InterSystems IRISのパフォーマンスをMySQLやSAP HANAなどの他のデータベースと比較する方法を紹介しています。

- [ドキュメント：ミラーリングの構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GHA_MIRROR_SET_CONFIG)

- [ドキュメント：高可用性を実現するためのフェイルオーバー方法](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GHA_failover)

- [オンラインラーニング（英語）:Introduction to Sharding in InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=1181)

    InterSystems IRIS® データ・プラットフォームの水平スケーラビリティ機能であるシャーディングについて学び、この機能を使ってシステム・パフォーマンスを向上させる方法を学びます。このコースには、2 つの説明レッスンといくつかのクイズ問題が含まれています。ビデオはフルスクリーンモードでご覧ください。

- [オンラインラーニング（英語）:Sharding Basics: Planning and Deploying](https://learning.intersystems.com/course/view.php?name=Sharding%20Basics)

    シャーディングは、システムの水平スケーリングに効果的なアプローチです。InterSystems IRIS® データ・プラットフォームを使ってシャーディング・クラスターを計画し、展開する方法をご紹介します。

    このコースには、2つの説明レッスンといくつかのクイズ問題が含まれています。ビデオとシミュレーションはフルスクリーンモードでご覧ください。

- [ドキュメント：分散キャッシュによるユーザ数に応じた水平方向の拡張](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSCALE_ecp)

## 12. What's next
省略

