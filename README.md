# このリポジトリについて

設計書を格納するリポジトリ。  
基本設計レベルのドキュメントを格納していく予定

## 設計書の種類

- シーケンス図（PlantUML）
- API 仕様書（Swagger）
- 画面遷移図（Figma）
- AWS 構成図（draw.io を予定）

## シーケンス図について

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
