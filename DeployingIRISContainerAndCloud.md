# InterSystems IRIS のコンテナとクラウドへの展開

オリジナル：[Deploying InterSystems IRIS in Containers and the Cloud](https://learning.intersystems.com/enrol/index.php?id=2141)

スケーラブルなデプロイメント戦略を使用して、InterSystems IRIS® データプラットフォームの実装に信頼性を追加します。このラーニング・パスでは、InterSystems IRIS のクラウドおよびコンテナベースのデプロイメントを作成する方法を説明します。まず、システムとデプロイメントの仕様の概要を説明します。次に、デプロイメントの例を確認し、自分のシステムに最適なアプローチを決定します。

![](/assets/ContainerAndCloud.png)

1. [システムとデプロイの仕様概要](#1-システムとデプロイの仕様概要)
2. [クラウドとコンテナのデプロイオプションに慣れる](#2-クラウドとコンテナのデプロイオプションに慣れる)
3. [スケーリングと自動化のためにコンテナを使用する](#3-スケーリングと自動化のためにコンテナを使用する)
5. [InterSystems Kubernetes Operator によるデプロイ](#5-intersystems-kubernetes-operator-によるデプロイ)

## 1. システムとデプロイの仕様概要

クラウドまたはコンテナへの InterSystems IRIS のデプロイの準備として、システムとデプロイに必要な内容を一覧します。

以下、[Job Aid: Define system requirements and deployment specifications (5m)](https://learning.intersystems.com/mod/page/view.php?id=13225)に書かれてる内容

### システム要件
InterSystems IRIS の新規導入を開始する際には、以下のようなシステム要件の詳細な説明を作成してください：

- システム・ユーザの数と開発者や管理者などの役割
- 接続する外部システムの数
- 想定されるデータベース・サイズとデータ・フロー量
- サーバーの可用性ニーズ

### デプロイの仕様
次に、いくつかの重要な技術的質問に答えながら、デプロイの仕様を作成します：

- 何台のインスタンスが必要で、どこに配置するのか？
- 各インスタンスに必要なデータベースと機能は何か。
- どの程度までデプロイを自動化しますか?
- 将来のアップデートはどのように計画するのか？
- インストールにどのようなサードパーティソフトウェアを使用しますか？
- 実装ではシャーディングを使用しますか？
- 実装ではミラーリングを使用しますか？

## 2. クラウドとコンテナのデプロイオプションに慣れる

InterSystems IRIS をコンテナやクラウドに導入するための戦略をご紹介します。

- [ビデオ（英語）:Tools for Running and Deploying InterSystems Containers](https://learning.intersystems.com/course/view.php?id=1751)

    InterSystems IRIS® データ・プラットフォームで利用可能なデプロイメント・ツールについて学ぶことで、ニーズに合ったコンテナ・ベースのシステムを設計することができます。

    このビデオでは
    - コンテナと Docker の基本を確認します。
    - InterSystems IRIS 組み込みの 2 つのデプロイ機能、永続的な %SYS と構成のマージについて学びます。
    - 2つの自動デプロイメント・プラットフォームの利点を紹介します：InterSystems Cloud ManagerとInterSystems Kubernetes Operator。

    **日本の記事・ビデオで代用するなら以下？**
    - [コンテナとIRISのプレイリスト](https://www.youtube.com/watch?v=yY8BLUYp5IA&list=PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb)

        ここにはマージCPFに触れてるものはないかも

    ― [KubeernetesとIRISのプレイリスト](https://www.youtube.com/watch?v=yKX8wB9d2cs&list=PLzSN_5VbNaxC2mfu1cYvn9pfbJRs7xtkk)


## 3. スケーリングと自動化のためにコンテナを使用する

- [ビデオ（英語）:Docker Containers and InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=888)

    このビデオシリーズでは、Dockerコンテナとその用途を紹介し、InterSystems IRIS®データプラットフォームと組み合わせた場合に、いかに効果的であるかを紹介します。また、コンテナが継続的インテグレーション、継続的デプロイメント（CICD）アプローチにどのように適合するかもご覧いただけます。

    （ビデオ3つある。最後はICM）

    **日本の記事・ビデオで代用するなら以下？**
    - [コンテナとIRISのプレイリスト](https://www.youtube.com/watch?v=yY8BLUYp5IA&list=PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb)


- [ビデオ（英語）:Run InterSystems IRIS Community Edition Using Docker](https://learning.intersystems.com/enrol/index.php?id=1762)

    **コミュニティエディションなら以下記事＋ビデオでよい？**
    - [InterSystemsコンテナレジストリの使い方とコンテナ開始までの流れ（解説ビデオ付き）](https://jp.community.intersystems.com/node/545786)



## 4. Deploy with InterSystems Cloud Manager

    ICMはDeprecatedなのでラーニング・パスから外したほうがいいのでは？（リタイヤリスト：https://usconfluence.iscinternal.com/display/OLT/Retired+Online+Content　には古いICMの演習は含まれてるけどここで紹介している内容は含まれていない）

## 5. InterSystems Kubernetes Operator によるデプロイ

- [ビデオ（英語）：Kubernetes Overview](https://learning.intersystems.com/enrol/index.php?id=1753)

    複数のホストにまたがるコンテナのデプロイをオーケストレーションするためのオープンソースプラットフォームであるKubernetesについてご紹介します。InterSystems Kubernetes Operatorにより、InterSystems IRIS®データプラットフォームのユーザは、InterSystems IRISアプリケーションのデプロイメントにおいてKubernetesのメリットを享受することができます。

- [ビデオ（英語）：Deploying and Upgrading InterSystems IRIS with the InterSystems Kubernetes Operator](https://learning.intersystems.com/enrol/index.php?id=1656)

    InterSystems Kubernetes Operator を使用して Kubernetes クラスターを拡張する方法、および InterSystems IRIS® データプラットフォームインスタンスをデプロイ、アップグレード、拡張する方法をご覧ください。

- [演習環境付き演習（英語）：Achieving High Availability with InterSystems IRIS and Kubernetes](https://learning.intersystems.com/enrol/index.php?id=1962)

    KubernetesをInterSystems IRIS®データプラットフォームと組み合わせて使用することで、デプロイメントで高可用性を実現する方法をご覧ください。この演習では、クラスタをデプロイし、災害シナリオをシミュレートし、Kubernetesがどのようにデータ損失とダウンタイムを防止するかを学びます。

    >この演習環境を開始すると4ノード　Readyのステータスでできた状態のUbuntuが立ち上がる。kubectlでpod作る、deployするなどの操作が試せる

**上記内容以下ビデオ2個で補えないか？**
[プレイリスト：KubernetesとInterSystems製品](https://www.youtube.com/playlist?list=PLzSN_5VbNaxC2mfu1cYvn9pfbJRs7xtkk)