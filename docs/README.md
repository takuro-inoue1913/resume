# 職務経歴書

## 基本情報

- Name: **井上 拓郎**
- Birth: **1988/01/18**
- Age: **37**
- Address: **東京都**
- X (旧 Twitter): [https://twitter.com/takutaku1913](https://twitter.com/takutaku1913)
- Qiita: [https://qiita.com/takutaku1913](https://qiita.com/takutaku1913)

## 技術スタック

- バックエンド 2 年
- フロントエンド 5 年

### 言語

- JavaScript
- TypeScript
- PHP
- Go
- ruby

### フレームワーク・その他

- Node.js
  - React.js
  - Vue.js
  - Next.js
  - Nuxt.js
- PHP
  - BEAR.Sunday
  - Laravel
- Rails

## エンジニアになってからの経歴

### 株式会社ブルーイッシュ （2020/08 〜 2022/03） 正社員

#### 使用言語やツール

- フロントエンド： React, TypeScript
- バックエンド： PHP, SQL, BEAR.Sunday, Laravel
- SQL クライアントツール： TablePlus
- バージョン管理ツール： GitHub
- スケジュール管理ツール： Notion
- コミニケーションツール： Slack

#### 関わった開発

サービス： [aipass](https://aipass.jp/)

- **ホテルの客室スケジュール管理用のカレンダー作成**

  宿泊管理システムに日付ごとに客室を管理する Google カレンダーの機能を備えた UI を作成しました。

  カレンダーを一から実装したため、API から取得したデータをカレンダーに適用させるのが苦労しましたが、カレンダー用のマトリックスを設計し、さまざまなレスポンスデータを想定しカレンダーに組み込みを行いました。

- **スマホで事前チェックイン、チェックアウト時に手軽に宿泊料金を支払える決済機能を実装**

  決済システムを提供しているベリトランスの PHP モジュールを現在の宿泊管理システムにライブラリーとして組み込み、各 API で使えるように実装を行いました。

  宿泊管理システムでの外部のモジュールを利用するケースは今回が初めてでしたのでノウハウがまだなく、根本的なプロダクトの設計レベルでのスタートでしたが、上司や他の開発メンバーとの MTG を定期的に実施し、最終的に今後も色々な決済機能に対応できる汎用性のある実装に仕上げることができました。

- **リモートロックの API を用いた客室鍵番号のリモート管理機能の開発**

  リモートロックのデバイスを設置した施設向けに、[リモートロック](https://remotelock.kke.co.jp/?utm_source=google&utm_medium=cpc&utm_campaign=Google%E6%A4%9C%E7%B4%A2-%E5%9B%BA%E6%9C%89%E5%90%8D%E8%A9%9E&utm_term=%E3%83%AA%E3%83%A2%E3%83%BC%E3%83%88%E3%83%AD%E3%83%83%E3%82%AF&hsa_acc=1744005690&hsa_cam=1602296873&hsa_grp=65951954283&hsa_ad=379417145900&hsa_src=g&hsa_tgt=kwd-323757690915&hsa_kw=%E3%83%AA%E3%83%A2%E3%83%BC%E3%83%88%E3%83%AD%E3%83%83%E3%82%AF&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gclid=Cj0KCQjw0oyYBhDGARIsAMZEuMvsthxDk1NaUIxV8RHh2puaQ4WuOQq-uaBpEExe9FxES0nReAgOrvIaAq8wEALw_wcB)の API を宿泊管理システムの API に組み込み、客室を操作するタイミングで鍵番号を自動で操作できる機能を作成しました。

  「ホテルの客室スケジュール管理用のカレンダー」にもこの鍵番号自動操作の機能を組み込む必要があったため、カレンダー機能とリモートロック API の仕様をどううまく連携させるか悩みましたが、リモートロック API ドキュメントを設計段階で確認し、今回要件に使えそうな API を洗い出してそれから API 設計を行なったことでスムーズに実装を進めることができました。

- **外部の予約システムと宿泊管理システムの予約管理との連携機能開発**

  外部の予約システムである[TL リンカーン](https://www.seanuts.co.jp/product/lincoln/)や[ねっぱん！](https://www.neppan.com/)などから API 等で予約情報や客室在庫状況を取得し、宿泊管理システムの予約用にデータを変換して自動で予約情報や在庫情報を連携できるような機能を作成しました。

  外部予約サービスを複数取り込む必要があったため、予約システムごとに独自の仕様が存在したり、同じ仕様に見えても状況によっては違う挙動を見せたりとそれぞれのサービスの全体の仕様を把握するのに非常に大変な思いをしましたが、クライアント側と開発側で協力して念入りに検証・テストを繰り返し、また外部の予約システムの担当者に直接連絡を取って都度仕様を確認したりした結果、少しずつではありましたが不具合などを 1 つ 1 つ潰していくことが出来ました。

### 株式会社マネーフォワード （2022/05 〜 2024/03） 正社員

#### 使用言語やツール

- フロントエンド： React, TypeScript
- バックエンド： Rails
- バージョン管理ツール： GitHub
- スケジュール管理ツール： Asana
- コミニケーションツール： Slack

#### 関わった開発

サービス： [マネーフォワードクラウド](https://biz.moneyforward.com/)

- **既存のクラウド会計システムをインボイス対応に向けて React でリニューアル作業**

  2023 年 10 月から開始されたインボイス対応に向けて、既存のクラウド会計システム各機能をインボイス対応可能な状態にリニューアル作業を行いました。

  対応方法としては、既存実装を修正する形だけではなく、フロントエンド側は一部 React のコンポーネントとして部品化する作業を行いました。
  もともと Rails のみで構成されており、作業中には 8 年前のコードを触る機会もしばしばありました。また、React でのリニューアル作業は初めてだったことから設計方針が明確に定まっていない状況でしたが、既存のコードを読み込みながら少しずつコンポーネント化していくことで、既存のコードを壊さずにリニューアル作業を進めることが出来ました。

  また、他のチームメンバーと開発していくうちに、コンポーネント化する際の設計方針やコーディング規約などを皆で話し合いながらお互いの認識を合わせることの重要性を学びました。
  こだわりが強めのメンバーもいたため、コーディング規約の話し合いはなかなか難航しましたが、「この人が本当に大切にしているところはどこだろう」と常に模索しながら話し合いを進めていき、議題に対してしっかりとした落とし所を決めることを心がけました。

  実装だけではなくレビュアとしても貢献できるように、コードレビューを行う際にはレビューする側の立場になって、レビューされる側がどのような気持ちでコードを書いているのかを考えながらレビューを行いました。特に意識したことは、「どのレビュアよりも丁寧にレビューをする」です。どうしてもレビューは冷たい印象を受けやすい傾向があると思うので、レビューを受ける側の経験や実装内容に関わらず、謙虚な姿勢を心がけました。

- **既存のクラウド会計システムの設計見直し、保守性向上に向けての取り組み**

  クラウド会計はマネーフォワードの中でも一番歴史があるサービスになっており、売り上げも大きいのですが、その分コードの量も多く、コードも全体的にレガシーになっており保守性が低い状態でした。そこで、保守性を向上させるために、既存のコードを見直し、設計を見直す作業を行いました。

  具体的には、まずは Rails View で構成されている部分を積極的に React に置き換えていくことで、UI 側のみで動作できる環境を増やしていき、それと合わせてユニットテスト、インテグレーションテストの実装、storybook の導入を行い、テストカバレッジを上げていきました。また、既存のコードを見直す際には、コードの重複をなくすために共通化を行ったり、コードの見通しを良くするためにリファクタリングを行ったりしました。

  また、React 側の構成に関しても、現在の状況で一番良いディレクトリ構成が最適なのかをチームメンバーと念入りに議論し合い、設計の方向性を統一することで、チームメンバーごとに設計方法が異なってしまうことを防ぎました。

- **2024 年 06 月執行のクラウド会計料金改定に向けた対応**

  クラウド会計の各プランに対して、全体的な見直しのタイミングがあり、そのプロジェクトに参画させていただきました。
  プラン情報は自社で作っている他のプロダクトに密接に関係していたり、さらに別軸で同時進行しているプロジェクトとの競合もあるなど、非常に複雑なプロジェクトでした。

  そのため、プロジェクトの進行にあたっては、常に互いのロードマップを共有し合い、どのプロジェクトがどのタイミングでどのような影響を及ぼすのかを常に意識しながら進めていきました。
  また、執行前まで現状のユーザーに対しての影響を及ぼさないように、料金改定フラグなどを導入し、それに合わせて各機能の実装を行いました。

  また、影響範囲が広いことから料金改定のコンテキストがかなり広くなってしまっていたので、仕様が完全に固まっていない状況での実装も多かったですが、先にプロトタイプを作成し、それをデザイナーや PM と共有しながら仕様を固めていくことで、イメージを体感してもらい、フィードバックをもらいながら実装を進めることができました。

### 株式会社 ZEST （2022/09 〜 2024/08） 業務委託

#### 使用言語やツール

- フロントエンド： Vue.js, TypeScript
- バックエンド： .NET Core
- バージョン管理ツール： GitHub
- スケジュール管理ツール： Notion
- コミニケーションツール： Slack

#### 関わった開発

サービス： [ZEST](https://zest.jp/)

- **新スケジュール管理画面の開発**

  Join した頃に既存のスケジュール管理画面をリニューアル作業が行われていましたので、その引き継ぎ作業を行いました。
  ベンチャー企業であることから、保守性よりも開発スピードを上げることを重点においていたため開発環境の整備がまだ行き届いていない状況でした。そのためバグが発生した際に原因を特定するのに苦労したり、開発環境の構築に時間がかかってしまったりといったことがありました。しかし、途中段階だった TypeScript の導入や eslint ルールの見直し等を積極的に行い、開発環境の整備を進めていきました。
  結果、バグの特定や開発環境の構築にかかる時間が短縮され、開発スピードが上がったと感じています。

  また、自分が入る前の実装箇所にバグがあった場合は、表面的な修正だけではなく、そのバグが発生した根本原因を特定し、その原因をなくすための修正を行うように心がけました。そしてその原因に対して、プルリクエストの Description に詳細な説明を書くことで、他のチームメンバーにもその原因を共有できました。
  さらに、修正の際にはテスト駆動開発を積極的に取り入れ、修正以外の箇所に影響が出ないように心がけました。

  また、PdM や CS チームの方々とのコミュニケーションを積極的に行い、認識の相違がないようにすることやユーザーのニーズを把握しながら開発を進めることを意識しています。結果、業務委託で関わる時間も少ないのにも関わらず、一緒に働くメンバーとも信頼関係を築くことができているし、これからも一緒に働きたいと感じています。

### BizteX 株式会社 （2024/04 〜 現在） 正社員

#### 使用言語やツール

- フロントエンド： React, TypeScript
- バックエンド： Rails, Go
- バージョン管理ツール： GitHub
- スケジュール管理ツール： GitHub ZenHub
- コミニケーションツール： Slack

#### 関わった開発

サービス： [BizteX Connect](https://service.biztex.co.jp/connect/)

- **iPaaS プロダクト開発**

  BizteX Connect は SaaS サービスと SaaS サービスを連携させ、業務効率化を図ることができるサービスであり、そのため、他社の API 仕様を理解し、それを使って連携機能を実装することが求められました。

  フロントエンド開発では、ある程度決まった UI を用意するのではなく、いろいろな SaaS サービスの API 仕様に合わせて UI を作成する必要があり、
  汎用性や再利用性のあるコンポーネントの設計が求められました。また、そのためにプロダクトの基盤となる仕様を考えることが重要でした。
  上記を達成するため、 storybook を導入して UI テストを充実させ、コンポーネントの再利用性を高めることを意識しました。

  また、既存のリポジトリでは、四年前からの設計から変わっておらず、最新の React でのやり方やベストプラクティスに準じていない部分が多かったため、それらを一掃して再設計を行い、コードの品質を向上させることを行いました。
  ライブラリ周りも最新のものにアップグレードし、コードの品質を向上させるために、 eslint や prettier, stylelint の設定を見直したことで、コードの品質を向上させることができました。

  また、今回は積極的にバックエンド開発にも関わることができ、Go や Rails を用いて、フロント側に必要な GraphQL サーバーを実装することができました。中には AWS の Pub/Sub メッセージング を使用した実装も行い、バックエンドの知識を深めることができました。

### シェルパ・アンド・カンパニー株式会社 / Cierpa ＆ Company, Inc. （2024/06 〜 現在） 業務委託

#### 使用言語やツール

- フロントエンド： React, TypeScript
- バックエンド： AWS Amplify
- バージョン管理ツール： GitHub
- スケジュール管理ツール： Jira
- コミニケーションツール： Slack, Notion

#### 関わった開発

サービス： [SmartESG](https://smartesg.jp/)

- **ESG プラットフォーム開発**

  SmartESG では、ESG（環境、社会、ガバナンス）に関する情報を収集し、分析するプラットフォームを開発しています。
  ESG 情報開示をするためにさまざまなフォーマットの質問に対して回答をする必要があるため、その分仕様も複雑化しやすいですが、ドメイン知識や仕様を理解し、それを実装に落とし込むことが求められました。

  おもにフロントエンド開発を担当しており、React を用いて、さまざまな要求に対して柔軟に対応できるような UI を作成しています。
  また、バックエンドに AWS Amplify を使用しているため、db schema の設計や GraphQL の設計も行い、フロントエンドとバックエンドの連携を密に行いながら開発を進めています。

## 自分の強みだと思っていること

- 実装や日々のコミュニケーションも含め、常に丁寧な仕事を心がけています。確かにいいコード、美しいコードを書くのは良いことですが、それがユーザーにとって本当に必要なものなのか、また、自己満になっておらずチームメンバーにとっても理解しやすいコードなのかを常に考えながら開発を行っています。そのため、認識のすり合わせや実装に時間がかかってしまうこともありますが、その分、ユーザーにとって本当に必要な機能を提供できるようになると考えています

- エンジニアになる前は板前として 10 年以上働いてきた経験から、自分の仕事に集中するだけではなく周りを気遣いながら作業を行うことが出来ます。また、板前では厳しい修行を行なってきたおかげで、技術に対する貪欲さ、忍耐力や精神力は人並み以上に高い自信はあります。ただ、技術を極めるだけではなく、どちらかというとチームメンバーとのコミュニケーションを大切にし、一緒に働くメンバーをサポートできるようなエンジニアになりたいと考えています

- 新しい技術・あらためて学び直す必要がある技術は自然と興味が湧くほうでして、気になったらサンプルをダウンロードして試してみたりしています。既存の知識にこだわることなく新しい技術を取り入れることで開発スピードを上げることができると考えています

- プログラムを書くことがとても楽しいと感じており、仕事が一部の趣味となっています。ここまで自分がエンジニアになることを楽しめるとは思っていなかったので、これからも楽しみながらエンジニアとして働いていきたいと思っています

- 「ものづくり」が好きなことは個人的にはいちばんの強みだと感じています。エンジニアになる前は長年板前としてお客さんが喜んでくれる料理を作ってきましたし、エンジニアになった今でも自分が関わったプロダクトで使ってくれるユーザーが喜んでくれる機能を色々考案したり、作ったりすることに喜びを感じます。これからも自分が関わったプロダクトでユーザーが喜んでくれるものを作っていきたいと思っています

## 今後の目標

- 今よりさらに技術や知識を身につけ、今後技術顧問として開発をサポートしたり、チームメンバーのマネジメントできるエンジニアになっていきたいと思っています

- もともと板前をやってたので、自分も料理業界に対してエンジニアとして貢献できるようになっていきたいです
