# InterSysetms IRIS 管理の基本

> オリジナル:[InterSystems IRIS Management Basics](https://learning.intersystems.com/course/view.php?id=1825)

InterSystems IRIS® データプラットフォームの基礎と、システム管理者が製品のライフサイクルを通じて一般的なタスクを実行するのに役立つツールをご紹介します。

このコースを修了すると、通常の操作やトラブルシューティングにインターシステムズのドキュメントを読めばわかる程度の知識が身に付きます。

**※ドキュメントへのリンクが多い**

![](/assets/IRISSysBasics.png)

1. [はじめに](#1-はじめに)
2. [ローカル／クラウドへのインストール](#2-ローカル／クラウドへのインストール)
3. [InterSystems IRIS の構成](#3-intersystems-iris-の構成)
4. [セキュリティの構成と管理](#4-セキュリティの構成と管理)
5. [システムの監視](#5-システムの監視)
6. [ユーザとシステムプロセスの管理](#6-ユーザとシステムプロセスの管理)
7. [パフォーマンスとスケーラビリティの向上](#7-パフォーマンスとスケーラビリティの向上)
8. [システムの継続性を実現する方法](#8-システムの継続性を実現する方法)
9. [InterSystems IRISのアップグレード](#9-intersystems-iris-のアップグレード)
10. [システムのトラブルシューティング](#10-システムのトラブルシューティング)
11. [演習](#11-演習)

## 1. はじめに

- [ビデオ（英語）InterSystems Architecture Overview](https://learning.intersystems.com/course/view.php?name=Architecture%20Overview)

    《相談》開発系と一緒のビデオで以下の日本語ビデオで対応できそうだけど良いかどうか
    - [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)
        
        IRISの開発環境の作成方法、ネームスペース／データベースについて、IDEからIRISに接続する方法を確認できます。


- [ビデオ（英語）：Introduction to the Management Portal](https://learning.intersystems.com/enrol/index.php?id=1322)

- [ビデオ（英語）：Using the InterSystems Terminal](https://learning.intersystems.com/enrol/index.php?id=1433)

    Windows／Linuxで分けて説明あり。%Statusのエラーの取り方、エラーの表示方法も説明してる。
- [ビデオ（英語）:Integration overvide:Receiving and Routing Data in a Production](https://learning.intersystems.com/course/view.php?name=Interop%20QS)

    《相談》以下でも対応できると思うけどいいかどうか（日本語字幕付けたほうがいいかどうか）

    - ビデオ：[Interoperability概要](https://www.youtube.com/watch?v=vo12UnH-c-s&list=PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s)

    - シリーズ記事
    
        - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

        - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)

- [ビデオ（英語）を見るだけ:Exploring Multiple Data Models with Globals](https://learning.intersystems.com/enrol/index.php?id=2189)

    ビデオは日本語字幕あり


## 2. ローカル／クラウドへのインストール
InterSystems IRIS では、製品をインストールする場所を選択できます。InterSystems IRIS のインストール、インスタンスの起動と停止、基本設定、およびアプリケーションに必要な場合は Web サーバのインストール方法について説明します。

- [ドキュメント：導入](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=PAGE_deployment)

### コンテナ
InterSystems IRIS コンテナ・イメージから Docker コンテナ内にインストールする場合。

- [ビデオ（英語）:Docker Containers and InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=888)

    このビデオシリーズでは、Dockerコンテナとその用途を紹介し、InterSystems IRIS®データプラットフォームと組み合わせた場合に、いかに効果的であるかを紹介します。また、コンテナが継続的インテグレーション、継続的デプロイメント（CICD）アプローチにどのように適合するかもご覧いただけます。

    （ビデオ3つある。最後はICM）

    **《相談》日本の記事・ビデオで代用するなら以下。いいかどうか**
    - [コンテナとIRISのプレイリスト](https://www.youtube.com/watch?v=yY8BLUYp5IA&list=PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb)


- [ビデオ（英語）:Run InterSystems IRIS Community Edition Using Docker](https://learning.intersystems.com/enrol/index.php?id=1762)

    **《相談》コミュニティエディションなら以下記事＋ビデオでよい？**
    - [InterSystemsコンテナレジストリの使い方とコンテナ開始までの流れ（解説ビデオ付き）](https://jp.community.intersystems.com/node/545786)

- [ビデオ（英語）：Kubernetes Overview](https://learning.intersystems.com/enrol/index.php?id=1753)

    複数のホストにまたがるコンテナのデプロイをオーケストレーションするためのオープンソースプラットフォームであるKubernetesについてご紹介します。InterSystems Kubernetes Operatorにより、InterSystems IRIS®データプラットフォームのユーザは、InterSystems IRISアプリケーションのデプロイメントにおいてKubernetesのメリットを享受することができます。

    《相談》これはないので日本語字幕付けるでOKか

### ライセンス

- [ドキュメント：InterSystems IRIS ライセンスの構成](https://docs.intersystems.com/irislatestj/csp/docbookj/DocBook.UI.Page.cls?KEY=GSA_license_config)

- [ドキュメント：ライセンス・キーの有効化](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_license_update_key)

## 3. InterSystems IRIS の構成
最初のネームスペースとデータベースを設定し、それらが基礎となるデータ構造にどのように関係するかを学びます。次に、構成パラメータ・ファイル（CPF）、メモリ、およびアラートを構成します。

### システム

- [ドキュメント：InterSystems IRIS インスタンスの制御](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_using_instance_control)

- [ドキュメント：システム情報の構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_system)

- [ドキュメント：構成パラメータ・ファイルの概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=RACS_cpf)

- [コミュニティ：InterSystemsデータプラットフォームとパフォーマンス-パート4: メモリの確認 ](https://jp.community.intersystems.com/node/477746)

- [ドキュメント：Webゲートウェイ概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCGI_intro)

- [ビデオ（英語）：Configuring the InterSystems Web Gateway](https://learning.intersystems.com/course/view.php?name=ConfigWebGateway)

    《相談》日本語のトレーニング資料で古いのはある（KCCS用に作ったやつ）。ビデオに日本語字幕付けるか、既存資料を使って何か作るか

### ネームスペース

- [ドキュメント：ネームスペースとデータベース](https://docs.intersystems.com/iris20231/csp/docbookj/DocBook.UI.Page.cls?KEY=GORIENT_ch_enviro)

    オリジナルのURLパラメータ違う：https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GORIENT_enviro

- [ビデオ（英語）：Creating Namespaces and Databases](https://learning.intersystems.com/enrol/index.php?id=2124)

    《相談》日本ビデオなら以下に含まれているがいいかどうか

    - [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)


- [ドキュメント：ネームペースの構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_namespace)



### データベース

- [ドキュメント：ローカル・データベースの作成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_database_create)

- [ドキュメント：データベースの構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_databases)

- [ドキュメント：ローカルデータベースの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_databases)

## 4. セキュリティの構成と管理
セキュリティの構成と管理に役立つ製品内のツールと認証オプションを使用して、ユーザーとロールを設定します。

### 概要

- [ドキュメント：InterSystems IRIS セキュリティ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GORIENT_ch_security)

- [ビデオ（英語）：Users and Roles in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Users%20Roles%20IRIS)

    《相談》日本語字幕なし（付けてもいいかも）。

### セキュリティの設定と管理

- [ドキュメント：^SECURITY](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ASECCLI_security)

    将来このリンク Item Not foundで、2023.3配下
   https://docs.intersystems.com/iris20233/csp/docbook/Doc.View.cls?KEY=GSTU_seccli#GSTU_seccli_security

- [ドキュメント：サービス](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GAUTHN_services)

    概要と「使用可能なサービス」のみお読みください。

- [ドキュメント：暗号化データベースの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GENCRYPT_dbmgmt)

    概要と「暗号化データベースの作成」のみお読みください

    将来このリンク Item Not foundで、2023.3配下
    https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_encrypt_dbmgmt

    参考
    - [データベースの暗号化手順について](https://jp.community.intersystems.com/node/485826)

- [ドキュメント（クラリリファレンス）：Security.User　Export()](https://docs.intersystems.com/irislatest/csp/documatic/%25CSP.Documatic.cls?&LIBRARY=%25SYS&CLASSNAME=Security.Users#Export)

### 認証

- [ドキュメント：LDAP and InterSystems IRIS®](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GLDAP_overview)

    将来このリンク Item Not foundで、2023.3配下
    https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_iam_ldap

- [ドキュメント：2要素認証](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GAUTHN_twofactor)

    概要のみお読みください。

## 5. システムの監視
システムの健全性を監視し、潜在的な問題を早期に発見する方法を学びます。

>以下の文丸ごとなくす予定

System Alerting & Monitoring (SAM) について学びますが、Splunk や Datalog などの製品を使用してアラートをトリガーすることも可能です。

※ SAMはDeprecated

- [ドキュメント：^SystemPerformance を使用したパフォーマンスの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_systemperf)

    「^SystemPerformance ユーティリティの実行」のみお読みください。

- [ドキュメント:管理ポータルを使用したInterSystemsの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_dashboard)

- [ドキュメント：システム・モニタ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_healthmon_sysmon)

- [ドキュメント：データベースの詳細ページ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_databases_details)


※SystemPerformance を実行し、トラブルシューティングを実行しても問題が解決しない場合はインターシステムズのサポートセンターまでご連絡ください。

## 6. ユーザとシステムプロセスの管理
プロセス、ロック、ジャーナリングの管理について学習します。

- [ドキュメント：プロセス管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSTU_process)

    冒頭の紹介文のみお読みください

- [ドキュメント：ロックの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_locktable)

- [ドキュメント：システム全体での現在のロックの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_locktable_viewall)

    概要説明のみお読みください

    参考
    - [ロックテーブルの使用状況を簡単に確認する方法](https://jp.community.intersystems.com/node/495426)

    - [プログラム内でロック情報を取得する方法](https://jp.community.intersystems.com/node/484976)

    - [アプリケーションでロックタイムアウトエラーが発生する理由](https://jp.community.intersystems.com/node/493301)

- [ドキュメント：タスク・マネージャの使用](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_taskmgr)

    参考
    - [プログラミングでタスクスケジュールを登録・参照する方法](https://jp.community.intersystems.com/node/492746)

    - [タスクスケジュールを別環境にコピーする方法](https://jp.community.intersystems.com/node/494331)

    - [タスクの起動でエラーが発生した時にメールで通知する方法](https://jp.community.intersystems.com/node/518651)

- [ドキュメント：ジャーナリングの概要](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_overview)


- [ドキュメント：ジャーナリング処理タスク](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_tasks)

    参考
    - [ジャーナルファイルの使用量をチェックする方法](ジャーナルファイルの使用量をチェックする方法)

    - [ジャーナルファイルを削除する方法](https://jp.community.intersystems.com/node/501426)

    - [ジャーナルのON／OFFについて、コマンドで操作する方法を教えてください。](https://faq.intersystems.co.jp/csp/faq/result.csp?DocNo=276)

    - [グローバル単位でジャーナルのON/OFF設定する方法](https://jp.community.intersystems.com/node/508306)

    - [ジャーナルの整合性チェックやサマリの表示をコマンドで実行する方法](https://faq.intersystems.co.jp/csp/faq/result.csp?DocNo=582)

    - [ジャーナル圧縮機能について](https://jp.community.intersystems.com/node/537211)

    - [IRISジャーナル（z圧縮済み）をCachéにリストアする方法](https://jp.community.intersystems.com/node/542656)


## 7. パフォーマンスとスケーラビリティの向上
パフォーマンス・メトリクスを確認し、SQL クエリを特定して最適化します。次に、Enterprise Cache Protocol (ECP) がどのようにスケーラビリティを向上させるかを確認します。

### SQLパフォーマンスの最適化
- [ビデオ（英語）：Optimizing Your SQL Queries](https://learning.intersystems.com/course/view.php?id=1013)

    《相談》同じような内容の説明は過去のサミットにあるけど最古は2011年。個々にまとまってる👉[クエリをチューニングする方法](https://jp.community.intersystems.com/node/502256)

        この内容を自習用ビデオにしてもいいのかも？あえて作るかどうか

- [ドキュメント：SQLパフォーマンス分析ツールキット](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GSOE_profile#GSOE_profile)


### ECPを使用したスケーラビリティの実現

- [ドキュメント：分散キャッシュによるユーザ数に応じた水平方向の拡張](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSCALE_ecp)

- [記事：データプラットフォームとパフォーマンス-パート7 パフォーマンス、スケーラビリティ、可用性のためのECP](https://jp.community.intersystems.com/node/476811)

## 8. システムの継続性を実現する方法
ミラーリング、定期的なバックアップ、ジャーナリングによる高可用性の実装方法を学びます。

- [オンラインコース(英語）:Backup and Restore](https://learning.intersystems.com/course/view.php?name=Backup%20and%20Restore)

    InterSystems IRIS® データ・プラットフォーム・システムのバックアップとリストアの方法、および効果的なバックアップ戦略の設計について説明します。

    前提学習または経験：管理ポータルおよび InterSystems IRIS の一般的なアーキテクチャについての理解が必要です。
   
    学習目標 このコースを修了するまでに、以下のことができるようになります：

    - 外部バックアップ・ソフトウェアまたは仮想マシンのスナップショットを使用して、InterSystems IRIS 内をバックアップする利点と欠点を識別する。
    - サイトの効果的なバックアップ戦略を設計する
    - 外部ツールを使用したInterSystems IRISのバックアップとリストア

    >このオンラインコースは実際の演習は含まれてない。概要を確認するだけ

    《相談》この日本語欲しいかも（CSからもあったらいいなリストにバックアップ＆リストアの話が含まれているので、自習用ビデオ＋演習資料の公開があってもいいのかも＝トレーニングでやってるやつでいいならそれで）

- [InterSystems IRISミラーリング](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GHA_failover_mirror)

    《相談》三浦さんのビデオをここにリンクしてもいいのかも

    - [ミラーリングを使用したHAおよびDRの構成例](https://www.youtube.com/watch?v=sp5wfKbqHuQ&list=PLzSN_5VbNaxCeC_ibw2l-xneMCwCVf-Or&index=5&t=3s)


- [ドキュメント：ミラーの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GHA_mirror_monitor)

- [ドキュメント：ジャーナリングの構成](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_config)

## 9. InterSystems IRIS のアップグレード
アップグレード・ガイドおよびリリース・ノートを使用して、InterSystems IRIS をアップグレードします。

- [ドキュメント：インスタンスのアップグレード](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCI_upgrade_tasks)    

    このURL将来Item not found になる。対象はこれ？
    [Upgrading Overview](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GCI_overview)

- [InterSystems IRISコンテナのアップグレード](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ADOCK_iris_upgrading)

- [最新リリースノート(英語)](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=PAGE_release)


## 10. システムのトラブルシューティング
エラーの早期発見や問題の迅速なトラブルシューティングに役立つ多くのツールについてご紹介します。

- [ビデオ（英語）:Reviewing the Application Error Log](https://learning.intersystems.com/enrol/index.php?id=1131)

    参考（日本オリジナル）
    - [メッセージ・ログ(messages.log)／コンソール・ログ(cconsole.log) に出力される「Purging Application Error Logs」のメッセージとは](https://jp.community.intersystems.com/node/508271)

    - [アプリケーションのログを^ERRORSグローバルに入れる方法](https://jp.community.intersystems.com/node/508466)

    《相談》ビデオに翻訳つけるだけで足りるかどうか

- [ビデオ（英語）:Reviewing the Console Log and SYSLOG](https://learning.intersystems.com/course/view.php?id=1133)

    参考
    - [記事：SYSLOG - その正体と意味するもの](https://jp.community.intersystems.com/node/492146)

- [ドキュメント：InterSystems 診断レポートの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_diagnostic)

    概要のみお読みください

    参考（日本オリジナル）
    - [記事＋日本語ビデオ：【IRISベース】トラブル発生時の情報収集方法（IRIS ／ IRIS for Health ／ UCR 編）](https://jp.community.intersystems.com/node/489511)

    - [記事＋日本語ビデオ:【Caché ベース】トラブル発生時の情報収集方法（Caché ／ Ensemble ／ HealthConnect 編）](https://jp.community.intersystems.com/node/489516)

- [ドキュメント：irisstat ユーティリティを使用した InterSystems IRIS の監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_irisstat)

- [ドキュメント：緊急アクセス](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ASECMGMT_emerg)

※問題が解決しない場合は、必ず「診断レポート」を実行し、インターシステムズのサポートセンターまでお問い合わせください。

## 11. 演習
あなたのスキルを総動員して、基本的なシステム管理作業を実際にやってみましょう。

- [演習環境付きオンラインコース（英語）:Performing Common InterSystems IRIS Management Tasks](https://learning.intersystems.com/enrol/index.php?id=1945)

　《相談》これは何か日本語で同じことをできるように資料なり用意したいかも

## 12. 次は？
学習を継続する場合は以下のリソースが最適です。

- [ドキュメント：トラブルシューティングガイド](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GOPS_troubleshoot)
- [コミュニティ：「InterSystemsデータプラットフォームのキャパシティプランニングとパフォーマンス」シリーズの索引](https://jp.community.intersystems.com/node/477596)
- [講師付きトレーニング:InterSystems Serverシステム管理1](https://www.intersystems.com/jp/intersystems-server-system-administration/)


- [講師付きトレーニング:InterSystems Serverシステム管理2(セキュリティ管理編)](https://www.intersystems.com/jp/intersystems-server-system-administration-2/)
