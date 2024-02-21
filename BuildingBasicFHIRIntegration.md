# InterSystems 製品を使った基本的なFHIRインテグレーション

オリジナル：[Building Basic FHIR Integrations with InterSystems](
https://learning.intersystems.com/course/view.php?id=1959)

InterSystems IRIS for Health™ または HealthShare® Health Connect で HL7® FHIR® アプリケーションを構築するための基本を学習します。このパスでは、FHIR エンドポイントを設定し、FHIR データを入力および変換する方法を説明します。また、API を管理し、クライアントアプリケーションから FHIR リソースにクエリを実行する方法についても説明します。

InterSystems製品を利用したシステム統合処理についての前提知識を習得される場合は以下コンテンツをご利用ください。

- InterSystems製品の基本構造について

    [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

    [7:03～ ネームスペースとデータベースについて](https://www.youtube.com/watch?v=ID6ImJTgJRk&t=423s)

- [オンラインラーニング（英語）：Integration Architecture（英語）](https://learning.intersystems.com/course/view.php?name=Integration%20Architecture)

    上記内容をカバーできそうな日本語コンテンツ
    
    - ビデオ：[Interoperability概要](https://www.youtube.com/watch?v=vo12UnH-c-s&list=PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s)
   
    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

    - シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)

![](/assets/BuildingBasicFHIRIntegration.png)

1. [FHIR概要](#1-fhir概要)
2. [HL7 FHIRサーバの作成](#2-hl7-fhirサーバの作成)
3. [HL7 FHIRフォーマットへのデータ変換](#3-hl7-fhirフォーマットへのデータ変換))
4. [HL7 FHIRインタラクションを利用する](#4-hl7-fhir-インタラクションを利用する)
5. [エンドポイントのセキュア化](#5-エンドポイントのセキュア化)
6. [API管理](#6-api管理)
7. [ハンズオン！](#7-ハンズオン)
8. [次は](#8-次は)

## 1. FHIR概要

医療用文書の標準フォーマットとして、また医療相互運用性にとってFHIRが重要である理由を学び、InterSystems IRIS for HealthがどのようにFHIRインテグレーションとアプリケーション開発をサポートしているかを学習します。

- [ビデオ（日本語）：HL7® FHIR® × InterSystems IRIS for Health](https://www.youtube.com/watch?v=rbIF4z8xRIY&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=1)

- [ビデオ（日本語字幕）:FHIR - 未来のために設計された医療データスタンダード "FHIR A Healthcare Data Standard Designed for the Future"](https://www.youtube.com/watch?v=gNjlaARboYk)

- [ドキュメント：アーキテクチャ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_arch)


>オリジナルは以下ビデオを指してる（字幕なし）

    [What is FHIR？](https://learning.intersystems.com/course/view.php?name=What%20is%20FHIR)

    [Improving Interoperability with FHIR](https://learning.intersystems.com/course/view.php?id=2202)


## 2. HL7 FHIRサーバの作成
FHIR データを消費する FHIR エンドポイントを作成し、他の FHIR プロファイルをサポートするように構成できます。InterSystems IRIS for Health が受信する HL7® CDA®、CSV、HL7® V2、XML データを FHIR フォーマットに変換する方法をご覧ください。

- [ドキュメント：FHIR サーバのインストールと構成](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_install)

- [演習環境付き体験：Importing FHIR Packages into the InterSystems IRIS for Health Server（英語）](https://learning.intersystems.com/course/view.php?id=1721)

- 日本語コンテンツ

    - [動画：他形式データからFHIR への変換](https://jp.community.intersystems.com/node/492506)

    - [動画：FHIR プロファイル](https://jp.community.intersystems.com/node/495321)

    - [FHIR R4 リソースリポジトリを簡単にお試しいただける開発環境テンプレートのご紹介](https://jp.community.intersystems.com/node/491836)

        [ビデオ：REST クライアントから FHIR R4 リソースリポジトリにアクセスする例](https://www.youtube.com/watch?v=AYz6d7MxXos)


## 3. HL7 FHIRフォーマットへのデータ変換

**※SDA経由をここで書くかどうか(以下オリジナルに沿った内容)**
InterSystems IRIS for Health を使用して、サマリー・ドキュメント・アーキテクチャ（SDA）と組み込みの変換を使用して、受信データを FHIR フォーマットに変換します。

- [ビデオ：Converting Legacy Data to HL7 FHIR R4 in InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=1744)

- [ビデオ：What is SDA?](https://learning.intersystems.com/course/view.php?id=2128)

- [オンラインラーニング：Transforming Data into the HL7 FHIR Format](https://learning.intersystems.com/course/view.php?id=2149)

    InterSystems IRIS for Health™ または HealthShare® Health Connect を使用して、医療システム間のデータ交換に一般的に使用されている HL7® FHIR® フォーマットにデータを変換する方法をお試しいただけます。その後、動的オブジェクトを使用してFHIRデータを操作する方法を学びます。コースの終わりには、実習でHL7 V2リソースをFHIRフォーマットに変換するための本番環境のセットアップを完了します。

    （オプションにFHIR用要求応答メッセージのQuickStreamに入ったJSONを修正できるようにダイナミックオブジェクトの操作演習が含まれている）

---
**日本オリジナルだとこう？**

- [動画：FHIRデータ変換機能](https://www.youtube.com/watch?v=rbIF4z8xRIY&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=1&t=865s)

- [ビデオ：JSONテンプレートエンジンのご紹介～FHIR JSONフォーマットを簡単生成～](https://www.youtube.com/watch?v=H4LzOV-Tfzg&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=5)

- 講師付きトレーニング
    - CSVからFHIRへの変換
        
        JSONテンプレートエンジンを利用した変換方法を習得できるコースです。
        作成例として、CSVで入力された情報からFHIRリソースを作成し、IRISに用意したFHIRリポジトリに登録する流れを体験します。

    - SSMIX2からFHIRへの変換（これは掲載する？）

        SDA経由の変換を体験できるコースです。

## 4. HL7 FHIR インタラクションを利用する

CRUDインタラクションの実行-クライアントアプリケーションからのFHIRリソースの検索や、RESTクライアントからの操作のテストなどを確認できます。

- [ビデオ：Searching for FHIR Resources in InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=1287)

    [日本語ビデオ：FHIR+IRIS for Health 101](https://youtu.be/S7PV3RIpMUM?t=1077)

- [ドキュメント：相互作用（インタラクション）](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_arch_supported_interactions)


## 5. エンドポイントのセキュア化
新しいFHIRサーバーをセットアップする際に、OAuth2.0でエンドポイントを保護し、プロダクショングレードのウェブサーバーを使用する方法を解説します。

- [ビデオ：Configuring the InterSystems Web Gateway](https://learning.intersystems.com/course/view.php?id=1787)

    Webゲートウェイのインストールを解説するトレーニング資料あり

- [ドキュメント：OAuth2.0認証](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_auth_oauth)

## 6. API管理

InterSystems API Manager を使用して FHIR エンドポイントへのトラフィックを制御する方法と、トラブルシューティングのテクニックを紹介します。

> USがさしてる概要ページ　[What is InterSystems API Manager?](https://learning.intersystems.com/course/view.php?name=What%20is%20IAM)　　＋　オンラインラーニング　https://learning.intersystems.com/course/view.php?id=1747

    IAM概要とハンズオンがあるといい
    概要説明ページに翻訳つけるだけでもいいかも？？

コミュニティのページを指すのはどうか？

- [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)

- [体験環境付き演習（英語）：Building FHIR Applications with InterSystems API Manager](https://learning.intersystems.com/course/view.php?id=1654)

    [演習資料PDF→これを例に日本語の演習作れる？コンテナで試せるようにしたらいい？](https://learning.intersystems.com/pluginfile.php/38823/mod_resource/content/10/FHIRExerciseGuide%20%281%29.pdf)

    InterSystems API Manager を使用して API を表示し、HL7® FHIR® アプリケーションを作成して、FHIR リクエストを監視する方法について説明します。

    この実習を修了するまでに、以下のことができるようになります：

    - InterSystems API Manager を使用して API を表示し、FHIR 要求のテスト
    - REST クライアントを使用して、InterSystems IRIS for Health™ に FHIR リクエストを作成
    - FHIR アプリケーションを InterSystems IRIS for Health に接続させる
    - API Manager 開発者ポータルで統計を表示して API 呼び出しを監視

- [ドキュメント：FHIR サーバのデバッグ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_debugMaintain)


## 7. ハンズオン！
この最後の演習では、サンプルのフロントエンドを使って、完全なFHIRアプリケーションを構築する練習をします。

- [体験環境付き演習（英語）：Working with the FHIR Resource Repository](https://learning.intersystems.com/course/view.php?name=FHIR%20Resource%20Repository)

    Syntheaデータ入れてRESTクライアントで試す＋Webページに表示させる内容
    
    日本語：初期のFHIRハンズオン資料がこの内容。一応試せるかも。どこかに置かないといけない

## 8. 次は？