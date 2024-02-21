# InterSystems IRISを利用したビジネス・インテグレーションの構築
オリジナル[Building Business Integrations with InterSystems IRIS](https://learning.intersystems.com/course/view.php?id=1437)

InterSystems製品の相互運用性フレームワークにより、インターフェイスエンジニアやソフトウェア開発者は、複数のシステムを接続し、下流のアプリケーションにメッセージを迅速にルーティングすることができます。このラーニング・パスでは、統合（インテグレーション）の基本を学び、組み込みオプションやカスタムオプションを使用してデータを送信、受信、処理、変換する方法を確認できます。

![](/assets/BuildingBusinessIntegrations.png)

1. [はじめに](#1-はじめに)
2. [処理とデータ変換](#2-処理とデータ変換)
3. [カスタムコンポーネントの開発](#3-カスタムコンポーネントの開発)


## 1. はじめに
このラーニング・パスで学習する内容を確認します。また、プロダクションの主なコンポーネントを含む統合アーキテクチャの基礎をビデオで学習します。

（ビデオでは、IRISを利用することで、様々なシステムやアプリケーションのさせル統合ツールとして利用でき、データ変換、ルーティングなど指示できるよ。
ユニークソリューションに対してはカスタムコンポーネントの開発ができるよ。な感じを解説してる概要。）

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

## 2. 処理とデータ変換
InterSystems IRIS に組み込まれているグラフィカル・ツールを使用して、メッセージを取り込み、正しい形式で下流のシステムに渡します。

- [ビデオ（英語）：Record Mapper Introduction](https://learning.intersystems.com/enrol/index.php?id=1094)

    ↑のビデオほど細かくないのとシンプルなサンプルだけどFAQトピックでこんな日本語記事有→[レコードマップで何ができるか？](https://jp.community.intersystems.com/node/494326)

- [オンラインラーニング（英語）:Building BPL Business Processes](https://learning.intersystems.com/course/view.php?name=Building%20BPL%20Business%20Processes)

    管理ポータルのビジネス・プロセス・デザイナーを使用して、BPLビジネス・プロセスを構築する方法を学びます。このコースには、6つのインストラクションレッスンといくつかのクイズ問題が含まれています。ビデオはフルスクリーンモードで見るのが最適です。

    コース受講に必要な前提知識は以下の通り（コンポーネントそれぞれの役割とプロダクション構成の画面操作ができること＋ビジネスオペレーションの作成方法を知っていること）

    - [Integration Architecture](https://learning.intersystems.com/course/view.php?name=Integration%20Architecture)

        （日本語コンテンツについては、[はじめに](#1-はじめに)と同じ内容）

    - [オンラインラーニング（英語）:Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)

        《サンプルと日本語記事を読みながら学習する場合》
        ※オンラインラーニングのほうが説明が浅く広い（HL7系の話も少し含まれてる）

        - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)  

    - [ビデオ（英語）:Setting Up Business Rules](https://learning.intersystems.com/course/view.php?id=1295)

        このビデオの日本語字幕あってもいいかも＋日本語記事書いてサンプル掲載しても面白いかも。

    - [オンラインラーニング（英語）:Data Transformations Basics](https://learning.intersystems.com/enrol/index.php?id=1170)

        グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。

        >メモ：前提知識にHL7が含まれている。HL7で流れるデータを使って変換書いてる。HL7によってるので、医療以外の人には良くなさそう

## 3. カスタムコンポーネントの開発

- [ビデオ（英語）：Building Custom Production Messages](https://learning.intersystems.com/course/view.php?name=Custom%20Messages)

    ↑字幕なし＋Atelier登場

    上記ビデオに対応しそうな記事👉　[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

- [オンラインラーニング（英語）：Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)

- [オンラインラーニング（英語）:Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)

    《サンプルと記事を読みながら学習する場合》
    ※オンラインラーニングのほうが説明が浅く広い（HL7系の話も少し含まれてる）

    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)
    - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)

        - [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)


## 4. 次は

