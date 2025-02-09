# AWS Fargate

## 概要
Fargateはコンテナのデプロイや管理を行うことができる。インスタンスの管理やインフラの管理は不要である。


## 主な特徴
- **ディベロッパーを意識したコンテナ実行**：サーバーのクラスタのプロビジョニングやパッチ適用が不要となっている。
- **ECSとEKSのサポート**：コンテナを実行するために、ECSとEKSを選択することができる。
- **従量課金**：コンテナのCPUやメモリの使用量に比例して、課金計算がされる。

## ネットワーク周り
- **VPCとの連携**：Fargateは定義されたVPC内で実行される。★EC2だと違う？
- **ALBとNLBのサポート** :ALBとNLBの両方をサポートしている。
- **タスクレベルのネットワークサポート** :エラスティックネットワークインターフェースを専用のVPCサブネットから実行中のタスクから直接割り当てることができる。セキュリティグループの割り当てやネットワークモニタリングがコンテナレベルで実施することができる。

## ユースケース
- アプリケーションを