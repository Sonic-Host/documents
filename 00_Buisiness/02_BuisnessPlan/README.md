# 事業計画書

本章では、Sonic-Host における事業計画書について記載する。  
※参考 https://j-net21.smrj.go.jp/startup/manual/list5/t5drrv0000007l9j-att/case3.pdf

## 企業概要

### 企業名等

|                  |                        |
| ---------------- | ---------------------- |
| **代表者名**     | 髙橋　勇人             |
| **企業名・屋号** | ※未決                  |
| **所在地**       | ※未決                  |
| **設立年月日**   | ※未決                  |
| **資本金**       | ※未決                  |
| **事業内容**     | ブログ提供基盤サービス |

### 経営者の略歴等

※後で記載

### 起業の動機

私は元々ブログを書いていたりしていた。  
その時に、ブログの内容自体より、ブログを高速化させる方法や
Google からの評価が高くなるような基盤設定にすることに凝り始めました。  
しかし、シンプルなレンタルサーバでは設定するべきことは多く、失敗も多発しました。  
そんな中、簡単に基盤レベルで高速化されたブログ基盤で Google から高評価されるようなものを提供できればと思いました。

## 事業内容

### ビジョン・目標

- 安全・高速・高評価のブログ基盤を提供したい
- 個人のスキル・知識を広めることにフォーカスできるようにしたい
- １年後に利用者（サブスク登録者数）１万人 (後述するが、競合が１年プラン・３年プランとかで安くすることでユーザを囲んでいるため、既存のブロガーはすぐに利用しないと予想)
  - ２年後に利用者 50 万人
  - 3 年後に海外展開含めて 300 万人
- 3 年間粗利益率 70%継続
- ブログサイトの可用性 99.999%を達成
  - 管理画面は 99.9%
- １年後の月間売上高 1200 万円
  - ２年後の月間売上高 6 億円
  - ３年後の月間売上高３６億円

### 事業コンセプト

#### サービス・商品の内容

WordPress 特価の超高速ブログ基盤提供サービス
内容：ローカル PC 上で作成したブログ記事のデータをアップロードしてもらうことで、ブログ記事のデータを抽出し、高速配布のサーバに配置。

#### ターゲット顧客

- ブログを始めたいが、基盤レベルの設定等が苦手な人
- 基盤レベルの設定にこだわってしまい、ブログ記事の執筆に集中できない人

##### ペルソナ

- 28 歳男性
- エンジニア
- 年収は７００万
- 副業で何かを始めたいと思い、ブログを開始している人
- マーケティングも学びたくてブログを始めたという思いもある
- その内転職をして見聞を広めたい

#### サービス・商品の提供方法・仕組み

- サイトから利用規約に同意し、登録してもらうことで提供開始
- 毎日１回アップロードされたブログデータを元にサイトを生成
  - ブログデータから HTML/CSS/JS を抽出し、CDN に保管
  - ユーザは参照するときに生成済みのファイルを CDN で取得可能
    - ユーザエージェント（端末情報）をもとに PC/スマホ・Android/iPhone 等を判定して最適なファイルを提供
- ブログの執筆をする際はユーザが持っている PC 上で WordPress を立ち上げて実施

### 現状分析

#### 業界のトレンド・市場規模

- SNS の台頭により、ブログよりはインスタなどに移りつつある
  - しかし、ブログは長期間残る情報として未だブロガーは多い。（ここら辺の数字は集めたい）
- 2019 年で日本の Web サイト数は９８００万 [参考サイト](https://wordpress-samurai.com/usewpsite_japan/)
  - WordPress のサイト数は 3420 万
  - 実稼働は２０％程？
- アクティブブログ数(最低月１更新のあるサイト)は横這いで 300 万サイト程 [参考サイト](https://yama-rock.com/blog-population/)

#### 競合の状況

ブログ基盤提供のサービスとして競合はいくつか存在する。  
基本的に競合となるのはいわゆるレンタルサーバを提供しているところになる。
基本的に利用期間が伸びれば伸びるほど安くなるプランになっている。

| サービス提供者       | 利用者数 | 料金      | 備考                                                                                 | サイト                                                                                                                                            |
| -------------------- | -------- | --------- | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| X-Server             | 230 万   | 990 円    | 3 つのプランに分かれてる。平均 1500 円位してそう。                                   | [Xserver 料金](https://www.xserver.ne.jp/price/)                                                                                                  |
| Lolipop              | 170 万   | 1100 円   | Wordpress 利用満足度 No.1 をうたってる。なんかいろいろオプションをつけるともっと高い | [Lolipop 料金](https://lolipop.jp/pricing/)                                                                                                       |
| Conoha Wing          | 　 50 万 | 1320 円   | パックで色々セットにしてユーザを離さないようにしている。                             | [Conoha Wing 料金](https://www.conoha.jp/wing/pricing/?btn_id=wing-winterbonus2022--wingHeader_wing-pricing)                                      |
| さくらレンタルサーバ | 45 万    | 　 425 円 | 普通に安くね？？しかし、色々サーバ設定がざるだったり、性能的に遅いみたい。           | [さくらレンタル 料金](https://rs.sakura.ad.jp/?gclid=CjwKCAiA2L-dBhACEiwAu8Q9YJCXKBM6NidDMDSHNn5opkUb8-SrYBsiDy8iN_bBBq1X_76QPzYipBoCnKIQAvD_BwE) |

#### 自社の強み・優位性

- 基盤レベルの設定がほとんど必要ない
  - 設定が必要なのはドメインの設定のみ
  - HTTPS による通信の暗号化・キャッシュ化・ファイル圧縮等は自動で設定
- 事前に HTML/CSS/JS を生成しているため、ブログの表示が早い
- サーバ上に管理画面の情報がないため、乗っ取りによるリスクなどがない
  - ローカルの PC がウィルスに侵されたらアウトだが、それはレンタルサーバでも同じ

### 販売・仕入れ計画

#### 販売計画

| 営業年数 | 売上高（年） | 会員数   | 単価    |
| -------- | ------------ | -------- | ------- |
| 1        | 2880 万      | 1 万人   | 1200 円 |
| 2        | 14 億４千万  | 50 万人  | 1200 円 |
| 3        | 86 億４千万  | 300 万人 | 1200 円 |

**計算式**  
売上高 = 会員数　 × 　単価　 × 　 12(１年) × 0.2

#### 販売促進・集客方法

- ブロガー対象なのでアフィリエイトへの掲載
  - ブロガーたちにアフィリエイトへ記載するために実際に体験してもらう
  - ブロガーのネットワークは強力なので、その口コミを狙う
- 今のブログを実際に適用したらどうなるかを体験してもらう
  - ドメインを指定してもらったら、そのサイトの複製を仮ドメインで３時間くらい表示してあげる機能
- SNS/ブログを用いた発信。
  - SNS としては Twitter が活発なので、Twitter を検討。
  - ブログはブログについてを発信するサイトとして掲載していく

## 数値計画

### 投資・調達計画

| 投資(必要な資金) | 金額                                            | 調達方法 |
| ---------------- | ----------------------------------------------- | -------- |
| サーバー費用     | １年目 115 万                                   | 売上     |
| 人件費           | ※お知らせ運営や、ブログ運営、問い合わせ対応など |
| 広告費用         | 　※ASP 費用                                     |
| **合計**         |

### 損益計画

## 実施スケジュール