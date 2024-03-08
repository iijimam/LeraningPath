# インプリメンテーションパートナ向けInterSystems製品をはじめよう（医療）

>オリジナル：[Getting Started with InterSystems for Implementation Partners (Health)](https://learning.intersystems.com/course/view.php?id=1445)

このリソースのリストでは、InterSystems® の概要、InterSystems 製品とテクノロジのアーキテクチャと機能について説明します。このパスに従うことで、コードを書き、統合を構築し、アプリケーションに必要なコンポーネントを作成することを学ぶことができます。

![](/assets/GettingStartedWithImplePartner-Health.png)

このラーニング・パスを終了することに加え、以下の講師付きクラスルームトレーニングコースに参加／個別開催の申し込みを行うことを強く推奨します。

内容|クラスルームトレーニング|オンラインコース
--|--|--
アプリケーションの開発|[InterSystems SQLの使い方](https://www.intersystems.com/jp/intersystems-sql/)<br> [InterSystems Objectの使い方](https://www.intersystems.com/jp/intersystems-object/)|[アプリケーションの開発](#3-アプリケーションの開発)
システム統合の構築|[システム統合機能の使い方（3日間）](https://www.intersystems.com/jp/system-integration-tool/)<br>必要に応じてHL7用システム統合機能の使い方](https://www.intersystems.com/jp/course-offerings/hl7-systems-integration-tool/)|[システム統合の構築](#2-システム統合の構築)<br>[カスタムコンポーネントを使用したシステム統合の開発](#4-カスタムコンポーネントを使用したシステム統合の開発)<br>[プロダクションの構築（上級編）](#5-プロダクションの構築上級編)
HealthShare製品郡の統合|[HealthShare Unified Care Record Fundamentals](https://www.intersystems.com/course-offerings/healthshare-unified-care-record-fundamentals/)|[HealthShare製品郡の統合](#6-healthshare製品郡の統合)

---

1. [InterSystems 製品紹介](#1-intersystems-製品紹介)
2. [システム統合の構築](#2-システム統合の構築)
3. [アプリケーションの開発](#3-アプリケーションの開発)
4. [カスタムコンポーネントを使用したシステム統合の開発](#4-カスタムコンポーネントを使用したシステム統合の開発)
5. [プロダクションの構築（上級編）](#5-プロダクションの構築上級編)
6. [HealthShare製品郡の統合](#6-healthshare製品郡の統合)

## 1. InterSystems 製品紹介
ヘルスケア向けのアプリケーションを構築する場合、InterSystems IRIS for Health が最適です。InterSystems IRIS for Health は、InterSystems IRIS をベースに構築されていますが、ヘルスケア環境で役立ついくつかの機能が追加されています。以下のリソースでは、すべてのインターシステムズ製品とその連携について説明します。

- [オンラインコース（英語）:Introduction to InterSystems Products and Technologies](https://learning.intersystems.com/course/view.php?name=Intro%20to%20InterSystems%20Products)

    InterSystems® の製品とテクノロジーの基本を学び、どのような製品が存在し、どのように使用され、技術的な観点以外からどのように比較されるのかを知ることができます。

    このコースには、4つのレッスンといくつかのクイズが含まれています。このコースのビデオは、フルスクリーンモードで見るのが最適です。

    >DataPlatform／HealthShare／Trakcare　の紹介がある。このまま使うならビデオに字幕付けるだけでOK？

    - 2.1 InterSystemsの説明はこのYouTubeと一緒：[ビデオ（英語）InterSystems へようこそ](https://www.youtube.com/watch?v=v4uoejre5IU)
    （サポートは24*7と言ってる）

    - 2.2 What is InterSystems IRISのビデオは日本語字幕ある
    
        Key Tools of InterSystems IRIS は字幕なし（IDE、管理ポータル、ターミナルの説明）

        これで代用できるかも：[【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

    - 2.3 What is IRIS for Health のビデオは日本語字幕ある

    - 2.4 CachéとEnsembleについて（ビデオは英語のみ）

    - 3. What is HealthShare (ビデオは英語のみ)　マーラさんの例で紹介されている

        7年前のビデオ+HSファミリーに触れてないけど日本語訳付きの[ペイシェント・ジャーニー](https://www.youtube.com/watch?v=uvsc3GFaURk)

- [ビデオ（英語／日本語字幕あり）What is InterSystems IRIS for Health?](https://learning.intersystems.com/course/view.php?id=2117)


## 2. システム統合の構築

このセクションでは、統合ソリューションのアーキテクチャ、基本的なプロダクションとデータ変換の構築方法、およびプロダクションのテストに必要な基本的なエラー処理とトラブルシューティングの実行方法について説明します。

> 以下の内容トレーニングコースで補える（HL7用コース資料更新してない）

- [オンラインコース（英語）：Integration Architecture（英語）](https://learning.intersystems.com/course/view.php?name=Integration%20Architecture)

    上記内容をカバーできそうな日本語コンテンツ
    
    - ビデオ：[Interoperability概要](https://www.youtube.com/watch?v=vo12UnH-c-s&list=PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s)
   
    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)

- [オンラインコース（英語）:HL7 Business Services and Business Operations](https://learning.intersystems.com/enrol/index.php?id=1393)

- [ビデオ（英語）:Getting Started with HL7 V2 Routing Rules](https://learning.intersystems.com/course/view.php?id=1129)

    InterSystems IRIS for Health™ 製品の HL7® V2 ルーティング・ルールの機能を学び、ルール・エディタを使用して、受信メッセージを評価し、適切なダウンストリーム・システムにルーティングするルール・セットを作成する方法をご覧ください。次に、テストメッセージのルーティングをシミュレートするためのエディタのテストルールを調べます。

    > ルールエディタ古い

- [オンラインコース（英語）:Data Transformations Basics](https://learning.intersystems.com/enrol/index.php?id=1170)

    グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。

    >メモ：前提知識にHL7が含まれている。HL7で流れるデータを使って変換書いてる。HL7によってるので、医療以外の人には良くなさそう

- [ビデオ（英語）:Designing Custom Schemas](https://learning.intersystems.com/course/view.php?id=1087)

- [ビデオ（英語）:HL7 Schema Editor](https://learning.intersystems.com/enrol/index.php?id=1118)

    InterSystems IRIS for Health™ および InterSystems HealthShare® Health Connect で受信する HL7 V2 メッセージを処理するためのカスタム HL7® V2 スキーマの作成方法について説明します。v2019.1 以降の HL7 スキーマエディタを使用することで、潜在的なバリエーションをより柔軟に処理し、統合を簡素化できます。

    >Zセグメントを例に説明

- [オンラインコース（英語）:Searching Messages Using the Message Viewer](https://learning.intersystems.com/enrol/index.php?id=1432)

- [ビデオ（英語）：Error Handling in HL7 Production](https://learning.intersystems.com/course/view.php?id=1260)

    Ens.Alertを使う例（ルーターの検証を使ってる）

- [ビデオ（英語）:Introduction to Troubleshooting Productions](https://learning.intersystems.com/course/view.php?id=1172)

    InterSystems IRIS® データ・プラットフォーム、InterSystems Ensemble®、および InterSystems HealthShare® におけるプロダクションのトラブルシューティング方法について説明します。ログ、メッセージ、キュー、およびジョブを表示するための管理ポータル・ページの場所と目的を確認します。このコースには、5 つのレッスンといくつかのクイズ問題が含まれています。ビデオはフルスクリーンモードで見るのが最適です。

    >発生しているエラーを例にプロダクション構成画面の色の違い、Logタブ、メッセージビューワ、キュー、Jobのそれぞれの画面の使い方を説明してる

- [オンラインコース（英語）:Designing Healthcare Productions](https://learning.intersystems.com/course/view.php?id=1285)

    InterSystems HealthShare® でプロダクションを設計するためのベスト・プラクティス (データベース、ネームスペース、コンポーネントの規約を含む) を確認します。HealthShare を開発環境として設定し、プロダクションを構築してテストする方法を学びます。このコースには、3つのレッスンといくつかのクイズが含まれています。ビデオはフルスクリーンモードでご覧ください。

    1. Envieonment Design
        - システムDBにユーザコード入れちゃだめ（ユーザ用環境として独自にNS,DB作る）
        - データとコードを分ける運用についての説明
    
    2. Production Design

        各コンポーネントのデザイン例を紹介（HL7）

- [演習環境付き演習（英語）：Final Exercise: Building Your First HL7 Production](https://learning.intersystems.com/course/view.php?id=1342)    

- 認定テスト

    [HealthShare Health Connect HL7 Interface Specialist](https://learning.intersystems.com/mod/url/view.php?id=7154)


## 3. アプリケーションの開発

InterSystems IRIS で ObjectScript を使用して高性能なアプリケーションを構築する方法を学びます。そうすることで、次のことができるようになります：

ビジネスルールとメッセージルータのコードでカスタム関数を作成する。
カスタムコードによる高度なデータ変換の作成
カスタム・プロダクション・コンポーネントの構築
カスタム・ビジネス・コンポーネントの構築方法の詳細については、このラーニング・パスの[カスタムコンポーネントを使用したシステム統合の開発](#4-カスタムコンポーネントを使用したシステム統合の開発)セクションを参照してください。

### オリジナル

- [ビデオ（英語）InterSystems Architecture Overview](https://learning.intersystems.com/course/view.php?name=Architecture%20Overview)

- [オンラインコース（英語）：Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)

- [オンラインコース（英語）:InterSystems ObjectScript Basics](https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics)

- [ドキュメント：クラス・プログラミングの基本的な考え方](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GOBJ_intro)

- [オンラインコース（英語）:InterSystems IRIS Objects Introduction](https://learning.intersystems.com/enrol/index.php?id=2225)

- [オンラインコース（英語）：InterSystems SQL Overview](https://learning.intersystems.com/enrol/index.php?id=960)

- [オンラインコース（英語）:Using JSON in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS)

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


## 4. カスタムコンポーネントを使用したシステム統合の開発
このセクションは、プロダクション用のカスタム・ビジネス・コンポーネントを構築する必要があるソフトウェア開発者のために設計されています。以下のアクティビティを順番に完了することをお勧めします。

- [ビデオ（英語）：Building Custom Production Messages](https://learning.intersystems.com/course/view.php?name=Custom%20Messages)

    ↑字幕なし＋Atelier登場

    上記ビデオに対応しそうな記事👉　[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

- [オンラインコース（英語）：Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)

- [ビデオ（英語）Building BPL Business Processes (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2030)


- [オンラインコース（英語）:Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)

    《サンプルと記事を読みながら学習する場合》
    ※オンラインコースのほうが説明が浅く広い（HL7系の話も少し含まれてる）


- 日本用なら《サンプルと記事を読みながら学習する場合》
※オンラインコースのほうが説明が浅く広い（HL7系の話も少し含まれてる）

    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)
    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・プロセス）](https://jp.community.intersystems.com/node/483171)
    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)


## 5. プロダクションの構築（上級編）
このセクションは、高度な HL7 V2 機能を使用する必要のあるインタフェース・エンジニアやソフ トウェア開発者のために設計されています。

- [オンラインコース（英語）:Advanced Data Transformations](https://learning.intersystems.com/enrol/index.php?id=2381)

    コードアクション、ユーティリティ関数、ルックアップテーブル、サブトランスフォーメーションなど、管理ポータルの DTL Editor の高度な機能を検討し、それらをデータ変換のロジックに組み込む方法を学びます。

- [オンラインコース（英語）:Setting Up Alerts](https://learning.intersystems.com/course/view.php?name=Setting%20Up%20Alerts)

    管理ポータルを使用して、プロダクションでアラートを構成し、ビジネス・コンポーネントでエラーが発生したり、メッセージがキューに長く留まったりした場合に通知を送信する方法を学びます。

- [オンラインコース（英語）:Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)

    APIファーストのステップで作るCoffee Maker API

    《サンプルと記事を読みながらの学習なら》
    - [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    - [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)　

    ※このRESTサンプルはAPIファースト用のではないけど、直接呼出しのサービス作成には良い

- [ビデオ（英語）:Setting Up Business Rules](https://learning.intersystems.com/course/view.php?id=1295)

    このビデオの日本語字幕あってもいいかも＋日本語記事書いてサンプル掲載しても面白いかも。

- [ビデオ（英語）：Record Mapper Introduction](https://learning.intersystems.com/enrol/index.php?id=1094)

    ↑のビデオほど細かくないのとシンプルなサンプルだけどFAQトピックでこんな日本語記事有→[レコードマップで何ができるか？](https://jp.community.intersystems.com/node/494326)


- [ビデオ（英語）:What is InterSystems API Manager?](https://learning.intersystems.com/course/view.php?name=What%20is%20IAM)

    日本語資料なら以下？

    - [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)


- [ビデオ（英語）:Installing InterSystems API Manager](https://learning.intersystems.com/enrol/index.php?id=1726)

    InterSystems API Manager バージョン 1.5+ のインストール手順、InterSystems IRIS® データベース・プラットフォーム・インスタンスとホスト・システムの準備方法、および API Manager インストール・キットで提供されるスクリプトの実行方法について説明します。

    ※古いけど同じ方法なのか？（2024年1月19日時点：IAM 3.4）

- [演習環境付き演習（英語）:Hands-On with InterSystems API Manager for Developers](https://learning.intersystems.com/course/view.php?name=IAMExercise)

    InterSystems API Manager を使用して、InterSystems IRIS® データ・プラットフォーム内のコーヒー・メーカー・アプリケーションの API を管理します。

    前提学習または経験 コンテナと Docker の基本的な知識。REST と HTTP リクエスト・レスポンス・ステータス・コードの基礎知識
    

## 6. HealthShare製品郡の統合

インターシステムズは、HealthShare製品ファミリーの中でIRIS for Healthと統合することが多い他の製品も提供しています。HealthShare製品（Unified Care Record、Patient Index、Health Insight、Personal Community）については、以下のリソースをご利用ください。

注：これらのリソースは、HealthShareの顧客とパートナーだけが利用できます。アクセスできるはずなのにアクセスできない場合は、リンク先の指示に従ってください。

- [オンラインコース（英語）:HealthShare Unified Care Record Basics](https://learning.intersystems.com/course/view.php?name=HSUCRBasics)

- [オンラインコース（英語）:HealthShare Patient Index Overview](https://learning.intersystems.com/enrol/index.php?id=2135)

- [ラーニング・パス（英語）：Analyzing Data with Health Insight](https://learning.intersystems.com/course/view.php?name=HSHILP)

- [ラーニング・パス（英語）:Exploring Unified Care Record](https://learning.intersystems.com/enrol/index.php?id=2407)

- [ラーニング・パス（英語）:Advancing Patient Engagement with Personal Community](https://learning.intersystems.com/enrol/index.php?id=2411)

- [クラスルームトレーニング：HealthShare Unified Care Record Fundamentals]()

## Further resources
省略


