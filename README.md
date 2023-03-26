# このリポジトリについて

設計書を格納するリポジトリ。  
基本設計レベルのドキュメントを格納していく予定

## 設計書の種類

- シーケンス図（PlantUML）
- API 仕様書（Swagger）
- 画面遷移図（draw.io）
- AWS 構成図（draw.io を予定）

## シーケンス図

PlantUML については [workFlow](./.github/workflows/plantuml-diagram.yaml) で自動的に SVG が作成される。
そのため、下記にて記載される手順にてシーケンスを作成することが推奨される。

### 作成手順

1. plantUML を.pu ファイルで作成
2. Readme.md を作成
3. Read.me の中で相対パスで.svg ファイルを参照(ファイル名は.pu と同じファイル名)
4. 変更内容を確認し、git push
5. github 上の Readme で正しくシーケンスが見れるか確認

### サンプル

会員登録フローのサンプルは[こちら](./01_Sequences/01_Registeration_Flow/Readme.md)を参照

## 画面遷移図

[draw.io](https://app.diagrams.net/)で作成した SVG ファイルを画面遷移図とする。  
生成した SVG ファイルを Readme に貼り付けることで Github 上でも参照可能にする。

### サンプル

クライアントアプリの画面遷移図は[こちら](./02_screenTransition/01_clientApplication/Readme.md)

## API 仕様書

[stoplight](https://sonic-host.stoplight.io/studio/documents:develop) で作成した OpenAPI の Yaml ファイルを API 仕様書とする。  
API 仕様書を元に`workflow`で`API-GW`にて直接読み込みが可能となる Swagger ファイルを生成する。

### サンプル

作成された API 仕様書については以下の通り

- [クライアントアプリ用](./05_API_Interface/endpoint/ClientAPIInterface.yaml)
- [公開ドメイン用](./05_API_Interface/endpoint/publicAPIInterface.yaml)
- [管理画面用](./05_API_Interface/endpoint/AdminAPIInterface.yaml)
