# 開発者向けInterSystems IRIS の管理

> オリジナル:[Managing InterSystems IRIS for Developers](https://learning.intersystems.com/course/view.php?id=1971)

InterSystems IRIS® データプラットフォームとその他のインターシステムズ製品の管理の基本について、ハイレベルな概要を学びます。このラーニング・パスは、システム管理者以外の方で、システム管理タスクの基本的な知識が必要な方を対象としています。
システム管理者向けのより包括的な学習パスについては、[InterSysetms IRIS 管理の基本](/IRISManagementBasics.md)を参照してください。

![](/assets/ManagingIRISforDeveloper.png)

1. [はじめに](#1-はじめに)
2. [セキュリティ管理](#2-セキュリティ管理)
3. [ログの監視](#3-ログの監視)
4. [高可用性の維持](#4-高可用性の維持)

## 1. はじめに
InterSystems IRISのアーキテクチャと、システム管理に役立つツールについてご紹介します。

- [ビデオ（英語）InterSystems Architecture Overview](https://learning.intersystems.com/course/view.php?name=Architecture%20Overview)

    開発系と一緒のビデオで以下の日本語ビデオで対応できそう
    - [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)
        
        IRISの開発環境の作成方法、ネームスペース／データベースについて、IDEからIRISに接続する方法を確認できます。


- [ビデオ（英語）：Introduction to the Management Portal](https://learning.intersystems.com/enrol/index.php?id=1322)

- [ビデオ（英語）：Using the InterSystems Terminal](https://learning.intersystems.com/enrol/index.php?id=1433)

    Windows／Linuxで分けて説明あり。%Statusのエラーの取り方、エラーの表示方法も説明してる。

## 2. セキュリティ管理

ユーザーを作成し、対応するロールに接続することで、必要なものにはロールベースでアクセスできるようにし、ロールに関係のないデータやツールへのアクセスを禁止します。次に、データベースを暗号化することで安全なデータを確保する方法をご覧ください。

- [ビデオ（英語）：Users and Roles in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Users%20Roles%20IRIS)

    日本語字幕なし（付けてもいいかも）

- [演習環境付き演習（英語）:Configuring Role-Based Access](https://learning.intersystems.com/enrol/index.php?id=2157)

    演習の例では、管理ポータルで使用する 2 種類のマネージャ・ロールの設定方法を示しています。最初のロールは、ユーザ定義やロール定義などのセキュリティ関連項目の変更を許可するページにアクセスできます。2つ目のロールにはそのようなアクセス権はありません。また、これらのロールを持つユーザが管理ポータルとどのようにやり取りするかも説明します。なお、LDAP もサポートされていますが、この演習では取り上げません。

- [ドキュメント：Encryption](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_encrypt)

    オリジナルがリンク切れ（元：https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GENCRYPT）

## 3. ログの監視
ログを使用してエラーを早期に特定し、問題をトラブルシューティングする方法をご覧ください。

- [ビデオ（英語）:Reviewing the Application Error Log](https://learning.intersystems.com/enrol/index.php?id=1131)

    参考
    - [メッセージ・ログ(messages.log)／コンソール・ログ(cconsole.log) に出力される「Purging Application Error Logs」のメッセージとは](https://jp.community.intersystems.com/node/508271)

    - [アプリケーションのログを^ERRORSグローバルに入れる方法](https://jp.community.intersystems.com/node/508466)

- [ビデオ（英語）:Reviewing the Console Log and SYSLOG](https://learning.intersystems.com/course/view.php?id=1133)

    参考
    - [記事：SYSLOG - その正体と意味するもの](https://jp.community.intersystems.com/node/492146)

- [ドキュメント：InterSystems 診断レポートの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_diagnostic)

    概要のみお読みください

    参考
    - [記事＋日本語ビデオ：【IRISベース】トラブル発生時の情報収集方法（IRIS ／ IRIS for Health ／ UCR 編）](https://jp.community.intersystems.com/node/489511)

    - [記事＋日本語ビデオ:【Caché ベース】トラブル発生時の情報収集方法（Caché ／ Ensemble ／ HealthConnect 編）](https://jp.community.intersystems.com/node/489516)


## 4. 高可用性の維持
冗長性と自動監視を組み込むことで、システムを効果的に稼働させ続ける方法を学びましょう。

- [オンラインコース(英語）:Backup and Restore](https://learning.intersystems.com/course/view.php?name=Backup%20and%20Restore)

    InterSystems IRIS® データ・プラットフォーム・システムのバックアップとリストアの方法、および効果的なバックアップ戦略の設計について説明します。

    前提学習または経験：管理ポータルおよび InterSystems IRIS の一般的なアーキテクチャについての理解が必要です。
   
    学習目標 このコースを修了するまでに、以下のことができるようになります：

    - 外部バックアップ・ソフトウェアまたは仮想マシンのスナップショットを使用して、InterSystems IRIS 内をバックアップする利点と欠点を識別する。
    - サイトの効果的なバックアップ戦略を設計する
    - 外部ツールを使用したInterSystems IRISのバックアップとリストア

    >このオンラインコースは実際の演習は含まれてない。概要を確認するだけ

    この日本語欲しいかも（CSからもあったらいいなリストにバックアップ＆リストアの話が含まれているので、自習用ビデオ＋演習資料の公開があってもいいのかも＝トレーニングでやってるやつでいいならそれで）

- [The Value of System Alerting & Monitoring (SAM)](https://learning.intersystems.com/course/view.php?id=1496)

    Deprecatedだからいらないかも