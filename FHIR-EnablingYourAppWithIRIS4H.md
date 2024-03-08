# FHIR - InterSystems IRIS for Healthでアプリケーションを有効にする
> オリジナル[FHIR-Enabling Your Applications with InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=2323)

InterSystems IRIS for Health™ を使用して、FHIR Facade を作成し、ヘルスケア・アプリケーションが HL7® FHIR® フォーマットでデータを送受信できるようにすることができます。このラーニングパスでは、以下の方法を学習できます。

- RESTを使用して、EHRのような外部のFHIRサーバーと対話するようにアプリケーションをセットアップする。
- 標準的なヘルスケアデータ形式のメッセージを FHIR 形式に変換する。
- FHIR Interoperability Adapterを使用してFHIR Facadeを設定する。

![](/assets/FHIR-EnablingYourAppWithIRIS4H.png)


0. [開始前の準備](#0-開始前の準備)
1. [はじめに](#1-はじめに)
2. [FHIRデータを送受信するためのRESTの使用方法](#2-fhirデータを送受信するためのrestの使用方法)
3. [HL7 FHIR へのデータ変換](#3-hl7-fhir-へのデータ変換)
4. [FHIR ファサードの作成](#4-fhir-ファサードの作成)

## 0. 開始前の準備

FHIRの基本的な知識について確認するため、以下のビデオをご参照ください。

- [ビデオ（英語）:What Is FHIR?](https://learning.intersystems.com/course/view.php?name=What%20is%20FHIR)

    以下ビデオで代用できる？
    - [動画：FHIR+IRIS for Health 101](動画：FHIR+IRIS for Health 101)

## 1. はじめに
アプリケーションのFHIR化に必要なアーキテクチャを紹介します。

- [ビデオ（英語）:FHIR Facade Architecture Overview](https://learning.intersystems.com/course/view.php?id=2137)

    アプリケーションが HL7® FHIR® リクエストに応答できるように、FHIR Facade アーキテクチャをセットアップする方法をご覧ください。このアーキテクチャを使用すると、InterSystems インスタンスを FHIR サーバーにすることができ、完全な FHIR リポジトリとして機能します。

    ※ビデオがない・・

## 2. FHIRデータを送受信するためのRESTの使用方法
インターシステムズのデータ・プラットフォームで REST エンドポイントを設定し、REST を使用した FHIR 相互運用性アダプタを使用して外部の FHIR サーバとやり取りする方法を確認し、FHIR レスポンス・メッセージを入力して REST 経由で FHIR データを送信する練習をします。

- [オンラインコース（英語）:Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)

    APIファーストのステップで作るCoffee Maker API

    《サンプルと記事を読みながらの学習なら》
    - [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    - [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)　

    ※このRESTサンプルはAPIファースト用のではないけど、直接呼出しのサービス作成には良い

- [ドキュメント：FHIR相互運用アダプタ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_fhir_adapter)

- [演習環境付き演習（英語）：Populating FHIR Response Messages](https://learning.intersystems.com/course/view.php?id=2272)

    FHIR Facade として構成された InterSystems IRIS for Health™ のインスタンスを使用して、HL7® FHIR® 要求を受け付け、InterSystems® データベースから要求されたデータを取得し、このデータを FHIR 形式で要求システムに返送するプロダクションを完成させます。

    InterSystems IRIS for Health または HealthShare® Health Connect を使用して FHIR 相互運用性ソリューションを構築する場合、FHIR 要求と応答はプロセスの不可欠な部分です。FHIR Facadeの場合、外部システムはFHIRリクエストを使用してFHIR形式のデータを要求します。データを収集し、FHIR形式に変換した後、FHIR応答メッセージを入力してデータを要求元のシステムに送り返す必要があります。

    この演習では、FHIR形式に変換された患者データを受け取り、このデータをFHIR応答メッセージに入力します。その後、REST クライアントを使用して患者データを要求し、応答メッセージが正しく入力されたことを確認します。

    ※プロダクションを使って変換する流れの一部（BP->BO）を演習で作る

## 3. HL7 FHIR へのデータ変換

インターシステムズの標準データフォーマットであるSDAについて学び、SDAを使用して標準的なヘルスケアフォーマットのデータをFHIRフォーマットに変換する方法をご覧ください。

- [ドキュメント：SDAドキュメント](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXSDA_ch_sda)

- [オンラインコース（英語）:Transforming Data into the HL7 FHIR Format](https://learning.intersystems.com/course/view.php?name=FHIRTransformations)

    InterSystems IRIS for Health™ または HealthShare® Health Connect を使用して、医療システム間のデータ交換に一般的に使用されている HL7® FHIR® フォーマットにデータを変換する方法をご覧ください。次に、ダイナミックオブジェクトを使用して FHIR データを操作する方法を学びます。

    > HL7 - SDA - FHIR の説明＋SDA-FHIRになったときに%bundleに入ったダイナミックオブジェクトを操作する例など


## 4. FHIR ファサードの作成

この最後の演習では、FHIR相互運用性アダプタを使用してFHIR Facadeを作成する練習をします。

- [演習環境付き演習（英語）:Creating a Simple FHIR Facade](https://learning.intersystems.com/course/view.php?id=2274)

    InterSystems IRIS for Health™ のインスタンスを使用して、FHIR Facade アーキテクチャを作成および構成することで、システムが HL7® FHIR® リクエストを受け入れ、データが元々この形式で保存されていない場合でも FHIR データを返すことができます。FHIR Facade を作成するには、FHIR 相互運用性アダプタを使用します。これは、特別なビジネスホストを使用してプロダクションで FHIR リクエストを処理する新しい相互運用性 REST エンドポイントを作成します。このプロダクションを使用して、データの検索と変換を促進し、要求されたデータを返すことができます。

    この演習では、内部形式でEMRデータを保存する医療施設のFHIR Facadeを作成します。この施設では、患者の詳細をJSON形式で返すREST APIが設定されていますが、FHIR形式の患者データの要求を受けています。

    > HS.FHIR.DTL.vR4.Model.Resource.Patient　を使ってる　古い？


