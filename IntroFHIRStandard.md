# FHIRのご紹介

> オリジナルページ：[Introduction to the FHIR Standard](https://learning.intersystems.com/course/view.php?id=2401)

> RUSSが話す超概要的な内容が多いもの。InterSystems 製品特化の内容はない。ビデオ（英語）に字幕を付けるだけでいいか、対応できそうな塩川さんや先生の講演を貼るか、もしくは日本オリジナルで作るか？**《要検討》**

HL7® FHIR® を世界をリードするヘルスケアデータ標準にしている多くの特徴と機能について学びます。このラーニング・パスでは、FHIR 標準がどのように機能し、最新のヘルスケアアプリケーションでどのように使用されるかを学びます。FHIR データモデルの実習を行い、FHIR データ標準についてよくある質問にお答えします。

![](/assets/IntrotoFHIR.png)

1.[FHIRのコンセプトを理解する](#1-fhirのコンセプトを理解する)
2.[FHIRの仕様を探る](#2-fhirの仕様を探る)
3.[FHIRリソースの構造を理解する](#3-fhirリソースの構造を理解する)
4.[FHIRデータモデルを構築する](#4-fhirデータモデルを構築する)
5.[FHIRの実践を理解する](#5-fhirの実践を理解する)

## 1. FHIRのコンセプトを理解する
FHIRデータ標準を利用することで相互運用性をどのように向上させるかを学習します。

**↓講演とかのっけていいのか？　それともオリジナルに日本語字幕を付けるかどうか**

- [FHIRの解説と動向・課題・今後の展望（IHE 塩川康成様のご講演）](https://www.youtube.com/watch?v=BM_lJtMPdXg&list=PLgFt3CvX3OePNM4vVY2oer6hDNrJqgv1A)

- [ビデオ（日本語字幕）:FHIR - 未来のために設計された医療データスタンダード "FHIR A Healthcare Data Standard Designed for the Future"](https://www.youtube.com/watch?v=gNjlaARboYk)

    >オリジナルの[Understanding the Concept of FHIR](https://learning.intersystems.com/course/view.php?name=ConceptOfFHIR)　同じ


- [ビデオ（日本語）：HL7® FHIR® × InterSystems IRIS for Health](https://www.youtube.com/watch?v=rbIF4z8xRIY&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=1)

> オリジナルは以下
- [Improving Interoperability with FHIR](https://learning.intersystems.com/course/view.php?name=InteropFHIR)

- [Understanding the Concept of FHIR](https://learning.intersystems.com/course/view.php?name=ConceptOfFHIR)


## 2. FHIRの仕様を探る
FHIR仕様がデータをどのように保存し共有するかを定義されているか、またデータ標準の全体的な目標を学習します。


- [ビデオ（英語）：What Is the HL7 FHIR Specification?](https://learning.intersystems.com/course/view.php?name=HL7FHIRSpec)

    HL7® FHIR® ヘルスケアデータ標準の概要と、FHIR標準仕様のウェブサイトナビゲート方法をご紹介しています。FHIRの標準化の目標、データの保存と共有方法の基本、仕様内のさまざまなデータモジュール間の関係について学びます。

    ＜メモ＞以下日本語ビデオで対応できる？
    - [ビデオ（日本語）：FHIR+IRIS for Health 101](https://www.youtube.com/watch?v=S7PV3RIpMUM&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=2)

- [ビデオ（英語）：Organizing HL7 FHIR Resources](https://learning.intersystems.com/course/view.php?name=OrganizingFHIRResources)

## 3. FHIRリソースの構造を理解する
個々のFHIRリソースの構造、データ表現の一貫性を可能にするデータ型と用語バインディングについて、FHIR標準仕様のウェブサイトを使用しながら確認します。

- [ビデオ（英語）：Understanding the Structure of HL7 FHIR Resources](https://learning.intersystems.com/course/view.php?name=StructureFHIRResources)

    HL7® FHIR® リソースの構造を紹介します。FHIR ウェブサイトのリソースのツリー表示の見方と読み方を確認できます。これにより、リソースに含まれるさまざまなデータ要素を理解することができます。また、リソースを XML、JSON、または Turtle で表示する方法や、FHIR リソースの UML (Universal Modeling Language) ダイアグラムの場所についても説明します。

- [ビデオ（英語）：Identifying Structured and Coded Data in HL7 FHIR Resources](https://learning.intersystems.com/course/view.php?name=StructuredCodedFHIRData)

    >メモ：データタイプ（CodeableConceptとかの複雑なものがあるよ）とValueSetに入る内容（用語）について説明してる

    HL7® FHIR® で使用され、データセットの表現に一貫性を持たせる、構造化データとコード化データの識別方法を学習できます。FHIR で使用されるデータ型と、用語バインディングが要素定義をデータ型と値セットにどのように結びつけるかを確認できます。FHIRリソースの一部として定義されたコードや、LOINCやSNOMEDのような外部の用語体系から引き出されたコードの例をご覧ください。

## 4. FHIRデータモデルを構築する
FHIRプロファイルと実装ガイド、FHIR shorthand を詳しく見て、FHIRデータアーキテクチャの学習します。

- [ビデオ（英語）:Understanding HL7 FHIR Profiles](https://learning.intersystems.com/course/view.php?name=FHIRProfiles)

- [ビデオ（英語）：What Are HL7 FHIR Implementation Guides?](https://learning.intersystems.com/course/view.php?name=FHIRIGs)

- [ビデオ（英語）：Using HL7 FHIR Shorthand](https://learning.intersystems.com/course/view.php?name=FHIRShorthand)

- [演習環境付き演習（英語）：Building a FHIR Data Architecture](https://learning.intersystems.com/course/view.php?id=2279)

    HL7® FHIR® アーキテクチャとその基礎となるデータモデルの基礎を学びます。この演習では、InterSystems がサポートする Graph Builder 2 (GB2) アプリを使用して、FHIR を使用した開発の基礎となる FHIR データアーキテクチャの構築を開始します。

    > 2年前？のSEサミットか何かで操作したブラウザ上でリソースを作るツールを使う演習。FSHエディタの操作もある。画面翻訳したらできる感じ？


## 5. FHIRの実践を理解する
医療システム間のセマンティック相互運用性について学び、FHIR分野で最もよくある質問を調査する。

    対応するものがないので翻訳つけるだけでいいか、日本語用に何か作るか

＜オリジナル＞
- [Achieving True Interoperability in Healthcare Systems](https://learning.intersystems.com/course/view.php?id=2203) 
    
    セマンティック相互運用性の概念と、医療データ交換におけるその役割についてご紹介します。セマンティック相互運用性は、医療データが確実に伝送されるだけでなく、容易に理解されることを保証するために、システムマッピングを超えるものです。HL7® FHIR® データ標準がこの課題にどのように対応できるかの紹介。
    (同じ病名疑いでもそれぞれの病院で記載される書かれ方はそれぞれ。それを同じであるとみなすことはシステムだけではできない。FHIRのプロファイルを使って当てはめれば違うEHRの書き方でも統一できるよ。的な内容。人の確認も必要よ)

- [FHIR FAQs](https://learning.intersystems.com/course/view.php?id=2278)

    InterSystems のSenior Clinical Interoperability Advisor である Russ Leftwich が HL7® FHIR® に関して遭遇する、FAQの紹介