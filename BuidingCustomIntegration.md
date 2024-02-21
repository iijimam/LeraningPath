# Interoperability：カスタムコンポーネントの作成

オリジナル：[Building Custom Integrations](https://learning.intersystems.com/course/view.php?id=397)

**Credlyのバッジあり**

InterSystems ObjectScript でInteroperability（相互運用性機能）のカスタムコンポーネントを作成し、InterSystems IRIS® データプラットフォーム製品に追加する方法を学習します。このラーニング・パスは、プロダクション用のカスタムビジネスサービス、プロセス、およびオペレーションを開発する必要のあるソフトウェア開発者向けに設計されています。

InterSystems ObjectScript の使用経験があることを前提としています。必要に応じて、[ObjectScript ラーニング・パス](/ObjectScript.md) を参照してください。

>オリジナルのObjectScriptラーニング・パスの先：https://learning.intersystems.com/course/view.php?id=289

![](/assets/BuildingCustomIntegrations.png)

1. [Interoperabilityプロダクションとは](#1-interoperabilityプロダクションとは)
2. [メッセージの作成](#2-メッセージの作成)
3. [カスタムコンポーネントのデザイン](#3-カスタムコンポーネントのデザイン)
4. [確認](#4-確認)

## 1. Interoperabilityプロダクションとは

- [オンラインラーニング：Receiving and Routing Data in a Production（英語）](https://learning.intersystems.com/course/view.php?name=Interop%20QS)

- [チュートリアル：InterSystems Interoperability（相互運用性）チュートリアル](https://play.instruqt.com/embed/intersystems/tracks/interop-jp?token=em_nMyn9Z_6s9Tq3KTv)
    
    事前準備なしでブラウザ上でお試しいただけます。

- ビデオ：[Interoperability概要](https://www.youtube.com/watch?v=vo12UnH-c-s&list=PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s)

- シリーズ記事
   
   - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

   - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)


## 2. メッセージの作成

プロダクション内のカスタム・コンポーネント間で送信されるプロダクション・メッセージの構築方法を説明します。

- [ビデオ（Atelier登場で古い）：Building Custom Production Messages](https://learning.intersystems.com/course/view.php?id=416)

    ↑字幕なし

    上記ビデオに対応しそうな記事👉　[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

## 3. カスタムコンポーネントのデザイン

プロダクション向けのカスタム・ビジネス・オペレーション、ビジネス・プロセス、ビジネス・サービスを設計、構築する方法を学びます。

《オンラインラーニングで学習する場合（全て英語）》
- [オンラインラーニング（英語）：Building Custom Business Operations (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2029)

- [オンラインラーニング（英語）：Building BPL Business Processes (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2030)

- [オンラインラーニング（英語）：Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)

《サンプルと記事を読みながら学習する場合》
※オンラインラーニングのほうが説明が浅く広い（HL7系の話も少し含まれてる）

- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)

- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・プロセス）](https://jp.community.intersystems.com/node/483171)

    - [ビデオ：バッチジョブ管理への応用から学ぶ ～インターオペラビリティ機能の ビジネスプロセスを理解する](https://www.youtube.com/watch?v=RUxeT4cTy4k&list=PLzSN_5VbNaxB39_H2QMMEG_EsNEFc0ASz&index=6)

- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)

   - [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)

## 4. 確認