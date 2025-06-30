# Sigma日本語ドキュメント 構成案

---

## 【第1部：Sigmaの基本】

### 第1章：はじめに (Get Started)
- **1-1. Sigmaについて (About Sigma)**
  - *主な参照先：ワークブックの基本、データセットの基本*
- **1-2. ワークブックの基本 (Workbook Basics)**
  - *主な参照先：データ探索、フィルタ、チャート作成*
- **1-3. クイックスタート (Quickstart: Analyze Your Data in 10 Minutes)**
  - *主な参照先：このチュートリアルで触れる全ての機能の詳細ページ*

---

## 【第2部：データモデルの構築】

### 第2章：データへの接続 (Connect to Data)
- **2-1. データソースへの接続**
  - *主な参照先：各データベース固有の認証情報や設定*
- **2-2. 接続の管理**
  - *主な参照先：管理者向けの権限設定（第5章）*

### 第3章：データモデリング (Model Data)
- **3-1. データモデリングを始める**
  - *主な参照先：この章のほぼ全てのページ（メトリクス、リレーションシップ等）*
- **3-2. メトリクスについて**
  - *主な参照先：関数リファレンス（第6章）*
- **3-3. リレーションシップの定義**
  - *主な参照先：データ分析の章のテーブルやピボットテーブルでの利用方法*
- **3-4. 各種セキュリティ設定（列、行）**
  - *主な参照先：ユーザーとチームの管理（第5章）*
- **3-5. 階層とマテリアライゼーション、パラメータ**
  - *主な参照先：データ分析の章（階層）、管理設定（マテリアライゼーション）、ワークブックの基本（パラメータ）*

---

## 【第3部：データの分析と共有】

### 第4章：データ分析 (Analyze Data)
- **4-1. データ探索と変換**
  - *主な参照先：関数リファレンス（第6章）*
- **4-2. チャートと可視化**
  - *主な参照先：色のカスタマイズ、条件付き書式*
- **4-3. ピボットテーブル**
  - *主な参照先：階層（第3章）*

### 第5章：共有と共同作業 (Share and Collaborate)
- **5-1. ワークブックの共有**
  - *主な参照先：エクスポート、スケジュール配信*
- **5-2. コメント機能**

---
#### 1-1. Sigmaについて (About Sigma)

Sigma を使用すると、アドホック分析とデータ探索を実行し、エンタープライズ グレードの分析を構築し、データに基づいて強力なアプリケーションを開発し、分析を製品に埋め込むことができます。
スプレッドシートでの作業、SQL クエリの記述、ビジネス インテリジェンス分析情報のダッシュボードの作成、コードの記述のいずれの場合でも、Sigma でビジネス ワークフローを構築できます。

Sigma をまだ使用していない場合は、今すぐ無料でお試しください。
Sigma の概念とユーザー インターフェイスの簡単な概要については、「Sigma の基礎」および「Sigma の使い方」を参照してください。

**アドホック分析を実行し、データを探索する**

アドホック分析でデータプラットフォームのデータを探索します。表やグラフから探索を開始し、分析結果が有益な場合は後で保存します。

* Sigma でデータの探索を始めましょう。

**エンタープライズグレードの分析を構築する**

ダッシュボードを作成する場合でも、スプレッドシートを使用する場合でも、Sigma でエンタープライズ グレードの分析を構築できます。
データはデータ プラットフォーム内に保存され、複雑なデータ ワークフローをモデル化し、テーブル、ピボット テーブル、グラフ、マップで分析できます。
他のアナリストとリアルタイムで連携し、AIベースの機能で分析を補完します。レポートをエクスポートすることで、Sigmaの外部のユーザーとインサイトを共有できます。

分析の構築を始めましょう:
* データ モデリングを始めましょう。
* テーブルやグラフなどのデータ要素とワークブックの操作を開始します。
* 200 を超える関数を使用して、単純な計算から複雑な計算まで実行します。
* AI クエリを実行して分析を補完します。
* レポートを PDF ファイル、画像、またはエクスポートによる生データとして共有します。
* マテリアライゼーションを使用して、実行速度が遅いクエリからのデータの可用性を向上させます。

**強力なデータアプリケーションを開発する**

データ プラットフォームからのリアルタイム データを使用してアプリケーションを開発し、データを使用してワークフローをアクティブ化します。
Sigma でデータ アプリケーションを開発する場合、次のことが可能になります。
* 入力テーブルを使用してデータ プラットフォームにデータを書き戻します。
* コントロール要素を使用してインタラクティブ性とフィルタリングを追加します。
* 複雑なアクションをシーケンスアクションで連結します。
* モーダルなどの UI コンポーネントを使用して、アプリケーションのような動作を設計します。

**分析を埋め込む**

Sigmaは、包括的な分析機能を様々なWebアプリケーションやワークフローにシームレスに統合できる柔軟な埋め込みオプションを提供しています。Sigmaのコンテンツと機能をエンドユーザーに直接提供することで、既存システムのユーザーエクスペリエンスを向上させることができます。

あなたの洞察を埋め込む:
* 組み込み分析の可能性を探ります。
* 埋め込みクイックスタートを使用して、実際の使用例を詳しく調べます。

#### 1-2. シグマの基礎 (Sigma Basics)

このドキュメントでは、Sigma で使用される基本的な概念と用語について説明します。

**コアコンポーネント**

Sigma 組織には次のコンポーネントがあります。

* **データソース (Data Sources)**
    分析に使用するデータのソースは、通常、Snowflake や BigQuery などのデータ プラットフォームのテーブルです。Sigma はデータ自体を保存せず、接続を介してデータにアクセスします。Sigmaはさまざまなデータ プラットフォームに接続でき、アップロードされた .csv ファイルもサポートします。Sigma 管理者は、接続のデータ権限を作成および管理します。
    ユーザーが共有されているデータセットまたはワークブックにアクセスすると、そのドキュメント所有者のソース データへの権限が Sigma 内で評価され、接続の設定で設定されているアカウント資格情報を使用して、データ プラットフォームへのクエリが実行されます。接続が OAuth 認証を使用するように構成されている場合は例外です。この場合、ユーザーのデータ権限は IdP を使用して制御され、クエリはユーザーの個人資格情報を使用して実行されます。

* **データモデルとデータセット (Data Models and Datasets)**
    データストアから取得した生データは、分析で最大限の効果を発揮するために、操作、プルーニング、追加計算、フィルタリングが必要となる場合があります。Sigmaでは、データストアからデータモデルまたはデータセットを作成し、それを使用して1つ以上のワークブック内のデータを操作します。常に生データを使用して変更を再構築するよりも、同じデータモデルを作成して異なるワークブックに再利用する方が効率的です。「データモデリング入門」をご覧ください。

* **ワークブック (Workbooks)**
    ワークブックには、分析結果を伝えるための表やビジュアライゼーションが表示されます。ワークブックには、スプレッドシートのタブのようにページが含まれています。ページには、ワークブックを閲覧するユーザーに情報を伝えるために使用される表、グラフ、コントロール（フィルター）、自由形式のテキスト、画像が含まれます。他のBI製品を使用したことがある方なら、ワークブックのページはダッシュボードのようなものです。ワークブックの概要をご覧ください。

* **API**
    Sigma REST APIを使用して、Sigma のさまざまな機能にプログラムでアクセスします。

**ワークブックの概念**

ワークブック内の Sigma で分析を実行する場合は、次の概念を理解しておいてください。

* **ページ (Pages)**
    ワークブックには、スプレッドシートのタブのようなページがあります。ページを従来のBIダッシュボードとして使用し、表示したりエクスポートしたりできます。詳細については、ワークブックの概要をご覧ください。

* **要素 (Elements)**
    要素とは、ワークブックのページに配置するオブジェクトです。要素の種類には以下のものがあります。
    * データ要素（表、グラフ、ピボットテーブル）
    * UI 要素 (テキスト、画像、ボタン、埋め込み、区切り線)
    * コントロール要素（フィルターとコントロール）
    * レイアウト要素（コンテナとモーダル）
    ワークブック内の要素を別の要素のデータソースとして使用できます。ソース要素は親要素と呼ばれ、データを使用する要素は子要素と呼ばれます。
    詳細については、「要素タイプの概要」を参照してください。

**テーブルの概念**

テーブルは Sigma での分析の最も簡単な出発点ですが、スプレッドシートや従来のビジネス インテリジェンス ツールでの作業とはいくつかの違いがあります。

* **セルではなく列 (Columns, not Cells)**
    従来のスプレッドシートツールは、データと数式をセル単位で提供します。Sigmaはデータを列レベルで管理します。計算と書式設定の変更は、列内のすべてのセルに適用されます。このアプローチは、大量のデータに対してよりスケーラブルです。
    表内の列の詳細については、「表の作成と管理」を参照してください。列の数式などの詳細を確認するには、「列の詳細の表示」を参照してください。

* **列のグループ化 (Column Grouping)**
    列をグループ化することで、グループ化レベルごとに集計などの計算を実行できます。列をグループ化することで、テーブル内で複雑な分析を実行できます。グループ化は1次元のピボットテーブルに似ていますが、ピボットテーブルよりもはるかに幅広い計算ライブラリを備えています。テーブルにグループ化を追加すると、週ごとのサインアップ数、地域ごとの売上、製品ラインごとのコストなどの指標や、特定のデータグループに適用されるその他の計算を実行できます。
    テーブルには複数のグループを追加できます。詳細な例を含む詳細については、「テーブルの作成と管理」をご覧ください。

* **フィルター (Filters)**
    フィルターは、グラフや表に表示される結果を制限し、特定の条件を満たすデータのみを表示します。例えば、特定の範囲内の値のみを表示したり、特定の日付以降に発生したイベントのみを表示したりできます。コントロール要素を追加することで、複数の要素を同時にフィルタリングできます。
    Sigmaは、ワークブック、データモデル、データセット向けに、さまざまな種類のフィルターをサポートしています。フィルターとコントロールの操作方法の詳細については、「Sigmaでデータを動的にフィルターおよび変更する」をご覧ください。

**ユーザー**

Sigma の機能へのアクセスは、さまざまなグループの人々の間で行われます。
**組織**は最高レベルであり、通常はビジネス エンティティと相関します。**チーム**はユーザーのグループです。チームを使用すると、接続、データモデル、データセット、ワークブックをグループ内で簡単に共有できます。また、チームを使用して、さまざまな種類のアクセス制限を管理することもできます。**ユーザー**とは、Sigma にアカウントを持つ個人です。ユーザーには、Sigma 組織全体の権限を管理するために、異なるアカウントタイプを割り当てることができます。

**エクスポートとレポート**

ワークブックへの権限を持つユーザーは誰でも、スクリーンショットを撮るのと同じように、要素のPNG画像をダウンロードできます。割り当てられたアカウントタイプで関連する権限が有効になっているユーザーは、Sigmaからメール、Slack、その他の形式や出力先にレポートをエクスポートできます。「ワークブックのエクスポートを送信またはスケジュールする」をご覧ください。

#### 1-3. Sigmaの歩き方 (Get around in Sigma)

**Sigmaのホームページ**

Sigmaにログインすると、ホームページが表示されます。以下の図と説明は、このページの主要な部分を解説するものです。一部の要素は、あなたのユーザー権限によっては表示されない場合があります。

* **a. 検索 (Search):**
    Sigma内のコンテンツを検索します。
    * *参照先: Search for files in your organization*

* **b. 新規作成 (Create New):**
    あなたの役割に基づいて、以下のコンテンツを作成します。
    * **ワークブック (Workbook):** スプレッドシート形式のインターフェースを使用してデータを分析し、ビジュアライゼーションを作成します。
      * *参照先: ワークブックの概要 (1-2. ワークブックの基本)*
    * **データモデル (Data model):** 他者と共有するために、データを収集、関連付け、変換、モデリングします。
      * *参照先: データモデリングを始める (Beta) (3-1. データモデリングを始める)*
    * **データセット (Dataset):** 他者と共有するために、データをキュレーション（整理・準備）します。
      * *参照先: Create and manage datasets*
    * **カスタムSQL (Custom SQL):** データウェアハウスに対して実行するSQLを記述します。
      * *参照先: Write custom SQL*
    * **CSVアップロード (CSV upload):** CSV形式のファイルをアップロードし、ワークブック内で分析を実行します。
      * *参照先: Upload CSV data*

* **c. マイコンテンツ (My Content):**
    * **ホーム (Home):** このホームページです。
    * **マイドキュメント (My Documents):** あなたが作成したコンテンツを保存するための個人用フォルダです。
    * **ワークスペース (Workspaces):** 組織内の特定のメンバーやチームとコンテンツを整理し、共有するための一つの方法です。ワークスペースに配置されたアイテムは、そのワークスペースへの権限を持つ誰もがアクセスできます。
    * **テンプレート (Templates):** あなたと共有されているワークブックのテンプレートです。
      * *参照先: Get started with workbook templates*
    * **共有アイテム (Shared with Me):** 他の人が直接あなたと共有したアイテムです。
    * **お気に入り (Favorites):** あなたがお気に入りに指定したアイテムです。
    * **ゴミ箱 (Trash):** 削除されたアイテムです。
    * **接続 (Connections):** (デフォルトでは管理者と作成者にのみ表示) あなたがアクセスできるデータウェアハウスとそのテーブルです。一つのSigma組織は多数の接続を持つことができ、各接続はメンバーやチームと共有されるために、異なるレベルのアクセス権で構成されます。
      * *参照先: データソースへの接続 (2-1. データソースへの接続)*

* **d. 最近のアイテム (Recents):**
    あなたが最近アクセスしたアイテムです。

* **e. あなたへのおすすめ (For you):**
    人気度、あなたの仕事に関連するデータの系譜、他のユーザーによって推奨されたアイテムに基づき、Sigmaがあなたに関連するドキュメントをリストアップします。

* **f. 管理 (Administration):**
    ユーザー管理やその他共通の構成設定を行うための専用エリアです。Adminアカウントタイプを付与されたユーザーにのみ表示されます。
    * *参照先: Administer Sigma*

* **g. ユーザープロフィール (User Profile):**
    あなたのプロファイルへのリンクとなっている、ユーザー名のイニシャルです。ここであなたの設定変更やサインアウトができます。他のオプションは、あなたの権限によって表示される場合とされない場合があります。

* **h. ヘルプ (Help):**
    ドキュメントやSigmaサポートのライブチャットへのアクセスなど、役立つ情報へのリンクです。

### 第2章：データへの接続 (Connect to Data)

#### 2-1. データソースへの接続 (Connect to data sources)

データソース接続は、Sigmaがあなたのデータウェアハウスと通信することを可能にします。Sigmaがコマンドを送信し、データの結果セットという形で応答を受け取るためには、オープンで利用可能な接続が必要です。

データソースに接続するために、あらゆるアプリケーション（Sigmaを含む）は、データのアドレスや場所、適切なユーザー検証（ユーザーIDとパスワード）、特定のデータベース構成オプション、セキュリティオプション、その他多くから成る**接続文字列**を提供しなければなりません。データソース接続は、その後に実行できる一連の操作の時間と比較して、作成にコストがかかります。そのため、私たちは接続を開き、一連の個別操作を実行するためにアクティブな状態を保ちます。私たちは定期的に接続の「クローズ」とリフレッシュを管理しているため、あなたが翌日Sigmaで作業する際も、シームレスに作業を続け、同じ接続を使用することができます。

接続は非常に強力なツールですが、同じデータベースエンティティに対して複数の接続を作成する前には、慎重に検討してください。接続をまたいでデータを移動させることはできないため、テーブルをまたいだ計算を実行することはできません。例えば、Connection1からTable1に、Connection2からTable2にアクセスした場合、たとえそれらが同じデータベース内にあっても、これらのテーブルを一つの集合的なエンティティとして見ることはできません。

**要件 (Requirements)**

* あなたのSigma組織における管理者権限。
  * *詳細は「ユーザーアカウントタイプ」を参照してください。*
* Sigmaがサポートするデータウェアハウス。
  * これには `Snowflake`, `BigQuery`, `Redshift`, `Databricks`, `PostgreSQL`, `AlloyDB`, そして `MySQL` が含まれます。

**データウェアハウスへの接続を作成する (Create a connection to the data warehouse)**

各ウェアハウスタイプは、異なる入力パラメータを受け付けます。あなたの接続方法に合わせて、以下の指示を使用してください。

* Connect to AlloyDB
* Connect to Azure SQL Database (Beta)
* Connect to BigQuery
* Connect to Databricks
* Connect to MySQL
* Connect to PostgreSQL
* Connect to Redshift
* Connect to Snowflake
* Connect to Starburst
* Connect to SQL Server 2022 and Azure SQL Managed Instance (Beta)

**SigmaのIPを許可リストに追加する (Add Sigma IPs to the allowlist)**

ファイアウォール、セキュリティグループ、またはその他のIPベースのセキュリティポリシーによって、あなたのウェアハウスが外部接続に対して閉じられている場合、データに正常に接続するためには、SigmaのIPアドレスを許可リストに追加する必要があります。

SigmaのアウトバウンドIPアドレスは、あなたのSigma管理者ポータルの各接続ページにリストされています。

表示するには：
1.  管理者ポータルを開き、左側のナビゲーションで `Connections` をクリックします。
2.  いずれかの接続を選択するか、`Create Connection` をクリックします。
3.  接続情報の資格情報の下にリストされているIPアドレスを探します。

> 📘
> 接続概要にリストされているIPアドレスは、プライベートリンク経由の接続には適用されません。プライベートリンク接続用のIPアドレスが必要な場合は、Sigmaサポートにお問い合わせください。

**書き込みアクセス (Write access)**

接続に対して[書き込みアクセスを有効にする](https://help.sigmacomputing.com/docs/enable-write-access)ことができます。書き込みアクセスは、[マテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)、[CSVアップロード](https://help.sigmacomputing.com/docs/upload-csv-data)、[入力テーブル](https://help.sigmacomputing.com/docs/input-tables-overview)、および[ウェアハウスビュー](https://help.sigmacomputing.com/docs/write-access-and-warehouse-views)に必要です。

**権限 (Permissions)**

接続を作成した後、組織内の他の人々と選択的にアクセスを共有することができます。詳細は、[データ権限](https://help.sigmacomputing.com/docs/data-permissions)を参照してください。

**クエリのタイムアウト (Query timeouts)**

デフォルトでは、Sigmaはクエリのタイムアウトを120秒（2分）に設定しています。クエリがタイムアウト制限に達すると、Sigmaはそのクエリをキャンセルします。`Connection Features` の下で、あなたの接続に対するカスタムクエリタイムアウトを設定できます。

**関連リソース (Related resources)**

* Connect to Snowflake
#### 2-3. Snowflakeへの接続 (Connect to Snowflake)

SigmaはSnowflakeへの安全な接続をサポートしています。

> 📘
> Snowflake接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

このドキュメントでは、あなたの組織をSigmaからSnowflakeウェアハウスに接続する方法を説明します。

> 📘
> まだSigma組織を作成していない場合は、Snowflake Partner Connectを使用して組織を作成し、数クリックでSnowflakeデータベースを接続することができます。Snowflake Partner Connectを使用するには、Snowflakeで `ACCOUNTADMIN` ロールを持っている必要があります。Snowflake Partner Connectでサインアップするには、Partner ConnectリストからSigmaを選択し、Connect to Sigmaモーダルで `Connect` をクリックします。
>
> SnowflakeとOktaを使用したOAuth構成のエンドツーエンドのウォークスルーについては、「[Open Authorization (OAuth) QuickStart](https://help.sigmacomputing.com/docs/oauth-quickstart)」を参照してください。

**要件 (Requirements)**

* あなたは `Admin` アカウントタイプを割り当てられている必要があります。
* 必要なデータベースとスキーマに対する `USAGE` 権限、および必要なテーブルに対する `SELECT` 権限を持つロールが割り当てられたSnowflakeユーザーの資格情報を提供できる必要があります。

> 🚩
> Sigmaは、データベース、スキーマ、テーブル、ビューをインデックス化するために、24時間ごとにSnowflake接続にクエリを実行します。このプロセスは自動化されており、クラウドサービスレイヤーのSnowflakeメタデータから読み取ります。通常の使用では、このプロセスによるクレジット消費は0ですが、24時間以内に最小限の使用しかない場合には、クレジット消費が発生することがあります。Snowflakeドキュメントの「[Understanding overall cost](https://docs.snowflake.com/en/user-guide/cost-understanding-overall)」を参照してください。

**SigmaでSnowflake接続を作成する (Create a Snowflake connection in Sigma)**

Snowflake接続を作成するには、Sigmaで以下のステップを実行します。
1.  接続を追加し、接続詳細を指定する
2.  接続資格情報を指定する
3.  認証方法を構成する：
    * キーペア認証でSnowflakeに接続する
    * OAuthでSnowflakeに接続する
    * 基本認証でSnowflakeに接続する
4.  書き込みアクセスを構成する
5.  接続機能を構成する

**1. 接続を追加し、接続詳細を指定する (Add a connection and specify connection details)**

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。`Add new connection` ページが表示されます。
3.  `Connection details` で、以下を指定します。
    * **Name:** 新しい接続の `Name` を入力します。Sigmaはこの名前を接続リストに表示します。
    * **Type:** `Snowflake` タイルを選択します。

**2. 接続資格情報を指定する (Specify your connection credentials)**

`Connection Credentials` セクションで、必須項目を入力します。

* [任意] プロキシサーバーを使用してSnowflakeにアクセスする場合は、`Use Custom Host` トグルをオンにし、`Snowflake Custom Host` 名を入力します。
* `Account` フィールドに、Snowflakeのアカウント名を入力します。アカウント名のフォーマット方法の詳細は、Snowflakeドキュメントの「[Using an account name as an identifier](https://docs.snowflake.com/en/user-guide/connecting.html#using-an-account-name-as-an-identifier)」を参照してください。
* `Warehouse` フィールドに、Snowflakeにリストされているウェアハウス名を入力します。
    > 📘
    > ユーザー属性を使用してウェアハウスを設定するには、`Warehouse` フィールドの `Set by user attributes` をクリックします。「[Configure user attributes on a Snowflake connection](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照してください。
* `Warehouse` フィールドをユーザー属性を使用して設定し、この接続で入力テーブルを使用する予定がある

* #### 2-4. Snowflake接続でユーザー属性を構成する (Configure user attributes on a Snowflake connection)

新規または既存のSnowflake接続でユーザー属性を設定することで、特定のユーザーが使用するSnowflakeのウェアハウスやロールを、そのユーザーの属性値に基づいて動的に割り当てることができます。

このドキュメントでは、Snowflake接続で属性を使用する方法とその理由について説明します。Snowflake接続では、`Warehouse`と`Role`の2つの属性が利用可能です。

接続で属性を構成した後、セキュアな埋め込みURLで外部ユーザーに属性を渡すこともできます。詳細は、「[Apply dynamic connection and role switching to embeds](https://help.sigmacomputing.com/docs/dynamic-connection-switching)」を参照してください。

**ウェアハウス属性について (About the warehouse attribute)**

`Warehouse`属性を使用すると、Sigma内のユーザーに割り当てられたユーザー属性の値に基づいて、使用されるSnowflakeウェアハウスを動的に変更できます。
これは、クライアントごとに個別のウェアハウスを作成し、クライアントごとのコンピューティングコストを簡単に監視できるため、クライアントベースのセットアップで役立ちます。

**ロール属性について (About the role attribute)**

`Role`属性は、Sigmaで行レベルのセキュリティやセキュリティポリシーを手動で再作成する代わりに、Snowflakeで構成したロールを使用して行レベルのセキュリティを提供します。この機能はOAuthを使用する代わりの方法であり、ユーザー属性を使用してSigmaのSnowflake接続にSnowflakeロールを動的に展開することができます。この機能はOAuthとは併用できません。

> 📘
> 埋め込みユーザーの場合、ユーザーとチームに属性を設定できます。内部ユーザーの場合、チームに属性を設定できます。

**要件 (Requirements)**

* あなたは `Admin` アカウントタイプを割り当てられている必要があります。
* また、この構成をサポートするために、Snowflakeでの権限が設定されていることを確認する必要があります。
    * 特定のウェアハウスで使用されるSnowflakeロールには、そのウェアハウスに対する少なくとも `USAGE` 権限が付与されている必要があります。
    * Snowflakeロールには、Sigmaに接続されている関連データベースとスキーマに対する少なくとも `USAGE` 権限も付与されている必要があります。
    * Snowflakeロールは、接続に関連付けられているSnowflakeユーザーに付与されている必要があります。

**ユーザー属性を構成する (Configure user attributes)**

Snowflakeウェアハウス接続でユーザー属性を構成するためには、まずユーザー属性を作成し、それらをチームに割り当てる必要があります。ユースケースに応じて、`Warehouse`、`Role`、またはその両方のためのユーザー属性を作成できます。

ユーザー属性を構成するには、以下を実行します。
1.  Sigma管理者ポータルで、`User Attributes` に移動し、`Create Attribute` をクリックします。
2.  `New Attribute` セクションで、`Name` フィールドに一意の名前を入力します。
3.  `Description` フィールドに、属性の説明を入力します。（任意）
4.  `Default Value` フィールドに、デフォルト値を入力します。チームに値が設定されていない場合、Sigmaはここで定義された値を使用します。（任意）
5.  `Create` をクリックします。

`Create` をクリックすると、属性は `User Attributes` の下に表示されます。
より詳細な説明については、「[User Attributes](https://help.sigmacomputing.com/docs/user-attributes)」を参照してください。

**ユーザー属性を割り当てる (Assign user attributes)**

チームにユーザー属性を割り当てるには、以下を実行します。
1.  `Teams Assigned` セクションで、`Assign Attribute` をクリックして、この属性にチームを割り当てます。
2.  検索バーで、この属性を割り当てるチームを検索するか、検索バー内をクリックして組織のチームのリストを表示します。詳細は、「[Teams](https://help.sigmacomputing.com/docs/teams)」を参照してください。
3.  `Assigned Value` フィールドに値を追加します。
4.  `Assign` をクリックします。これで、あなたのチームは `Teams Assigned` の下にリストされます。
5.  チームの優先順位を並べ替えるには、`Teams Assigned` セクションで、ドラッグハンドルの上にカーソルを置きます。`Priority` 列の下で、チームを目的の優先順位にドラッグ＆ドロップします。

> 📘
> ユーザーが複数のチームのメンバーである場合、`Priority` を使用して、そのチームのユーザーがどの割り当て値に従うかを決定します。

**Snowflake接続でユーザー属性を設定する (Set user attributes on a Snowflake connection)**

ウェアハウスやロールをユーザーに動的に割り当てるために使用するユーザー属性を構成した後、新規または既存の接続でユーザー属性を使用するように構成します。

1.  管理者ポータルで、`Connections` に移動します。
2.  `Create Connection` をクリックするか、既存のSnowflake接続を開きます。
3.  サービスアカウントを使用する既存の接続でユーザー属性を構成している場合は、ステップ5に進みます。
4.  `Snowflake` をクリックします。`Connect to Snowflake` ドキュメントの一般的な構成手順に従います。
5.  `Warehouse` フィールドの `More Menu` をクリックして、以前に構成したウェアハウス属性を参照して選択します。
6.  `Role` フィールドの `More Menu` をクリックして、以前に構成したロール属性を参照して選択します。OAuthアクセスは選択解除する必要があります。

これで、あなたのSnowflake接続は、Snowflakeで設定されたロールとウェアハウスを動的に使用するように構成されました。

**セキュアな埋め込みでの使用 (Use with secure embeds)**

接続で属性を構成した後、セキュアな埋め込みURLで外部ユーザーに属性を渡すことができます。埋め込みでロールとウェアハウスの属性を使用するには、パラメータをURL（埋め込みパスURL）に追加する必要があります。

> 📘
> `Role`属性の場合、この構成はセキュアな埋め込みの期間中、行レベルのセキュリティを強制します。

**セキュアな埋め込みURLにパラメータを追加する (Add parameters to a secure embed URL)**

セキュアな埋め込みで属性を渡すためには、両方の属性のパラメータを埋め込みURLに追加する必要があります。
埋め込みURLでは、属性は次のようにフォーマットされるべきです。

#### 2-5. エクスポートウェアハウスを構成する (Configure an export warehouse)

エクスポートウェアハウスとは、Sigmaのエクスポートを実行するために特別に作成された、Snowflake内の仮想ウェアハウスのことです。

デフォルトでは、Sigmaはエクスポートクエリを接続のプライマリウェアハウスに送信しますが、すべてのスケジュールされた、直接の、オンデマンドのエクスポートを別のエクスポートウェアハウス経由で実行するように構成することができます。この慣行は、エクスポート操作を分離してパフォーマンスを最適化し、コンピューティングコストを削減します。

このドキュメントでは、Sigmaでエクスポートウェアハウスを構成する方法を説明します。

**システムとユーザーの要件 (System and user requirements)**

Sigmaでエクスポートウェアハウスを構成する機能には、以下が必要です。
* あなたのSigma組織には、既存の[Snowflake接続](https://help.sigmacomputing.com/docs/connect-to-snowflake)が必要です。
* あなたは `Admin` アカウントタイプを割り当てられている必要があります。

**前提条件 (Prerequisites)**

Sigmaでエクスポートウェアハウスを構成する前に、あなた（または適切なSnowflake権限を持つ別のユーザー）は、Snowflake内でエクスポートクエリを実行するための専用の仮想ウェアハウスを別途作成しておく必要があります。このプロセスの詳細については、Snowflakeのドキュメント「[CREATE WAREHOUSE](https://docs.snowflake.com/en/sql-reference/sql/create-warehouse)」を参照してください。

**エクスポートウェアハウスを構成する (Configure an export warehouse)**

Snowflake接続を適宜構成することで、Sigmaが専用のエクスポートウェアハウスを使用できるようにします。

1.  **「Administration」 > 「Connections」に移動します。**
    * Sigmaヘッダーで、あなたのユーザーアバターをクリックしてユーザーメニューを開きます。
    * 「Administration」を選択して、管理者ポータルを開きます。
    * サイドパネルで、「Connections」を選択します。
2.  **「Connections」ページで、エクスポートウェアハウスを追加したいSnowflake接続を選択します。**
3.  **接続概要の「Connection Details」セクションに移動し、「Edit」をクリックします。**
4.  **「Connection Features」セクションで、「Export Warehouse」フィールドを探し、エクスポートクエリ用に作成した仮想ウェアハウスの名前を入力します。**
5.  **「Save」をクリックして、指定されたウェアハウス経由ですべてのスケジュールされた、直接の、オンデマンドのエクスポートを実行するようにします。**

> 📘
> エクスポートウェアハウスは、プライマリウェアハウスの接続キューサイズを継承します。エクスポートウェアハウスに異なるキューサイズを設定するには、サポートにお問い合わせください。
>
> #### 2-6. Snowflake接続またはユーザーの入力テーブルアクセスを復元する (Restore input table access for a Snowflake connection or user)

管理者がSigmaで接続用に構成されたSnowflakeロールを変更すると、不十分なロール権限が入力テーブルへのアクセスを中断させ、ユーザーが新しい入力テーブルを作成したり、既存のものへの編集を保存したりできなくなることがあります。このエラーは、接続がOAuthを使用しており、ユーザーのロールがSnowflake内で再割り当てされた場合にも発生する可能性があります。

このドキュメントでは、エラーの根本原因を特定し、接続またはユーザーの入力テーブルアクセスを復元するために必要な権限を付与する方法について説明します。

**システムとユーザーの要件 (System and user requirements)**

接続またはユーザーの入力テーブルアクセスを復元する機能には、以下が必要です。
* あなたはSigmaで `Admin` アカウントタイプを割り当てられている必要があります。
* あなたはSnowflakeでオブジェクトに対する権限を付与できる必要があります。

**エラーの根本原因と解決策を特定する (Identify the error's root cause and resolution)**

Snowflakeロールが入力テーブルデータと編集ログ（先行書き込みログ、WALとも呼ばれる）にアクセスするための権限を欠いている場合、影響を受けるユーザーはSigmaで新しい入力テーブルを作成したり、既存のものへの編集を保存したりできません。ワークブックには「SQL compilation error」メッセージが表示され、オブジェクトが存在しないか、承認されていないことを示します。そして、Sigmaは「Input table edits failed」というシステムメールを組織の全管理者とエラーに遭遇したユーザーに送信します。このエラーについて管理者に送信されるメールには、「ユーザーが不十分なロール権限のために入力テーブルへの編集を保存できませんでした」と記載されています。

入力テーブルアクセスを復元するための解決策は、接続の認証方法と、そのロールが接続に適用されるか、接続にアクセスする特定のユーザーに適用されるかによって異なります。以下の表を使用してエラーの根本原因と解決策を特定し、その後、このドキュメントの「ロールと書き戻しスキーマを取得する」および「Snowflakeでロール権限を更新する」セクションを参照してください。

| 接続認証 | エラーメッセージのオブジェクトプレフィックス¹ | 根本原因 | Snowflakeでの解決策 |
| :--- | :--- | :--- | :--- |
| 非OAuth<br>(基本またはキーペア) | `SIGDS` または `SIGDS_WAL` | 接続で使用されるロールが、入力テーブルデータと編集ログを含むテーブルにアクセスできない。 | 書き戻しスキーマ内で、接続で使用されるロールに以下の権限を付与する：<br>入力テーブルデータを含むテーブル（`SIGDS`プレフィックス）に対し、`ALL PRIVILEGES`を付与。<br>編集ログを含むテーブル（`SIGDS_WAL`プレフィックス）に対し、`INSERT`と`SELECT`を付与。 |
| OAuth | `SIGDS_WAL` | 接続のサービスアカウントで使用されるロールが、編集ログを含むテーブルにアクセスできない。 | 書き戻しスキーマ内で、接続のサービスアカウントで使用されるロールに以下の権限を付与する：<br>編集ログを含むテーブル（`SIGDS_WAL`プレフィックス）に対し、`INSERT`と`SELECT`を付与。 |
| OAuth | `SIGDS` | ユーザーに割り当てられたロールが、入力テーブルデータを含むテーブルにアクセスできない。 | 書き戻しスキーマ内で、ユーザーに割り当てられたロールに以下の権限を付与する：<br>入力テーブルデータを含むテーブル（`SIGDS`プレフィックス）に対し、`ALL PRIVILEGES`を付与。 |

¹ Sigmaは（ユーザーがエラーに遭遇した際に）ワークブックにエラーメッセージを表示し、システムメールにもそれを含めます。エラーメッセージでは、`SIGDS`プレフィックスは入力テーブルに保存されたデータを含むテーブルを識別し、`SIGDS_WAL`プレフィックスは編集ログを含むテーブルを識別します。

**ロールと書き戻しスキーマを取得する (Retrieve the role and write-back schema)**

Snowflakeでロール権限を正確に更新するために、まずSigmaから関連する詳細情報を取得します。

* **非OAuth接続 (Non-OAuth connection)**
    エラーが非OAuth接続で発生した場合、接続で使用されるロールの名前と、書き戻しスキーマの名前を取得します。
    1.  入力テーブル編集の失敗を報告するシステムメールを受け取った場合は、メール内の `View connection` をクリックして、Sigma管理者ポータルの接続概要に直接アクセスします。そうでない場合は、Sigmaで `Administration` > `Connections` に移動し、該当するSnowflake接続を選択します。
    2.  接続概要の `Connection Credentials` セクションで、`Role` フィールドを参照して、権限付与が必要なSnowflakeロールの名前を取得します。
    3.  `Write Access` セクションで、`Write schema` フィールドを参照して、入力テーブルデータと編集ログを含む書き戻しスキーマの名前を取得します。

* **OAuth接続 (OAuth connection)**
    エラーがOAuth接続で発生した場合、接続のサービスアカウントで使用されるロールの名前（根本原因がサービスアカウントのロールレベルにある場合のみ）と、書き戻しスキーマの名前を取得します。
    1.  入力テーブル編集の失敗を報告するシステムメールを受け取った場合は、メール内の `View connection` をクリックして、Sigma管理者ポータルの接続概要に直接アクセスします。そうでない場合は、Sigmaで `Administration` > `Connections` に移動し、該当するSnowflake接続を選択します。
    2.  権限付与が必要なSnowflakeロールの名前を取得します。
        * エラーの根本原因がサービスアカウントのロールレベルにある場合、接続概要の `Connection Credentials` セクションに移動し、`Role` フィールドを参照します。
        * エラーの根本原因がユーザーのロールレベルにある場合、システムメール内のユーザーのメールアドレスを参照し、Snowflakeで割り当てられているユーザーのデフォルトロールを特定します。
    3.  `Write Access` セクションで、`Write destinations` フィールドを参照して、入力テーブルデータと編集ログを含む書き戻しスキーマの名前を取得します。
    > 📘
    > 接続が複数のデスティネーションに書き込む場合、システムメールのエラーメッセージを参照し、デスティネーションパスから特定の書き戻しスキーマを取得します。また、ワークブックにアクセスして入力テーブルを更新し、入力テーブルのクエリ詳細から該当する書き戻しスキーマの名前を取得することもできます。

**Snowflakeでロール権限を更新する (Update role privileges in Snowflake)**

前のセクションで取得したロールと書き戻しスキーマを使用して、このドキュメントの「入力テーブルエラーの根本原因と解決策を特定する」セクションで概説された適切な解決策を実装します。

SQLまたはSnowsightを使用して、Snowflakeのテーブルに権限を付与できます。詳細はSnowflakeのドキュメント「[Grant privileges to the role](https://docs.snowflake.com/en/user-guide/security-access-control-configure#grant-privileges-to-the-role)」を参照してください。

> 💡
> テーブルに権限を付与する前に、そのロールが入力テーブルデータへのアクセスを必要とし、意図的に制限されていないことを確認してください。
> Snowflakeで特定された書き戻しスキーマまたはテーブルが見つからない場合、そのオブジェクトはもはや存在しない可能性があります。スキーマまたは編集ログが意図せず削除された場合は、新しい接続を作成するか、編集ログテーブルを再作成する必要があります。詳細はサポートにお問い合わせください。
* 
* Connect to AlloyDB
* #### 2-7. AlloyDBへの接続 (Connect to AlloyDB)

SigmaはAlloyDBへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をAlloyDBデータベースに接続する方法を説明します。

> 📘
> AlloyDB接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* あなたのSigma組織における管理者権限。
  * 詳細は、「[User account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* AlloyDBデータウェアハウスと、そこのアカウント。
  * データストアに接続する際に使用するアカウントに過剰な権限を付与しないことをお勧めします。例えば、SYSADMINレベルのアクセスは必要ありません。

**AlloyDB接続を作成する (Create an AlloyDB Connection)**

> 📘
> あなたのAlloyDBインスタンスがVPC上にある場合、追加のステップが必要です。詳細は、「[Configure VPC Service Controls](https://help.sigmacomputing.com/docs/vpc-service-controls)」を参照してください。

接続を作成するには、以下のステップに従います。

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。
    * `Add new connections` ページが表示されます。

3.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`AlloyDB connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`AlloyDB` タイルをクリックします。

4.  `Connection Credentials` セクションで、以下を指定します。
    * **Host**
        あなたのデータベースへのパス。これはURLまたはIPアドレスです。
        あなたのクラスタのエンドポイントURLを入力してください。SigmaはIP `104.197.169.18` と `104.197.193.23` から接続します。
    * **Port**
        Sigmaがホストへの接続に使用するポート。
    * **User**
        AlloyDBへの接続に使用するユーザー名またはアカウント。
        例： `test`
    * **Password**
        AlloyDBアカウントの `User` に対応するパスワードを入力します。
    * **Database**
        クエリを実行
* Connect to BigQuery
* #### 2-8. BigQueryへの接続 (Connect to BigQuery)

SigmaはBigQueryへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をBigQueryウェアハウスに接続する方法を説明します。

> 📘
> BigQuery接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* あなたのSigma組織における管理者権限。詳細は「[account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* あなたのGoogle Cloudプロジェクトで[サービスアカウントを作成する](https://cloud.google.com/iam/docs/creating-managing-service-accounts)権限。
* データストアに接続する際に使用するアカウントに過剰な権限を付与しない
* Connect to Databricks
* #### 2-9. Databricksへの接続 (Connect to Databricks)

SigmaはDatabricksへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をDatabricksウェアハウスに接続する方法を説明します。

> 📘
> Databricks接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* **あなたのSigma組織にて：**
    * あなたは `Admin` アカウントタイプを割り当てられている必要があります。
* **Databricksにて：**
    * Databricks SQLアクセスが有効になっているDatabricksワークスペースへのアクセス権が必要です。Databricksドキュメントの「[Manage entitlements](https://docs.databricks.com/en/sql/admin/manage-users-and-groups.html#manage-entitlements)」を参照してください。
    * Databricks SQLウェアハウスへのアクセス権、またはAdminであるか `Allow unrestricted cluster creation` ユーザーエンタイトルメントを持つことによる作成能力が必要です。Databricksドキュメントの「[Requirements](https://docs.databricks.com/en/sql/admin/sql-warehouses.html#requirements)」を参照してください。
    * あなた自身のパーソナルアクセストークン（PAT）、または権限を持つユーザーやサービスプリンシパルに紐づいたトークンを使用できる必要があります。Databricksドキュメントの「[Monitor and manage access to personal access tokens](https://docs.databricks.com/en/security/auth-authz/pat.html#monitor-and-manage-access-to-personal-access-tokens)」を参照してください。

**Databricksを構成する (Configure Databricks)**

SigmaにDatabricks接続を追加する前に、Databricksで以下のステップを完了してください。

1.  まだ存在しない場合は、Databricks SQLウェアハウスを作成します。Databricksドキュメントの「[Create a SQL warehouse](https://docs.databricks.com/en/sql/admin/sql-warehouses.html#create-a-sql-warehouse)」を参照してください。
2.  このSQLウェアハウスへの接続に使用するユーザーまたはサービスプリンシパルが、そのコンピュートリソースに対する `Can use` または `Can manage` の権限を持ち、全てのワークスペースユーザーが `Can use` の権限を持っていることを確認してください。
3.  `Auto stop` 設定を構成します。この設定に関する情報は、Databricksドキュメントの「[Configure SQL warehouse settings](
* Connect to MySQL
* #### 2-10. MySQLへの接続 (Connect to MySQL)

SigmaはMySQL（リリース8.0以上）への安全な接続をサポートしています。
このドキュメントでは、あなたの組織をMySQLデータベースに接続する方法を説明します。

> 📘
> MySQL接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

* **お客様 (Customers)**
  この機能へのアクセスは、アカウント担当者を通じてリクエストしてください。
* **見込み客の皆様 (Prospects)**
  この機能へのアクセスは、弊社[セールスチーム](https://www.sigmacomputing.com/contact-sales/)を通じてリクエストしてください。

**要件 (Requirements)**

* あなたのSigma組織における管理者権限。詳細は、「[User account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* 関連するデータベースとテーブルに対する `READ` 権限を持つMySQLアカウント。CSVデータをアップロードする予定がある場合は、アカウントは `WRITE` 権限を持っている必要があります。
* SigmaはMySQLバージョン8.0以上をサポートしています。
* データストアに接続する際に使用するアカウントに過剰な権限を付与しないことをお勧めします。例えば、SYSADMINレベルのアクセスは必要ありません。
* Azure上のMySQLは、デフォルトでは名前付きタイムゾーンを持っていません。そのため、Sigmaが正しく動作するためには、タイムゾーンデータをMySQLデータベースにロードする必要があります。そうしないと、接続設定時にエラーが発生する可能性があります。Microsoftのドキュメント「[Populating the time zone tables](https://learn.microsoft.com/en-us/azure/mysql/single-server/how-to-server-parameters#populating-the-time-zone-tables)」を参照してください。これはAWSやGCP上のMySQLでは問題になりません。

**接続を作成する (Create a connection)**

接続を作成するには、以下の基本的なステップに従います。

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。
    * `Add new connections` ページが表示されます。

3.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`MySQL connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`MySQL` タイルをクリックします。

4.  `Connection Credentials` セクションで、以下を指定します。
    * **Host**
        あなたのデータベースへのパス。これはURLまたはIPアドレスです。
    * **Port**
        Sigmaがホストへの接続に使用するポート。
        MySQLのデフォルトポートは `3306` です。
    * **User**
        MySQLデータウェアハウスへの接続に使用するユーザー名またはアカウント。
        例：`test`
    * **Password**
        MySQLアカウントの `User` に対応するパスワードを入力します。
    * **Database**
        クエリを実行する予定のデータベースの名前。
    * **Enable TLS**
        任意。このスイッチは接続のTLS暗号化を有効または無効にします。
        デフォルトで有効。
    * **SSH Tunnel**
        任意。このスイッチはセキュアなリモートログインのためのSSHプロトコルを有効にします。詳細は、「[Connect through SSH](https://help.sigmacomputing.com/docs/connect-through-ssh)」を参照してください。
        デフォルトで無効。
        もしオンにする場合は、`Tunnel host` と `Tunnel port` フィールドを指定します。
    * **Tunnel host**
        トンネルサーバーへのパス。これはURLまたはIPアドレスです。
        `SSH Tunnel` がオンの場合にのみ表示されます。
    * **Tunnel port**
        トンネルが接続するポート。
        `SSH Tunnel` がオンの場合にのみ表示されます。

5.  `Connection Features` セクションで、以下を指定します。
    * **Connection timeout**
        タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
        デフォルトは120（2分）。最大は600（10分）。
    * **Use friendly names**
        このスイッチはデータソースの列名をより読みやすくします。
        例えば、データベースの列 `ORDER_NUMBER` は `Order Number` として表示されます。
        デフォルトでオン。

6.  `Write Access` セクションで、書き込みアクセスが必要かどうかを決定します。
    * 詳細は、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」を参照してください。
    * **Enable write access**
        `CSV upload` と `Materialization` に必要です。
        デフォルトでオフ。
        もしオンにする場合は、`Write schema` フィールドを指定します。
    * **Write schema**
        Sigmaがテーブルを書き込むスキーマ。
        `Enable write access` がオンの場合にのみ表示されます。

7.  接続の全てのパラメータを指定したら、`Create` をクリックします。

接続が正常に作成されると、Sigmaはそれを画面に表示します。
接続を確認するには、`Browse Connection` をクリックし、表示されるデータベースとテーブルを探索します。
`Add Permission` をクリックして、組織内のユーザーにデータアクセス権を付与します。
詳細は、「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
新しい接続は、あなたのアカウントにある接続のリストにも表示されます。
* Connect to PostgreSQL
#### 2-11. PostgreSQLへの接続 (Connect to PostgreSQL)

SigmaはPostgreSQLへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をPostgreSQLデータベースに接続する方法を説明します。

> 📘
> PostgreSQL接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* あなたのSigma組織における管理者権限。詳細は「[Account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* PostgreSQLデータウェアハウス
* 構成済みのPostgreSQLクラスター
* データストアに接続する際に使用するアカウントに過剰な権限を付与しないことをお勧めします。例えば、SYSADMINレベルのアクセスは必要ありません。

**PostgreSQL接続を作成する (Create a PostgreSQL connection)**

接続を作成するには、以下の基本的なステップに従います。

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。
    * `Add new connections` ページが表示されます。

3.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`PostgreSQL connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`PostgreSQL` タイルをクリックします。
* Connect to Redshift
#### 2-12. Redshiftへの接続 (Connect to Redshift)

SigmaはAmazon Redshiftへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をAmazon Redshiftウェアハウスに接続する方法を説明します。

> 📘
> Amazon Redshift接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* **あなたのSigma組織にて：**
    * あなたは `Admin` アカウントタイプを割り当てられている必要があります。
* **AWSにて：**
    * 構成済みのクラスターを持つAmazon Redshiftデータウェアハウスへのアクセス権が必要です。この接続で入力テーブルを使用している場合、ノードサイズは `ra3.4xlarge` 以上が推奨されます。

**Amazon Redshiftを構成する (Configure Amazon Redshift)**

あなたのSigma組織でAmazon Redshift接続を追加する前に、AWSマネジメントコンソールで以下のステップを完了してください。

1.  あなたのAmazon Redshiftクラスターをパブリックアクセス可能に変更し、それに接続するためのElastic IPアドレスを割り当てます。
2.  セキュリティグループを作成し、そのセキュリティグループのインバウンドおよびアウトバウンドルールにSigmaのIPアドレスを追加します。IPアドレスはSigma UIの接続構成ページから取得します。「[Add Sigma IPs to the allowlist](https://help.sigmacomputing.com/docs/connect-to-data-sources#add-sigma-ips-to-the-allowlist)」を参照してください。
3.  あなたのAmazon Redshiftクラスターにセキュリティグループをアタッチします。
4.  あなたのSigma組織への接続のためのサービスアカウントとして機能するAmazon Redshiftユーザーを作成します。
5.  このユーザーに、Redshiftクラスター内の関連する全てのスキーマに対する `USAGE` 権限と、それらのスキーマ内の関連する全てのテーブルに対する `SELECT` 許可を付与します。スキーマに追加される可能性のある追加のテーブルに対しても、このユーザーが同じ権限を持つように構成します。
    * 権限付与に関するドキュメントは、Amazon Redshiftデータベース開発者ガイドの「[GRANT](https://docs.aws.amazon.com/redshift/latest/dg/r_GRANT.html)」を参照してください。
    * **SQLステートメントの例:**
        ```sql
        CREATE USER your_sigma_service_account_name password ‘a_secure_password’; 
        GRANT USAGE ON SCHEMA your_schema_name TO your_sigma_service_account_name;
        GRANT SELECT ON ALL TABLES IN SCHEMA your_schema_name TO your_sigma_service_account_name;
        ALTER DEFAULT PRIVILEGES IN SCHEMA your_schema_name
        GRANT SELECT ON TABLES TO your_sigma_service_account_name;
        ```
6.  [任意] [ストアドプロシージャアクション](https://help.sigmacomputing.com/docs/stored-procedure-actions)を実行したい場合は、サービスアカウントユーザーに、Sigmaから実行したいストアドプロシージャを含む任意のスキーマに対する `USAGE` と、全てまたは特定のストアドプロシージャに対する `EXECUTE` 権限を付与します。
    * **SQLステートメントの例:**
        ```sql
        GRANT USAGE ON SCHEMA your_sproc_schema_name TO your_sigma_service_account_name;
        GRANT EXECUTE ON ALL PROCEDURES IN SCHEMA your_sproc_schema_name TO your_sigma_service_account_name;
        ```
7.  [任意] CSVアップロード、マテリアライゼーション、入力テーブル、ウェアハウスビューなどの書き込みアクセス機能を活用したい場合は、Sigmaの書き戻し機能がデータ書き込みに使用できる専用のスキーマを作成します。
    * そのスキーマに対する `CREATE` 権限をあなたのユーザーに付与し、そのスキーマ内の全てのテーブルに対する `SELECT, INSERT, UPDATE, DELETE` を付与します。スキーマに追加される可能性のある追加のテーブルに対しても、あなたのユーザーが同じ権限を持つように構成します。
    * **SQLステートメントの例:**
        ```sql
        GRANT USAGE, CREATE ON SCHEMA your_write_schema_name TO your_sigma_service_account_name;
        GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA your_write_schema_name TO your_sigma_service_account_name;
        ALTER DEFAULT PRIVILEGES IN SCHEMA your_write_schema_name
        GRANT SELECT, INSERT, UPDATE, DELETE ON TABLES TO your_sigma_service_account_name;
        ```

**SigmaでAmazon Redshift接続を作成する (Create an Amazon Redshift connection in Sigma)**

Amazon Redshift接続を作成するには、Sigma UIで以下のステップを実行します。
1.  接続を追加し、接続詳細を指定する
2.  接続資格情報を指定する
3.  書き込みアクセスを構成する
4.  接続機能を構成する

* **1. 接続を追加し、接続詳細を指定する**
    1.  画面右上のユーザーアイコンをクリックします。
        * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
    2.  ドロップダウンメニューで、`Add connection` を選択します。`Add new connection` ページが表示されます。
    3.  `Connection Details` セクションで、以下を指定します。
        * **Name:** 新しい接続の `Name` を入力します。
        * **Type:** `Redshift` タイルを選択します。

* **2. 接続資格情報を指定する**
    `Connection Credentials` セクションで、必須項目を入力します。
    * `Host` フィールドに、あなたのRedshiftクラスターの `General Information` 画面にある `Endpoint` フィールドの値を入力します。
      * *例: `cluster.abcd.us-west-1.redshift.amazonaws.com`*
    * `Port` フィールドに、あなたのクラスターのポート番号を入力します。ポート番号はAmazon Redshiftクラスターのプロパティの `Database configurations` の下にあります。
      * *例: `5439`*
    * `User` および `Password` フィールドに、あなたのSigma組織に接続するために作成したAmazon Redshiftユーザーのユーザー名とパスワードを入力します。「[Configure Amazon Redshift](#configure-amazon-redshift)」のステップ4を参照してください。
    * `Database` フィールドに、あなたのクラスターのデータベース名を入力します。
    * [任意] `Enable TLS` トグルをオンにして、接続のTLS暗号化を有効にします。
    * [任意] `SSH Tunnel` トグルをオンにしてSSH経由で接続し、`Tunnel host` と `Tunnel port` を入力します。「[Connect through SSH](https://help.sigmacomputing.com/docs/connect-through-ssh)」を参照してください。
    * 次に、追加オプションについては「書き込みアクセスを構成する」および「接続機能を構成する」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

* **3. 書き込みアクセスを構成する**
    書き込みアクセスは、以下の機能に必要です。
    * CSV upload
    * Materialization
    * Input tables
    * Warehouse views

    書き込みアクセスを構成するには、Sigmaがデータ書き込みに使用できる専用のスキーマをAmazon Redshiftで設定し、そのスキーマに対する必要な権限をサービスアカウントに付与する必要があります。「[Configure Amazon Redshift](#configure-amazon-redshift)」のステップ5を参照してください。
    1.  この接続で書き込みアクセスを許可するには、`Enable write access` の隣にあるトグルをオンにします。
    2.  `Write schema` フィールドに、Sigmaが書き戻しデータを保存するために作成した専用スキーマの名前を入力します。
    3.  次に、追加オプションについては「接続機能を構成する」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

* **4. 接続機能を構成する**
    `Connection Features` セクションで、以下を指定します。
    * `Connection timeout` フィールドに、タイムアウトまでの時間（秒）を指定します。デフォルトは120秒です。最大は600秒（10分）です。
    * [任意] `Use friendly names` トグルをオフにすると、Sigmaが自動で列名を読みやすくするのをやめます。

* **接続作成を完了する**
    接続の全てのパラメータを指定した後、`Create` をクリックします。接続の概要が表示されます。
    `Browse Connection` をクリックし、`Add permission` をクリックして、組織内のユーザーに接続アクセスを許可します。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
    左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。
* Connect to Starburst
#### 2-13. Starburstへの接続 (Connect to Starburst)

Sigmaは、Snowflake、Databricks、BigQuery、またはPostgreSQLデータウェアハウスに接続するために、TrinoのSaaSディストリビューションであるStarburst Galaxyの使用をサポートしています。

このドキュメントでは、あなたのSigma組織を[Starburst Galaxy](https://www.starburst.io/platform/starburst-galaxy/)クラスターに接続する方法を説明します。

> 📘
> Starburst接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**要件 (Requirements)**

* あなたは `Admin` アカウントタイプを割り当てられている必要があります。
* Sigmaがアクセスする必要のある全てのテーブルに対する `Select from table` 権限と、クラスターに対する `Use cluster` 権限を持つStarburst Galaxyサービスアカウントの資格情報が必要です。

**Starburst接続を作成する (Create a Starburst connection)**

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。
    * `Add new connection` ページが表示されます。

3.  `Connection Details` セクションで、以下を指定します。
    * **Name:** 新しい接続の `Name` を入力します。Sigmaはこの名前を接続リストに表示します。
    * **Type:** 構成したい接続タイプを表すタイルを選択します。ここでは、`Starburst` タイルをクリックします。

4.  `Connection Credentials` セクションで、以下のフィールドを入力します。
    * **Host:**
        URLまたはIPアドレスとしての、あなたのStarburst Galaxyクラスターのアドレス。
    * **Port:**
        SigmaがあなたのStarburst Galaxyクラスターに接続するためのポート。
    * **User:**
        あなたのStarburst管理者によって設定されたサービスアカウントのユーザー名。
    * **Password:**
        あなたのStarburst管理者によって設定されたサービスアカウントのパスワード。

5.  [任意] `Connection features` セクションで、必要に応じてデフォルト値を調整します。
    * **Connection timeout:**
        タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
        デフォルトは120（2分）。最大は600（10分）。
    * **Use friendly names:**
        この設定はデフォルトでオンになっており、データソースの列名をより読みやすくします。
        例えば、データベースの列 `ORDER_NUMBER` は `Order Number` として表示されます。

6.  接続の全てのパラメータを指定したら、`Create` をクリックします。Sigmaは画面に接続の概要を表示します。

7.  `Browse Connection` をクリックし、次に `Add permission` をクリックして、組織内のユーザーにデータアクセスを許可します。

8.  左側のナビゲーションパネルを使用して、接続内のデータベースとテーブルを探索します。
    新しい接続は、あなたのアカウントにある接続のリストにも表示されます。
*
