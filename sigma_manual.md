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
### 第3章：データモデリング (Model Data)

#### 3-1. データモデリングを始める (Get started with data modeling)

データモデルはあなたのデータにセマンティックレイヤーを提供し、生データを変更することなく、構造化され管理された方法でデータを整理・保存することを可能にします。最も重要なのは、データモデルが再利用可能であるという点です。データモデルを作成すると、ビジネスロジックとメトリクスを一元管理でき、結合や長い数式を記述するような繰り返し作業を最小限に抑えることができます。

* 再利用可能なデータソース要素でデータモデルを構築します。
* 分析時にその都度結合を構築するのではなく、関連するデータソース間の[リレーションシップを定義](https://help.sigmacomputing.com/docs/define-relationships-in-data-models)します。
* 集計分析の一貫性を向上させるために[メトリクスを定義](https://help.sigmacomputing.com/docs/about-metrics)します。

データモデルは、データの操作を容易にし、分析結果に対するユーザーの信頼性を高めます。Sigmaでデータを操作するためにデータモデルを使用する必要はありませんが、データモデルを利用することで、あなたはビジネスユーザーが、管理され、キュレーションされ、頻繁に再検証されるデータを用いて分析や探索を行うことを可能にできます。

**データモデルについて (About data models)**

データモデルは、再利用可能なデータソース要素のコレクションを作成・管理するためのフレームワークを提供するSigmaドキュメントの一種です。あなたは、接続されたプラットフォームから焦点を絞ったデータのビューをキュレーションでき、ユーザーはそれをワークブックや他のデータモデルのソースとして使用できます。

データモデルは、組織のメンバーがワークブックや他のデータモデルで再利用できる関連データを統合、変換、共有するための、包括的で動的なプラットフォームを提供します。単一のデータモデルは、データモデルのより広範なデータコンテキストの異なるサブセット、視点、または評価を提供できる、再利用可能な要素のコレクションのコンテナとして機能します。この累積的なデータ表現は、関連性が高く詳細なワークブック分析を構築するための、便利で構造化された基盤を促進します。

データモデルは、以下の利点も提供します。
* **一元化された権限 (Centralized permissions):** データモデルレベルで権限を付与し、一貫性のある合理化されたアクセス制御を実現します。
* **効率的なデータハンドリング (Efficient data handling):** コントロールで再利用可能な要素を強化し、データセグメントを簡単にフィルタリングおよび洗練させます。
* **柔軟な再利用性 (Flexible reusability):** データソースとしての再利用のために、要素を迅速に有効または無効にします。

適切に設計されたデータモデルがあれば、ユーザーは分析に必要なデータに簡単にアクセスでき、データ分析に必要な時間と労力を削減できます。

**データモデルとデータセット (Data models and datasets)**

データモデルは、データセットとほぼ同じ機能のほとんどをサポートしているか、または将来サポートする予定です。
* メトリクス
* リレーションシップ
* 列レベルのセキュリティ
* 行レベルのセキュリティ
* マテリアライゼーション
* ウェアハウスビュー
* パラメータ
* URLパラメータ

データモデルと再利用可能な要素は、既存のデータセット機能を置き換えるために設計されています。Sigmaはいずれデータセットを非推奨にしますが、データモデルが完全に開発され、シームレスな移行が促進できるようになるまで、それらをサポートし続けます。この非推奨化に先立ち、Sigmaはすべてのお客様に通知し、すべてのデータセットをデータモデルに変換するための自動化された移行パスを実装します。

**データモデリングのベストプラクティス (Best practices for data modeling)**

データモデルを構築する際は、最も粒度の細かいデータから始め、関連に応じてリレーションシップとメトリクスを構築して、再利用可能なデータソース要素を開発します。

* リレーションシップが上流のテーブルを参照する**循環スキーマを避けます**。
* データモデルの下流に最も関連性の高いデータのみを提供するために、**データにフィルタを適用します**。
* ユーザーがデータソースが自分のユースケースに適合するかを判断するのに役立つよう、**説明的なタイトルを追加し、説明を含めます**。
* パフォーマンスを向上させるために**データをマテリアライズ**し、データベースの更新後にマテリアライゼーションが発生するようにスケジュールして、常に最新のデータが利用できるようにします。

詳細は、Sigmaコミュニティの「[Data model best practices](https://community.sigmacomputing.com/data-modeling/data-model-best-practices-206)」を参照してください。

#### 3-2. データモデルのナビゲーション (Navigate data models)

データモデルは、**ワークブックページ**と**概要ページ**の2つのページで構成されています。ワークブックページでは、データモデルを構築するための再利用可能な要素を作成・変換でき、一方、概要ページでは、データモデルに関するコンテキストや、組織全体での一般的な使用状況が提供されます。概要ページ内では、メタデータにアクセスして、データの構造、品質、リネージ（系譜）に関する重要なインサイトを得ることもできます。

このドキュメントでは、データモデルのナビゲーションに役立つよう、ワークブックページと概要ページの構造と内容について説明します。

**データモデルのワークブックページ (Data model workbook page)**

ワークブックページでは、単一のデータモデル内で、様々なテーブルや入力テーブルを再利用可能な要素として作成・管理することができます。このフォーマットは、Sigmaのワークブック構造の容易さと柔軟性を、データモデル開発にもたらします。ワークブック分析で行うようにデータを統合・変換し、どの要素が組織全体でデータソースとして再利用できるかを制御します。

* **a. 公開 (Publish) ボタン:**
    データモデルに適用された編集を保存します。
    データモデルを参照するドキュメントは、その再利用可能な要素の公開された状態を反映します。ドラフト状態の編集は適用されません。
* **b. コントロール要素 (Control element):**
    一つ以上の要素のデータをフィルタリングします。
    再利用可能な要素がフィルタリングされると、それを参照するドキュメントは、公開されたフィルタリング済みの状態に含まれるデータにのみアクセスできます。コントロールの使用に関する詳細は、「[Intro to control elements](https://help.sigmacomputing.com/docs/intro-to-control-elements)」を参照してください。
* **c. 再利用可能な要素 (Reusable element):**
    データソースとして利用可能です（再利用可能アイコンで示されます）。
* **d. 無効化された要素 (Disabled element):**
    データソースとして利用できません（無効化アイコンで示されます）。
* **e. 要素追加バー (Add element bar):**
    新しいテーブル、入力テーブル、コントロール、またはUI要素を追加できます。

**データモデルの概要ページ (Data model overview page)**

概要ページは、データの可視性と管理を向上させるために、データモデル内の各再利用可能要素に関する詳細を提供します。

* **a. 編集 (Edit) ボタン:**
    **データモデルのワークブックページ**を開きます。
* **b. データモデル詳細 (Data model details):**
    データモデルの説明を表示し、モデルの所有者、場所、最終更新の相対的なタイムスタンプ、モデルに含まれる再利用可能な要素の数を識別します。
* **c. 展開された要素の概要 (Expanded element overview):**
    再利用可能要素の接続、最終マテリアライゼーションの相対的なタイムスタンプ、それをデータソースとして参照しているトップ3のドキュメント、それを活用しているトップ3の組織メンバー、そして要素のデータテーブルの公開された状態を表示します。
* **d. 折りたたまれた要素の概要 (Collapsed element overviews):**
    再利用可能要素のタイトル、それをデータソースとして参照しているドキュメントの数、そしてそのデータテーブルの行数と列数を表示します。
* **e. 詳細表示 (View details) ボタン:**
    再利用可能要素のデータ構造、品質、分布、リネージに関するシステム生成のインサイトを含むモーダルを開きます。詳細は、このドキュメントの「[Data details](#data-details)」セクションを参照してください。
* **
#### 3-3. データモデルの作成と管理 (Create and manage data models)

データモデルを構築して、テーブル要素と入力テーブル要素のコレクションを作成し、それらを組織全体のワークブックや他のデータモデルでデータソースとして参照することができます。使い慣れたワークブック形式のフォーマットにより、データモデルの権限を合理化しつつ、データを簡単に変換・分析できます。

このドキュメントでは、データモデルの作成と管理の方法について説明します。データモデルの概念に関する情報については、「[Get started with data modeling](https://help.sigmacomputing.com/docs/get-started-with-data-modeling)」を参照してください。

データモデルを作成した後、それをカスタマイズし、機能をさらに拡張して、アナリストやビジネスユーザーに以下のことを可能にできます。
* パラメータを使用してワークブックからデータモデルに値を渡す
* データモデルでリレーションシップを定義する
* メトリクスを作成・管理する
* 列レベルのセキュリティを構成する

> 📘
> Sigmaは、データモデルが完全に開発され、シームレスな移行が促進できるようになるまで、以前のデータセットバージョン（レガシーデータセット）を引き続きサポートします。レガシーデータセットに関する情報については、「[Create and manage datasets](https://help.sigmacomputing.com/docs/create-and-manage-datasets)」を参照してください。

**ユーザー要件 (User requirements)**

データモデルを作成または管理する機能には、以下が必要です。
* `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
* あなたはデータモデルの所有者であるか、そのデータモデルに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-data-model)を付与されている必要があります。

**再利用可能な要素でデータモデルを作成する (Create a data model with reusable elements)**

データモデルを作成するには、以下を実行します。

1.  **ホーム**ページに移動します。
2.  `Create New` をクリックし、メニューから `Data Model` を選択します。
3.  新しいデータモデルが**ワークブックページ**で開きます。以下のいずれかの方法でデータを追加します。
    * **`Add element` バーで、`Data > Table` または `Input` を選択し、入力テーブル要素を選びます。**
        テーブルまたはリンクされた入力テーブルを選択した場合、要素のデータソースを選択します。データソースは、あなたのデータプラットフォームからのデータ、CSVアップロード、カスタムSQL、または任意のデータモデルの既存要素にすることができます。
        > 📘
        > ソースに適用された将来のデータレベルの変更は、データモデルに反映させることができます。フィルタのような一部の変更は自動的に継承されます。追加または削除された列のような他の変更については、データモデルのワークブックページを再度開くとSigmaがプロンプトを表示します。それらの他の変更については、プロンプトに従って変更を無視するか、再利用可能な要素を更新するかを選択できます。非表示の列や列のグループ化のような表示レベルの変更は継承されません。
    * **既存のワークブックまたはデータモデルからテーブルまたは入力テーブル要素をコピー＆ペーストします。** 詳細は、「[Copy and paste elements](https://help.sigmacomputing.com/docs/copy-and-paste-elements)」を参照してください。
        > 📘
        > コピー＆ペーストから作成された再利用可能な要素は、元のコピーされた要素とは同期されず、元の要素に適用された将来の変更を反映しません。
4.  [任意] 必要に応じて、追加の再利用可能な要素を作成し、データを変換します。ワークブックと同様に、列のグループ化、値の集計、子要素の作成、コントロール要素の追加などができます。
5.  新しい再利用可能な要素を保存するには、`Publish` をクリックします。

データモデルが正常に保存されると、**概要ページ**が開きます。その後、各再利用可能要素をプレビューし、[データモデルの管理を続ける](https://help.sigmacomputing.com/docs/create-and-manage-data-models#manage-an-existing-data-model)ことができます。

**ワークブックのテーブルからデータモデルを作成する (Create a data model from a workbook table)**

ワークブック内のテーブルからデータモデルを作成することもできます。例えば、CSV形式のファイルをワークブックに直接アップロードし、そのファイルのデータを別のワークブックで再利用したい場合、CSV形式のファイルをデータソースとするテーブル要素からデータモデルを作成できます。

1.  データモデルに変換したいテーブル要素があるワークブックを開きます。
2.  要素を右クリックするか、要素の上にカーソルを合わせて `More` をクリックします。
3.  `Advanced options > Create data model...` を選択します。
4.  表示された `Create data model` モーダルで、`Next` をクリックします。
5.  `Add to a new data model` モーダルで、データモデルの名前を入力し、データモデルを整理するための保存先を選択します。
6.  `Create` をクリックします。データモデルが新しいタブで開きます。

**データモデルで変更された列をマッピングする (Map changed columns in a data model)**

データモデル要素の列にいくつかの変更を加えると、ワークブックや他のデータモデルなどの下流の要素で、次のようなエラーが表示されることがあります： `Unknown column [columnID]`, `Column [ColumnID] does not exist`, または `Reference to errored column: [columnID]`。変更例としては以下のようなものがあります。
* テーブルから列を削除する。
* テーブルから列を削除し、その後ソース列のリストから再度追加する。
* 結合されたテーブルから新しいテーブルへなど、要素のソースを変更する。

これらのエラーが、データモデル要素をソースとして使用するデータモデルやワークブックに表示されるのを防ぐため、Sigmaはこれらの変更を検出し、データモデルを公開する際に変更された列をマッピングするよう促します。

変更された列をマッピングするには、以下を実行します。
1.  データモデルを編集中に、下流の要素でエラーを引き起こす可能性のあるテーブルへの変更を加えます。
2.  データモデルを公開します。
3.  `Map columns` モーダルが表示されます。
4.  影響を受けるテーブルの変更された列を確認し、任意で、公開バージョンのデータモデル内の変更された列を、公開予定のドラフト内の置換列にマッピングします。デフォルトでは、変更された列は `No match` にマッピングされ、これにより下流の要素で列がエラーとなります。
    * *例えば、`Normalized Price` という複雑な計算列を更新したい場合、更新された計算ロジックを持つ `Revised Normalized Price` という新しい列を追加し、前の列を削除します。データモデルを公開する際、`Normalized Price` 列を `Revised Normalized Price` 列にマッピングします。*
    * *`Normalized Price` 列を置換列にマッピングせずにデータモデルから削除するには、デフォルトの `No match` の選択のままにします。*
5.  すべての影響を受けるテーブルの関連するすべての列のマッピングが完了したら、`Save and publish` を選択します。

* **トラブルシューティング：列を選択できない (Troubleshooting: Unable to select column)**
    変更された列を別の列にマッピングしたいが、選択できない場合は、以下を実行します。
    1.  `Map columns` モーダルで、`No matches` トグルをオフにします。
    2.  新しい列を `No match` にマッピングし、その後、削除された列を新しい列にマッピングします。
        * *例えば、`Revised Normalized Price` を `No match` にマッピングし、その後、削除された列 `Normalized Price` を置換列 `Revised Normalized Price` にマッピングします。*
    > 🚩
    > `No match` にマッピングされた列は、このテーブルをデータソースとして使用するデータモデルやワークブックで列エラーを引き起こす可能性があります。

* **トラブルシューティング：列がリストされていない (Troubleshooting: Column is not listed)**
    マッピングしたい変更された列が `Map columns` モーダルにリストされていない場合、そのデータモデルは以前に列をマッピングせずに公開されています。
    既に公開された列を別の列にマッピングしたい場合は、データモデルのドラフトを以前のバージョンに復元して再公開し、その後で列を再マッピングする必要があります。
    * *例えば、`Normalized Price` 列を削除してデータモデルを公開したとします。データモデルを公開した際、その列を `No match` にマッピングしました。*
    * *後で、`Revised Normalized Price` 列を作成し、`Normalized Price` 列を新しい列にマッピングしたいが、それがマッピング対象として利用できない場合。*
    * *この例では、データモデルを `Normalized Price` 列を削除する前のバージョンにドラフトとして復元し、その後、変更の間に公開せずに新しい列を追加し、前の列を削除する必要があります。そして、ドラフトを公開する際に `Map columns` モーダルが表示され、`Normalized Price` を `Revised Normalized Price` にマッピングすることができます。*
    データモデルの以前のバージョンをドラフトとして復元する詳細については、「[Document versions and version history](https://help.sigmacomputing.com/docs/document-versions-and-version-history)」を参照してください。

**既存のデータモデルを管理する (Manage an existing data model)**

データモデルのメタデータに変更を加えたり、データモデルを他の人と共有したり、データモデル内のデータソースに変更を加えたりすることができます。また、データモデルを削除したり、削除されたデータモデルを復元したりすることもできます。

* **データモデルの名前を編集する (Edit a data model's name)**
    メンバーがデータモデルを検索・識別しやすくするために、一意の名前を選択します。
    1.  編集したいデータモデルを開きます。
    2.  データモデルのヘッダーで、ドキュメント名を選択し、`File > Rename` を選択します。
    3.  ドキュメント名が編集可能になります。
    4.  データモデルの名前を変更し、`Enter` を押すか、どこかをクリックして変更を適用します。
    5.  データモデルを公開して、名前の変更を下流で利用可能にします。

* **データモデルの説明を編集する (Edit a data model’s description)**
    データモデルとその要素にコンテキストを追加するために、説明を入力します。
    1.  データモデルを開きます。
    2.  **概要ページ**のサイドバーにある `About the data model` セクションで、説明フィールドをクリックしてテキストを更新します。Sigmaは変更を即座に適用します。

* **データモデルを共有する (Share the data model)**
    組織のメンバーが要素をデータソースとして使用できるように、データモデルを共有します。特定のデータモデルを使用するアクセス権が付与されていないユーザーは、ワークブックや他のデータモデルでその要素

  #### 3-4. データモデルでリレーションシップを定義する (Define relationships in data models)

データモデル内のテーブル間にリレーションシップを追加することで、ビジネスユーザーがアドホックな結合を行うことなく、関連データを扱うことを可能にできます。

リレーションシップは、Sigmaがテーブルを結合する際に使用する結合ロジックを定義します。2つのテーブル間にリレーションシップを定義した後、両方のテーブルの列は、必要に応じて分析や探索のためにソーステーブルで利用可能になります。ユーザーがワークブックでソーステーブルを分析し、関連する列を追加すると、Sigmaは結合を実行します。

リレーションシップは、不要な結合を減らすのに役立ち、これによりパフォーマンスが向上し、コストを削減できます。リレーションシップを使用すると、結合は関連する列がワークブック要素に追加されたときにのみ実行されます。代わりに結合を使用すると、結合は毎回、基盤となるSQLで実行されます。

Sigmaは、接続されたデータソースからテーブル間のリレーションシップを自動的に作成しません。テーブルに主キーと外部キーが定義されていても、関連する列を下流の要素で利用可能にするためには、データモデル内でテーブル間のリレーションシップを作成する必要があります。

> 💡
> 要素間のリレーションシップには方向性があります。リレーションシップを定義する際には、データがどのように関連しているかを考慮してください。

**リレーションシップをモデリングするためのガイダンス (Guidance for modeling relationships)**

データモデルのテーブル間のリレーションシップは、多対一（many-to-one）または一対一（one-to-one）の結合のみをサポートします。データモデル内のテーブル間にリレーションシップを定義する場合、最も粒度の細かいデータテーブルをソース要素として使用し、一つ以上のより粗い粒度のテーブルをターゲット要素としてリレーションシップを追加します。ソーステーブルの各行は、ターゲットテーブルで可能な結果が一つだけでなければなりません。そうしないと、意図しないファンアウトや誤った結果が、関連する列を使用するワークブックに導入される可能性があります。

例えば、[スター スキーマ](https://en.wikipedia.org/wiki/Star_schema)を使用する場合、ファクトテーブル（例：EVENTS）をソース要素として使用し、各ディメンションテーブル（例：USER、またはEVENT_TYPE）とのリレーションシップをターゲット要素として追加します。

詳細は、Sigmaコミュニティの「[Relationships: what they are and how to use them](https://community.sigmacomputing.com/data-modeling/relationships-what-they-are-and-how-to-use-them-4332)」を参照してください。

**2つのデータモデルテーブル間にリレーションシップを追加する (Add a relationship between two data model tables)**

追加の列をデータモデル要素から利用可能にするために、リレーションシップを定義します。

> 📘
> 同じ接続上の要素間にのみリレーションシップを定義できます。すべての関連要素は、同じデータモデル内にある必要があります。

1.  編集のためにデータモデルを開きます。
2.  データモデルに要素を追加します。
3.  `Data model ERD` () を選択して、エンティティ関係図（ERD）ビューを開きます。
4.  `Data model ERD` ビューで、キャンバス上のリレーションシップのソース要素を選択します。
5.  エディタパネルで、`Modeling` タブを選択します。`Relationships` セクションで、`+` (リレーションシップを追加) を選択します。
6.  `Add a relationship` モーダルが開きます。
7.  [任意] リレーションシップに名前を付けます。デフォルトでは、リレーションシップ名はターゲット要素のタイトルを使用します。
8.  [任意] リレーションシップに説明を追加します。
9.  `Target source` で、リレーションシップのターゲットとして追加するデータモデル内の要素を選択します。要素をターゲットとして追加すると、その列がソース要素から利用可能になります。
    > 💡
    > ターゲットソースは、ソースとして無効化された要素にすることができます。ターゲットソースが無効化されている場合、下流のユーザーがその要素の列を扱う唯一の方法は、このリレーションシップを通じてです。
10. `Join keys` で、リレーションシップの結合キーとして使用するソース要素とターゲット要素の列を選択します。
11. [任意] `+ Add another mapping` をクリックして、さらに列マッピングを追加します。
12. [任意] ソース要素とターゲット要素のキーマッチングの詳細を確認して、リレーションシップが正しいキーで設定されていることを検証します。`Result preview` を選択して、リレーションシップの出力が期待通りに見えることを確認します。
13. `Save` をクリックします。
14. リレーションシップを下流のユーザーが利用できるようにするには、データモデルを公開します。

ワークブックで関連する列を使用する方法の詳細については、「[Use related columns in a workbook](https://help.sigmacomputing.com/docs/use-related-columns-in-a-workbook)」を参照してください。

**リレーションシップの例 (Example relationship)**

例えば、SigmaサンプルデータベースのBIKESデータをワークブックでより簡単に分析したい場合、次のようにモデリングしてリレーションシップを定義できます。
1.  あなたのデータモデルで、Sigmaサンプルデータベースの `EXAMPLES.BIKES` スキーマをデータソースとして使用し、`TRIP` テーブルと `STATIONS` テーブルを2つのデータ要素として追加します。
    * `TRIP` テーブルは、レンタルバイクでのバイクトリップに関する詳細を提供します。バイクトリップごとに1行あり、各ステーションに対して多くの合計行があります。
    * `STATIONS` テーブルは、各バイクドッキングステーションの場所に関する詳細を提供します。各ステーションごとに1行あります。
2.  2つのテーブル間にリレーションシップを作成するには、`TRIP` テーブルから始め、`STATIONS` テーブルをターゲット要素として使用します。この方向でリレーションシップを作成すると、多対一（many-to-one）結合のロジックが定義されます。
3.  その後、データモデルを公開すると、ビジネスアナリストはデータモデルから `TRIP` テーブルを扱い、`STATIONS` テーブルから関連する列を簡単に追加できます。Sigmaはリレーションシップで定義されたロジックに基づいて結合を実行し、その結合は関連する列がワークブックに追加されたときにのみ実行されます。

**データモデル要素の既存のリレーションシップを確認する (Review existing relationships for data model elements)**

データモデルのエンティティ関係図（ERD）を使用して、データモデル要素間のリレーションシップを確認できます。
* 要素を接続する矢印で方向性のあるリレーションシップを識別します。各リレーションシップには個別の矢印があります。
* 矢印を選択すると、リレーションシップと、ソースおよびターゲット要素の関連するキーがハイライトされます。
* どのリレーションシップが、再利用可能要素のどの列に対して設定されているかを識別します。

* #### 3-6. メトリクスの作成と管理 (Create and manage metrics)

メトリクスは、データソースを共有するデータ要素間で再利用できる、カスタムの集計計算です。接続されたデータベースやカタログのデータモデル、データセット、またはテーブルでメトリクスを定義すれば、ユーザーが一貫した方法で簡単かつ効率的に計算を実行するのを助けることができます。

このドキュメントでは、メトリクスのガバナンスを向上させるためのメトリクスの作成と管理の方法について説明します。ワークブックのデータ要素でメトリクスを使用する方法については、「[Use metrics in a workbook](https://help.sigmacomputing.com/docs/use-metrics-in-a-workbook)」を参照してください。

制限事項やベストプラクティスを含むメトリクスの詳細については、「[About metrics](https://help.sigmacomputing.com/docs/about-metrics)」を参照してください。

**ユーザー要件 (User requirements)**

* **データモデル**でメトリクスを作成・管理する機能には、以下が必要です。
    * `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
    * あなたはデータセットの所有者であるか、そのデータモデルに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-data-model)を付与されている必要があります。

* **データセット**でメトリクスを作成・管理する機能には、以下が必要です。
    * `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
    * あなたはデータセットの所有者であるか、そのデータセットに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-dataset)を付与されている必要があります。

* **データベースまたはカタログのテーブル**でメトリクスを作成・管理する機能には、以下が必要です。
    * 特定のテーブルに対する `Can use & annotate` [データアクセス権](https://help.sigmacomputing.com/docs/data-permissions)が付与されているか、または該当する接続、データベース、カタログ、スキーマレベルで付与された権限を継承している必要があります。

**データモデルでメトリクスを扱う (Work with metrics in data models)**

データモデルでメトリクスを追加、ハイライト、更新します。

* **データモデルでメトリクスを作成する (Create a metric in a data model)**
    1.  編集のためにデータモデルを開きます。
    2.  メトリクスを追加したいデータモデル要素を選択します。
    3.  エディタパネルで、`Modeling` タブを選択します。
        > 💡
        > `Modeling` タブが表示されない場合は、`Element Properties` の `Metrics` タブでもメトリクスを追加できます。
    4.  `Metrics` セクションで、`+` (メトリクスを追加) を選択します。
    5.  `Add a metric` モーダルが表示されます。
    6.  `Name` フィールドに、メトリクスに使用する名前を入力します。
    7.  `Description` フィールドに、メトリクスが何をするかの説明を入力します。この説明は、ユーザーがメトリクスにカーソルを合わせたときに表示されます。
    8.  `Formula` フィールドで、メトリクスのロジックを定義します。Sigmaの関数を使用したり、データモデルのテーブル内の任意の列を参照したり、別のメトリクスを参照したりできます。
    9.  [任意] `Timeline` スイッチをオンにすると、**データモデルの概要**ページにメトリクスのタイムラインが表示されます。
        * `Date` で、タイムラインに使用するデータ内の日付列を選択します。
        * `Truncation` で、日付をどのように切り捨てるかを選択するか、日付の切り捨てを削除して日付列の既存の粒度を使用するかを選択します。
    10. [任意] `Compare period` で、メトリクスの比較期間を選択するか、`None` を選択します。
    11. [任意] `Direction` で、比較トレンドの方向を選択するか、`None` を選択します。
    12. メトリクスの `Preview` を確認し、任意でメトリクスの出力フォーマットを定義します。
        * 例えば、数式の結果を通貨やパーセンテージとして指定したり、小数点以下の桁数を設定したり、数値フォーマットメニュー()をクリックして完全なフォーマットメニューからオプションを選択したりできます。
        > 📘
        > メトリクスは集計計算を定義します。プレビューがnull値を表示する場合、あなたの数式には `Sum()`, `Avg()`, `Count()` などの集計関数が欠けている可能性があります。
    13. データモデルを公開して、変更を下流で利用可能にします。

* **データモデルの概要でメトリクスをハイライトする (Highlight a metric in the data model overview)**
    デフォルトでは、データモデルで作成した最大6つのメトリクスが**データモデルの概要**ページに表示されます。どのメトリクスを表示するかを変更するには、概要ページで特定のメトリクスをハイライトして、それらだけを表示するように選択できます。
    1.  編集のためにデータモデルを開きます。
    2.  メトリクスを追加したいデータモデル要素を選択します。
    3.  エディタパネルで、`Modeling` タブを選択します。
    4.  エディタパネルの `Modeling` タブの `Metrics` セクションで、メトリクスを探します。
    5.  そのメトリクスについて、`More` () をクリックし、`Highlight in overview` を選択します。
    6.  データモデルを公開して、変更を利用可能にします。
    ハイライトされたメトリクスは、データモデルへのアクセス権を持つ誰もが探索できます。詳細は、「[Navigate data models](https://help.sigmacomputing.com/docs/navigate-data-models)」を参照してください。

* **データモデルでメトリクスを編集する (Edit a metric in a data model)**
    メトリクスを修正するには、以下を実行します。
    1.  編集のためにデータモデルを開きます。
    2.  メトリクスが定義されているテーブルを選択します。
    3.  エディタパネルの `Modeling` タブの `Metrics` セクションで、メトリクスを探します。
    4.  `(Edit metric...)` をクリックします。
    5.  必要な変更を加え、`Save` をクリックします。
    6.  データモデルを公開して、変更を下流で利用可能にします。
        * メトリクスを使用する列や他のメトリクスは、改訂されたメトリクスを使用するように更新されます。

* **データモデルでメトリクスを削除する (Delete a metric in a data model)**
    メトリクスを削除するには、以下を実行します。
    1.  編集のためにデータモデルを開きます。
    2.  メトリクスが定義されているテーブルを選択します。
    3.  エディタパネルの `Modeling` タブの `Metrics` セクションで、メトリクスを探します。
    4.  そのメトリクスについて、`More` () をクリックし、`Delete` を選択します。
    5.  データモデルを公開して、変更を下流で利用可能にします。
        * 削除されたメトリクスに依存する列やメトリクスは、エラーを表示します。

**データセットでメトリクスを扱う (Work with metrics in datasets)**

データセットおよびデータセット内のメトリクスは、一般的に利用可能です。

* **データセットでメトリクスを作成する (Create a metric in a dataset)**
    メトリクスを作成するには、以下のステップに従います。
    1.  データセットまたはデータベースのテーブルを開きます。
    2.  ヘッダーで `Edit` をクリックします。
    3.  `Metrics` タブを選択し、`Create Metric` をクリックしてメトリクスビルダーを開きます。
    4.  `Name` フィールドに、メトリクスの名前を入力します。
    5.  `Description` フィールドに、メトリクスの詳細を入力します。この情報は、ユーザーがワークブック要素にメトリクスを適用するときに表示されます。
    6.  `Formula` フィールドで、メトリクスのロジックを定義します。Sigmaの関数を使用したり、開いているデータセットやデータベースのテーブル内の任意の列を参照したりできます。データセットの既存のメトリクスを使用することもできます。これは、データセット内で再利用可能な計算コンポーネントを構築するための非常に強力な方法です。
    7.  クイックフォーマットツールとプレビューを使用して、メトリクスの出力をカスタマイズします。
        * 例えば、数式の結果を通貨やパーセンテージとして指定したり、小数点以下の桁数を設定したり、数値フォーマットメニュー()をクリックして完全なフォーマットメニューからオプションを選択したりできます。
        * メトリクスは集計計算を定義します。メトリクスビルダーのプレビューが `null` 値を返す場合、あなたの数式には `Sum()`, `Avg()`, `Count()` などの集計関数が欠けている可能性があります。
    8.  ヘッダーで `Publish` をクリックしてメトリクスを保存します。

* **データセットでメトリクスを編集する (Edit a metric in a dataset)**
    メトリクスを編集すると、Sigmaは特定のデータセットやデータベースのテーブルにリンクするワークブック要素に変更を反映させます。メトリクスへの全てのワークブック参照には名前と説明の変更が含まれ、Sigmaは数式の更新に基づいてメトリクスの結果を再計算します。
    メトリクスを編集するには、以下のステップに従います。
    1.  編集する予定のメトリクスを含むデータセットまたはデータベースのテーブルを開きます。
    2.  `Edit` をクリックします。
    3.  `Metrics` タブを選択します。
    4.  リストからメトリクスを探し、その名前をクリックしてメトリクスビルダーでメトリクスを開きます。
    5.  メトリクスの名前、説明、数式、フォーマットを必要に応じて編集し、`Publish` をクリックしてメトリクスを更新します。

* **データセットでメトリクスを削除する (Delete a metric in a dataset)**
    メトリクスを削除すると、ワークブック要素でのその計算は無効になります。テーブルは、以前メトリクスの出力を含んでいた列にエラーメッセージを表示します。ビジュアライゼーションとピボットテーブルは、要素の代わりにエラーメッセージを表示します。
    1.  削除する予定のメトリクスを含むデータセットまたはデータベースのテーブルを開きます。
    2.  `Edit` をクリックします。
    3.  `Metrics` タブを選択します。
    4.  メトリクスのリストから、削除する予定のメトリクスを探します。
    5.  そのメトリクスについて、`More` () をクリックし、`Delete` を選択します。
    6.  あるいは、メトリクスを選択してメトリクスビルダーを開き、サイドパネルでメトリクスを探します。メトリクスの名前の隣にある `Delete metric` () をクリックします。
 
    7.  #### 3-7. データカタログのレビューと管理 (Review and manage your data catalog)

Sigmaに接続されている各データソースについて、データカタログのレビューと管理ができます。Sigmaで利用可能なデータベースまたはカタログ、スキーマ、およびテーブルを探索し、テーブルや列に説明やその他のメタデータを追加します。

> 💡
> あなたのデータベースまたはカタログの情報スキーマにあるコメントは、Sigmaで自動的に利用可能になります。

テーブルバッジ、テーブルの説明、および列の説明は下流で利用可能であり、ビジネスユーザーが特定の分析で使用するテーブルや列について決定を下すのに役立ちます。

データプラットフォームからのデータをさらにモデリングするために、Sigmaでデータモデルまたはデータセットを作成することもできます。
* [テーブルからデータモデルを作成する](https://help.sigmacomputing.com/docs/create-and-manage-data-models#create-a-data-model-from-a-workbook-table)
* [テーブルからデータセットを作成する](https://help.sigmacomputing.com/docs/create-and-manage-datasets#create-a-dataset-from-a-table)

**システムとユーザー要件 (System and user requirements)**

Sigmaでデータカタログを管理する機能には、以下が必要です。
* あなたの組織が[データソースに接続されている](https://help.sigmacomputing.com/docs/connect-to-data-sources)必要があります。
* あなたは `Manage connections` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
* あなたは接続に対する `Can use & annotate` [アクセス権](https://help.sigmacomputing.com/docs/data-permissions)を付与されている必要があります。

**メタデータでテーブルを注釈する (Annotate tables with metadata)**

テーブルの説明、認定ステータスを示すバッジ、列の説明とデータ型、追加の列設定の構成など、Sigmaでデータカタログのテーブルにメタデータを追加します。
テーブルと列の説明は、ワークブックで特定の列にカーソルを合わせるか、データソースとしてデータベーステーブルを使用するデータモデルのリネージを表示する際に、データテーブルと対話するビジネスユーザーに表示されます。

* **関連テーブルを見つける (Find relevant tables)**
    まず、注釈を付けたい関連テーブルを探します。
    1.  Sigmaホームから `Connections` を選択して、接続されているデータソースのリストを開きます。
    2.  表示したいデータカタログを持つデータ接続を選択します。
    3.  左のナビゲーションパネルで、注釈を付けたいテーブルを検索または参照して探します。

* **テーブルの説明を追加する (Add table descriptions)**
    データカタログでテーブルを見つけたら、説明を追加します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  右上の `Edit` を選択します。
    4.  テーブル名の隣にある `More info` () を選択します。
    5.  表示されるポップオーバーで、`Description` フィールドに説明を入力します。
    6.  変更を保存するには、`Publish` を選択します。

* **バッジを追加または更新する (Add or update a badge)**
    データのステータス、品質、信頼性を示すために、認定バッジを追加または更新します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  テーブル名の隣にある `More info` () を選択します。
    4.  ポップオーバーで、`Badge` ドロップダウンからオプションを選択します。
    5.  [任意] バッジを選択すると、ポップオーバーに `Badge note` フィールドが表示されます。バッジに関するコンテキストを提供するためにメモを追加します。

    バッジは自動的に保存され、左パネルのテーブルアイコンに即座に反映されます。

* **列の説明を追加する (Add column descriptions)**
    データソースのユーザーに追加のメタデータとガイダンスを提供するために、列に説明を追加します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  右上の `Edit` を選択します。
    4.  `Columns` タブを選択します。
    5.  `Description` 列で、テーブル内の任意の列に説明を追加します。
    6.  変更を保存するには、`Publish` を選択します。

* **列をフォーマットする (Format columns)**
    列のデータのフォーマットを変更する（例えば、数値データを通貨フォーマットで表示するなど）には、テーブルで列をフォーマットします。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  右上の `Edit` を選択します。
    4.  `Columns` タブを選択します。
    5.  フォーマットしたい列を探します。
    6.  `Format` で、列に適用したいフォーマットオプションを選択します。フォーマットオプションは、列のデータ型に依存します。例えば、数値列の場合、`Currency` を選択します。
    7.  変更を保存するには、`Publish` を選択します。

 #### 3-8. データセット (Datasets - レガシー機能)

Sigmaでデータセット（CDWやDBMSのテーブルに基づくデータのコレクション）を使用して、データをモデリングします。

データセットは、一元管理された、共有可能なデータ定義として機能し、集計やその他のデータ操作を含むことができます。管理者は、ビジュアライゼーション、テーブル、ピボットテーブルのソースとしてワークブック分析で使用されるデータセットを定義します。

ワークブックは、基盤となるデータセットに適用された全ての変更を継承し、一貫性のある信頼できるメトリック計算を保証します。メトリックのロジックが更新を必要とする場合、一つの場所（データセット）で変更を適用すれば、該当する全てのワークブックが自動的に更新された計算を継承し、反映します。

**データのモデリング (Modeling data)**
* ベストプラクティス
* [テーブルに注釈を付ける](https://help.sigmacomputing.com/docs/annotate-tables)
* [データセットを作成する](https://help.sigmacomputing.com/docs/create-and-manage-datasets)
* [列を構成する](https://help.sigmacomputing.com/docs/configure-columns)
* [リンクを追加する](https://help.sigmacomputing.com/docs/add-links-to-datasets)
* [データセットのワークシート](https://help.sigmacomputing.com/docs/the-dataset-worksheet)
* [データを結合する](https://help.sigmacomputing.com/docs/join-data)

**共有と権限 (Sharing and permissions)**
* [権限タイプ](https://help.sigmacomputing.com/docs/permission-types)
* [データセットを共有する](https://help.sigmacomputing.com/docs/share-a-dataset)
* [アクセス権を修正または取り消す](https://help.sigmacomputing.com/docs/modify-or-revoke-access)
* [コンテンツへのアクセスリクエストに応答する](https://help.sigmacomputing.com/docs/respond-to-a-request-for-access-to-content)

**高度なモデリング (Advanced modeling)**
* [データセットのクエリを調査する](https://help.sigmacomputing.com/docs/examine-dataset-queries)
* [データセットのリネージ](https://help.sigmacomputing.com/docs/dataset-lineage)
* [Sigmaからウェアハウスデータを編集する](https://help.sigmacomputing.com/docs/edit-warehouse-data-from-sigma-deprecated)
* [データセットのウェアハウスビュー](https://help.sigmacomputing.com/docs/dataset-warehouse-views)
* [データセットのマテリアライゼーション](https://help.sigmacomputing.com/docs/dataset-materialization-api)

**モデリングのベストプラクティス (Modeling Best Practices)**

**関連リソース (Related resources)**
* [データセットのクエリを調査する](https://help.sigmacomputing.com/docs/examine-dataset-queries)
* [データセットのリネージ](https://help.sigmacomputing.com/docs/dataset-lineage)
* [Sigmaからウェアハウスデータを編集する（非推奨）](https://help.sigmacomputing.com/docs/edit-warehouse-data-from-sigma-deprecated)
* [データセットのウェアハウスビュー](https://help.sigmacomputing.com/docs/dataset-warehouse-views)
* [データセットのマテリアライゼーションAPI](https://help.sigmacomputing.com/docs/dataset-materialization-api)

#### 3-9. データセットの作成と管理 (Create and manage datasets)

Sigmaでデータをモデリングしたい場合、データセットを作成することができます。データセットを作成すると、数式、データ変換、フィルタ、グルーピング、およびパラメータを、他の人がその上で構築できるリッチなデータソースにまとめることができます。また、[データセットをマテリアライズする](https://help.sigmacomputing.com/docs/dataset-materialization-api)ことで、データ分析を加速させるのに役立ちます。

> 💡
> データセットの代わりにデータモデルを作成することを検討してください。データモデルは、リレーションシップ（リンク）、メトリクス、列レベルのセキュリティ（CLS）のような主要なデータセットの機能を改善し、他のモデラーとのライブ編集、エンティティ関係図（ERD）などの新機能を追加します。「[Get started with data modeling](https://help.sigmacomputing.com/docs/get-started-with-data-modeling)」を参照してください。

データプラットフォームのテーブル、CSVファイル、またはカスタムSQLステートメントからデータセットを作成できます。
* [テーブルからデータセットを作成する](https://help.sigmacomputing.com/docs/create-and-manage-datasets#create-a-dataset-from-a-table)
* [CSVファイルからデータセットを作成する](https://help.sigmacomputing.com/docs/upload-csv-data)
* [SQLからデータセットを作成する](https://help.sigmacomputing.com/docs/create-a-dataset-from-sql)

**ユーザー要件 (User requirements)**

データセットを作成・管理するには、`Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。

**テーブルからデータセットを作成する (Create a dataset from a table)**

接続されたデータソースのテーブルからデータセットを作成するには：
1.  Sigmaホームから `Connections` を選択して、接続されているデータソースのリストを開きます。
2.  表示したいデータカタログを持つデータ接続を選択します。
3.  左のナビゲーションパネルで、テーブルを検索または参照して探します。
4.  テーブル名を選択してテーブルを開きます。
5.  `Explore` の隣にあるキャレット()を選択して `Use this table` を選び、次に `Create Dataset` を選択します。
6.  データセットに名前を付け、保存する場所を選択し、`Create` をクリックします。

**データセットのメタデータを修正する (Modify dataset metadata)**

データセットのメタデータを修正して、使用ガイダンス付きの説明を追加したり、特定の列のドキュメントを提供したり、例えばデータセットの内容が高品質であること、非推奨であること、または無関係であることをラベル付けするためにバッジを適用したりすることができます。

* **データセットの説明を追加する (Add a dataset description)**
    データセットに説明を追加するには：
    1.  データセットを開き、`Edit` を選択します。
    2.  データセット名の隣にある `More info` () を選択します。
    3.  `Description` フィールドに、データセットの説明を入力します。
    4.  説明を保存するには、データセットを公開します。

* **データセットのバッジを追加または更新する (Add or update a dataset badge)**
    データのステータス、品質、信頼性を示すために、認定バッジを追加または更新します。
    1.  データセットを開きます。
    2.  ヘッダーで `More info` () を選択します。
    3.  ポップオーバーで、`Badge` ドロップダウンからオプションを選択します。
    4.  [任意] バッジを選択すると、ポップオーバーに `Badge note` フィールドが表示されます。バッジに関するコンテキストを提供するためにメモを追加します。
    
    バッジは自動的に保存され、データセットのヘッダーに即座に反映されます。

**データセットを削除する (Delete a dataset)**

データセットを削除するには、あなたがデータセットの所有者であるか、データセットに対する `Can edit` アクセス権を持っているか、`Admin` アカウントタイプを割り当てられている必要があります。
1.  データセット名の隣にあるキャレット()をクリックし、次に `Delete...` をクリックします。
2.  `Confirm Deletion` モーダルで、`Delete` をクリックします。

**削除されたデータセットを復元する (Recover a deleted dataset)**

削除されたデータセットを復元するには、あなたがデータセットの所有者であるか、`Admin` アカウントタイプを持っている必要があります。
1.  **ホーム**ページに移動します。
2.  ナビゲーションメニューで、`Trash` を選択します。
3.  `Trash` ページで、削除されたドキュメントのリストを検索し、復元したいものをクリックします。`Name`, `Deleted on`, `Deleted by` の列をソートして、該当するドキュメントを特定するのに役立てることができます。
4.  `Document has been deleted` モーダルで、`Recover` をクリックします。Sigmaは復元されたドキュメントを即座に開きます。

5.  #### 3-10. データセットのベストプラクティス (Dataset best practices)

* **レベルを最小限にする (Minimize Levels)**
    データセットのワークシートタブにあるすべてのレベルは、そのデータセットを基に作成されたワークシートではフラット化されます。混乱を防ぐため、主要な計算に必要なレベルのみを作成してください。

* **フィルターを考慮する (Consider Your Filters)**
    最も関連性の高いデータを表示するためにフィルターを適用すると、インサイト発見のプロセスがはるかに速くなります。マテリアライゼーションと組み合わせると、クエリの実行も速くなります。最良のフィルターとは、制限しすぎることなく、無関係なデータを削減するものです。

* **データセットを説明する (Describe the Dataset)**
    もしデータセットが特定のユースケースの基盤として構築された場合、良いタイトルと説明は、人々にそのユースケースが何であるかを知らせます。データセットがいつ使用されるべきで、いつ使用されるべきでないかを明確にすることが重要です。

* **マテリアライズする (Materialize)**
    データセットのマテリアライゼーションを設定している場合は、使用しているデータがデータベースでいつ更新されるかを確認してください。データベースの更新後に更新スケジュールが発生するように設定したいはずです。

#### 3-11. チュートリアル：データセットを使用したデータモデリング (Tutorial: Data modeling with datasets)

データチームは、ビジネスユーザーによるデータ探索を可能にするためにデータセットを作成することが多いですが、データセットは多くの理由で作成されます。例えば以下のような理由です。
* ディメンショナルモデルの結合とフラット化
* 機密データのマスキング
* パフォーマンス向上のためのデータのマテリアライズ
* 共通の計算や重要業績評価指標（KPI）の一貫性を確保する

このステップバイステップガイドでは、ディメンショナルモデルをフラット化するデータセットの作成手順を説明します。

**要件 (Requirements)**

* あなたはCreatorアカウントタイプ、またはモデリング権限を含むカスタムアカウントタイプを割り当てられている必要があります。

**データセットを作成する (Create Datasets)**
1.  ホームページの上部で、`Create New` をクリックし、`Dataset` を選択します。
2.  `Select a Data Source` ページで、`Table` オプションを選択します。
3.  左パネルのConnectionsセクションを見つけ、`Sigma Sample Database` を選択します。
4.  `Examples` データベースと `PLUGS_ELECTRONICS` スキーマを探します。
5.  `F_POINT_OF_SALE` テーブルをクリックして、データのプレビューを表示します。
6.  ページヘッダーの右上隅にある `Get Started` をクリックします。

**データをモデリングする (Modeling Data)**

* **計算を作成する (Create Calculations)**
    データセットを構築するためのテーブルを見つけたので、次に追加の列に計算を追加します。データセットに計算列を追加することで、組織によるメトリクスやKPIの計算方法の一貫性が保証されます。計算列は、アナリストが毎回共通の計算をワークブックに追加する必要がなくなるため、貴重な時間節約になります。
    1.  画面上部の `Worksheet` タブをクリックします。
    2.  `Sales Amount` 列のキャレットアイコン()をクリックします。
    3.  `Add New Column` をクリックします。
    4.  数式バーに `[Sales Amount] * [Sales Quantity]` と入力します。
    5.  キーボードの `Enter` をクリックします。
    6.  新しい列の名前をダブルクリックし、`Revenue` に変更します。
    7.  `Revenue` 列のキャレットアイコン()をクリックします。
    8.  `Format` を選択します。
    9.  `Currency` を選択します。
    10. ステップ1-5を繰り返し、`COGS` (Cost of Goods Sold) という名前の別の列を追加します。
        * 数式バーに `[Cost Amount] * [Sales Quantity]` と入力します。
    11. キーボードの `Enter` をクリックします。
    12. `COGS` 列のキャレットアイコン()をクリックし、`Format` を選択します。
    13. `Currency` を選択します。

* **追加のテーブルを結合する (Joining additional tables)**
    このデータセットに追加のテーブルを結合して、上記で作成したデータセットにさらなるコンテキストを追加しましょう。
    Sigmaはleft, right, full, inner joinタイプ、およびlookupをサポートしています。複数の列を結合したり、結合内で任意の関数（例：日付の切り捨て）を定義したりすることもできます。詳細は「[Join types](https://help.sigmacomputing.com/docs/join-data#join-types)」を参照してください。
    1.  データセットが編集モードの状態で、データベースアイコンをクリックしてそのタブを開きます。これは右側のパネルにあります。
    2.  データベースアイコンの下にあるプラスアイコン()をクリックします。これにより `Add Source` ページが開きます。
    3.  データソースタイプとして `Table` を選択します。
    4.  ページの左側、`Connections` の下で、`Sigma Sample Database` を選択します。
    5.  `Examples` データベースと `PLUGS_ELECTRONICS` スキーマを探します。
    6.  `F_SALES` テーブルをクリックしてデータのプレビューを表示します。
    7.  ページヘッダーの右上隅にある `Next` をクリックします。
    8.  `Join Type` で、デフォルトの `Left Join` を使用します。
    9.  左の結合キーセレクタを `ORDER_NUMBER` 列に設定します。
    10. 右の結合キーセレクタを `ORDER_NUMBER` 列に設定します。
        * *注：Sigmaは両方のテーブルに同名の列を見つけた場合、これらのフィールドを自動的に入力します。*
    11. `Done` をクリックして、データセットのワークシートに戻ります。
        * *注：左側のパネルを見ると、`F_SALES` からの列がワークシートに存在し、`F_SALES` テーブルがデータソースとしてリストされていることがわかります。*
    12. 以下の各テーブルについて、ステップ2から5を繰り返します。
        * **D_STORE**
            * Join Key: `STORE_KEY`
            * Columns: `STORE_NAME`, `STORE_CITY`, `STORE_STATE`, `STORE_JSON_FIELD`
        * **D_CUSTOMER**
            * Join Key: `CUST_KEY`
            * Columns: `CUST_NAME`, `CUST_JSON_FIELD`
        * *注：結合を介して追加されたすべての列には、括弧内にテーブル名が付加されます。列名をダブルクリックして名前を変更します。列をワークシートの新しい位置にドラッグして移動します。*

* **JSONを抽出する (Extracting JSON)**
    SigmaではJSONを抽出する機能があります。
    1.  `Cust Json Field (D_CUSTOMER)` 列のキャレットアイコン()をクリックします。
    2.  `Extract Columns` を選択します。
    3.  `Extract Fields` モーダルで、`AGE_GROUP` と `LOYALTY_PROGRAM` フィールドを選択します。
    4.  `LOYALTY_PROGRAM` のキャレットアイコン()をクリックします。
    5.  `Logical` を選択します。
    6.  `Confirm` ボタンをクリックします。

* **データをフィルタリングする (Filter Your Data)**
    データセットをフィルタリングすると、データ探索中にアナリストが利用できるデータの量が制限されます。
    * **相対日付フィルターを追加する**
        1.  `[Date (F_SALES)]` のキャレットアイコン()をクリックします。
        2.  `Add Filter` を選択します。
        3.  フィルタータイプとして `Date Range` を選択します。
        4.  `Select Date Range` フィールドをクリックして、日付選択メニューを表示します。
        5.  モーダルの左側で `Relative` を選択します。
        6.  テキスト入力フィールドに `1` と入力します。
        7.  `...` メニューで `Weeks` を選択します。
            * *注：このフィルターにより、データは常に最新の週にフィルタリングされます。*
        8.  `Save` をクリックします。
    * **テキストフィルターを追加する**
        1.  `Store State` 列のドロップダウン矢印をクリックし、`Add Filter` を選択します。
        2.  `Filter Values` ドロップダウンメニューをクリックします。
        3.  `California`, `Texas`, `Michigan` のチェックボックスをオンにします。
        4.  `Save` をクリックします。

* **テーブルをリンクする (Link Tables)**
    データセットでリンクを定義することにより、ユーザーは結合されたデータをワークブックに追加するオプションを得ます。さらに、SigmaはSnowflakeでリレーショナルメタデータ（外部キー）が定義されているテーブルを自動的にリンクします。
    1.  画面上部の `Links` タブをクリックします。
    2.  `Add links to other source` をクリックします。
    3.  左パネルの下部にある `Connections` をクリックします。
    4.  `Sigma Sample Database` を選択します。
    5.  `Examples` と `PLUGS_ELECTRONICS` フォルダを探します。
    6.  `D_PRODUCT` テーブルをクリックしてデータのプレビューを表示します。
    7.  `Next` をクリックします。
    8.  `Join Type` の選択を見つけ、`Left Join` を選択します。
    9.  左の結合キーセレクタを `PRODUCT KEY Link (F_POINT_OF_SALE)` に設定します。
    10. 右の結合キーセレクタを `PRODUCT KEY` に設定します。
    11. `Save` をクリックします。
    12. 画面上部の `Publish` ボタンをクリックして、すべてのデータセットの変更を保存します。

* **データセットにバッジを付ける (Badging Datasets)**
    データセットにバッジを追加して、コンテンツが `Endorsed`（推奨）、`Warning`（警告）、または `Deprecated`（非推奨）であることを示します。任意のバッジノートを使用して、すべての組織メンバーに追加のコンテキストを提供できます。
    * **バッジを追加または更新する**
        1.  ページヘッダーの情報アイコン()をクリックします。これにより、ページのポップアップが開きます。
        2.  ドロップダウンリストから `Endorsed` バッジタイプを選択します。

* **権限設定とデータセットの共有 (Setting Permissions & Sharing Datasets)**
    モデリングが完了したら、データセットを共有できます。ユーザーのチームや個人に[直接共有](https://help.sigmacomputing.com/docs/share-a-dataset#direct-share)するか、より広範に[ワークスペース](https://help.sigmacomputing.com/docs/share-a-dataset#move-to-workspace)に共有することができます。権限が付与されると、人々はデータセットを分析の基礎として使用できます。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
    * **直接共有 (Direct Share)**
        1.  画面上部の `Permissions` タブをクリックします。
        2.  `Add Permission` をクリックします。
        3.  メンバーのメールアドレスまたはチーム名を検索します。
        4.  選択したメンバーまたはチームに付与したい権限の種類を選択します。
            * *注：ユーザーはホームページの「Shared with Me」タブからデータセットにアクセスできるようになります。*
    * **ワークスペースへ移動 (Move to Workspace)**
        1.  データセットヘッダーの `More` をクリックします。
        2.  `Move` をクリックします。
        3.  `Workspaces` タブをクリックします。
        4.  データセットを移動したいワークスペースを選択します。
        5.  `Move` をクリックします。

* **マテリアライゼーション (Materialization)**
    マテリアライゼーションにより、データセットをテーブルとしてウェアハウスに書き戻すことができます。これらのテーブルは、Sigmaで構築する複雑なSQLクエリの簡略化版として機能し、下流のレポートの速度とパフォーマンスを向上させることができます。各テーブルは、設定したスケジュールでウェアハウスに書き込まれ、再書き込みされます。Sigmaはテーブルの上にビューを作成するため、Sigma外の他のアプリがSigmaの作成した準備済み/変換済みデータにアクセスできます。
    * **要件 (Requirements)**
        * データセットの接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。
        * あなたは組織のAdminである必要があります。
    * **データセットにマテリアライゼーションを追加する**
        1.  画面上部の `Materialization` タブをクリックします。
        2.  `Create Schedule` をクリックします。
        3.  データをマテリアライズする頻度を選択します。
        4.  `Save` をクリックします。
        マテリアライゼーションのスケジュールを保存すると、Sigmaは最初のマテリアライゼーションを実行します。
        スケジュールされた全てのマテリアライゼーションは、データセットの `Materialization` タブで表示できます。

#### 3-12. データセットワークシート入門 (Introduction to the Dataset Worksheet)

データセットのワークシートを使用すると、そのデータを構造化し、操作することができます。計算の作成、データのグループ化、フィルターやフォーマットの適用、パラメータの追加などが可能です。データセットのワークシートには、少なくとも一つのデータソースが含まれている必要があります。データソースの例としては、あなたの組織のデータウェアハウスのテーブル、アップロードされたCSV、さらには他のデータセットも含まれます。

**ワークシートタブの構成 (Worksheet Tab Anatomy)**

* **数式バー (The Formula Bar)**
    各ワークシートには、ページの上部近くに数式バーが配置されています。
    数式はセルではなく、列に適用されます。数式が列に適用されると、その列のすべての行に適用されます。
    データソースから直接データを参照している列を含め、すべての列には数式があります。列の数式を表示するには、その列を選択すると、数式バーに自動的にその数式が表示されます。
    ワークシートで新しい計算を作成するには、まず新しい列を追加し、その列に数式を追加する必要があります。Sigmaの最も[人気のある関数](https://help.sigmacomputing.com/docs/function-index)から始めてみましょう。

* **右側パネル (The Right Side Panel)**
    どのワークシートの右側にあるパネルにも、列ビューとデータソースリストの2つのコンポーネントがあります。
    * **列ビューパネル (The Column View Panel)**
        列ビューパネルには、ワークシート内の全列の完全なリストが含まれています。非表示に設定されていない限り、これらの列はすべてワークシートのスプレッドシートに表示されます。
        ここから、ワークシートの列を整理し、レベルにグループ化することができます。前述のスプレッドシートセクションで述べたように、レベル化されたグループを作成することで、選択した列の共通の特性に基づいてデータの行をまとめることができます。列ビューパネルからデータをグループ化すると、それらのグループは自動的にワークシートのスプレッドシートに反映されます。
        この列ビューパネルには、ワークシートの合計のためのセクションも含まれています。合計は、ワークシートの最上位レベルに存在する単一値の列集計です。
    * **データソースパネル (The Data Source Panel)**
        ワークシートの右側パネルにある2番目のタブをクリックすると、データソースパネルが開きます。このパネルには、ワークシートのデータソースが表示されます。ここから、データソースを編集したり、結合したりすることができます。
        各データソースにはその列のリストが含まれているため、ソースのドロップダウン列リストから、ワークシートに欠けているデータソースの列を追加することもできます。

* **コントロールパネル (The Control Panel)**
    ワークシートには、画面の左側に展開可能なコントロールパネルがあります。これには、ワークシートのフィルターとパラメータが含まれています。また、合計値が存在する場合は、それも含まれます。
  #### 3-13. データセットワークシートのコントロール (Dataset worksheet controls)

**ユーザー要件 (User requirements)**

データセットワークシートのコントロールを利用するには、以下が必要です。
* `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
* あなたはデータセットの所有者であるか、`Can edit` のデータセット権限を付与されている必要があります。

**コントロールパネルの開閉とサイズ変更 (Opening, closing, and resizing the control panel)**

Sigmaのワークシートコントロールは、ワークシートのテーブルおよびチャートエリアの真左に配置された、ワークシートコントロールパネル内にあります。この配置により、コントロールの値を作成・修正しながら、同時にデータがリアルタイムで応答するのを見ることができます。

コントロールパネルを開くには、ワークシートの左側にある `CONTROLS` バー、またはツールバーの `Show Controls` ボタンをクリックします。

コントロールパネルは、その右側にある青いホバーバーをドラッグすることで、サイズ変更したり閉じたりすることができます。

**合計 (Totals)**

合計は、ワークシートの最上位レベルに存在する単一値の列集計です。計算されたワークシートの合計は、コントロールパネルの `TOTALS` セクションで表示および選択できます。`TOTALS` セクションは、ワークシートに一つ以上の合計が存在する場合にのみ表示されます。「[Dataset totals](https://help.sigmacomputing.com/docs/dataset-totals)」を参照してください。

**フィルター (Filters)**

フィルターを使用すると、特定の条件を満たす行のみを表示するようにデータを制限できます。ワークシートのフィルターは、コントロールパネルの `FILTERS` セクションで作成および管理できます。「[Dataset filters](https://help.sigmacomputing.com/docs/dataset-filters)」を参照してください。

**パラメータ (Parameters)**

パラメータは、ワークシートに追加し、数式で参照できるカスタマイズ可能なフィールドです。パラメータは、What-If分析やユーザー入力分析にとって非常に大きな資産となり得ます。ワークシートのパラメータは、コントロールパネルの `PARAMETERS` セクションで作成および管理できます。「[Dataset parameters](https://help.sigmacomputing.com/docs/dataset-parameters)」を参照してください。
#### 3-14. データセットワークシートの列 (Dataset Worksheet Columns)

列はSigmaで作業する上で中心的な役割を果たします。データセットワークシートを作成する際、既存の列を構造化・フォーマットしたり、列の計算を作成したり、データをソート・フィルタリングしたりすることができます。

**データセットワークシートで列を表示する (View columns in dataset worksheets)**

データセットのワークシートで作業する際、下のスクリーンショットのように見えます。このビューは、列の操作をすぐに始めるための2つの方法を提供します：ワークシートのスプレッドシートと列ビューパネルです。これら2つのコンポーネントのいずれかから変更が加えられると、あなたの列はもう一方でも自動的に更新されます。

* **スプレッドシートインターフェース (The spreadsheet interface)**
    ワークシートのスプレッドシートインターフェースは中央に配置され、インタラクティブなスプレッドシートのようなインターフェースを提供します。全ての列アクションは、このテーブルから列メニューを使用して開始できます。

* **列ビューパネル (The column view panel)**
    列ビューパネルはワークシートの右側にあります。これはワークシートの列のハイレベルな編集可能ビューを表示します。このパネルを使用して列を検索し、データをレベルにグループ化します。スプレッドシートと同様に、各列には[列メニュー](#column-menus)もあります。

**列の詳細 (Column details)**

Jsonを除く全てのワークシート列タイプで、列の詳細が利用可能です。個々の列の詳細と統計情報を表示するには、列メニューを開き、`Column Details...` を選択します。

モーダルの内容は列のタイプによって異なりますが、全体的な構造は一貫しています。
* **About (概要)**
    このセクションには、列のタイプ、名前、および数式（fx）がリストされます。
* **Values (値)**
    このセクションは、列のデータの視覚的な表現を表示します。トップ値リストには、列の最も一般的な値が含まれます。この情報は、テキスト、数値、日付の列で利用可能です。値の分布ヒストグラムも、数値と日付の列で利用可能です。
* **Summary (サマリー)**
    このセクションには、主要な列の合計がリストされます：値、Null値、行数、個別値。パーセント列は、列の総行数に対するカウントの割合を示します。
    * **Values** - Nullでない値の総数 (参照：`Count`)
    * **Nulls** - Null値の総数 (参照：`CountIf`, `IsNull`)
    * **Row Count** - 値に関わらず、列の総行数
    * **Distinct Values** - ユニークな値の総数 (参照：`CountDistinct`)
* **Statistics (統計)**
    このセクションには、様々な列の統計がリストされます。最小値と最大値は、日付とテキストの列で表示されます。これらと以下にリストされる他の全ての統計は、数値列で利用可能です。
    * **Minimum** - 列の最小値。(参照：`Min`)
    * **25th Percentile** - 列の値の下位25パーセンタイルに入る値。(参照：`PercentileCont`)
    * **Median** - ソートされた列の値の中点。(参照：`Median`)
    * **75th Percentile** - 列の値の下位75パーセンタイルに入る値。(参照：`PercentileCont`)
    * **Maximum** - 列の最大値。(参照：`Max`)
    * **Average** - 全ての列の値の平均。(参照：`Avg`)
    * **Standard Deviation** - 列の計算された標準偏差。(参照：`StdDev`)
    * **Variance** - 列の統計的分散。(参照：`Variance`)

**既存の列を操作する (Work with existing columns)**

* **列メニュー (Column Menus)**
    列メニューを使用すると、ワークシートのデータを直接操作できます。いくつかの一般的な列アクションは、ソート、フォーマット、非表示、削除、フィルタリング、およびデータの集計です。
    列メニューは、ワークシートのスプレッドシートと列ビューパネルの列名の隣にあります。メニューを開くには、列名にカーソルを合わせ、表示されるドロップダウン矢印をクリックします。

* **列のフォーマット (Formatting columns)**
    1.  フォーマットしたい列の列メニューを開きます。
    2.  ドロップダウンで、`Format` にカーソルを合わせます。
    3.  サブメニューからフォーマットを選択します。
        * *注：フォーマットオプションは列の値のタイプに依存します。*

* **列のソート (Sorting columns)**
    個々の列は、列メニューから直接、昇順と降順の両方でソートできます。複数列のソートを定義するには、いずれかの列の列メニューからワークシートのソートモーダルを開きます。

* **列の移動 (Moving columns)**
    個々の列はドラッグ＆ドロップを使用して移動できます。これはスプレッドシートインターフェースと列ビューパネルの両方で可能です。

* **列の名前変更 (Renaming columns)**
    列の名前を変更するには、列名をダブルクリックするか、列メニューから `Rename Column` を選択します。
    * Sigmaで列の名前を変更しても、データベースでの名前は変更されません。

* **列の説明の追加 (Adding column descriptions)**
    * **列メニューから説明を追加または編集するには：**
        1.  列メニューを開きます。
        2.  `Add Description` をクリックします。
        3.  テキスト入力ボックスに説明を入力します。
        4.  `Save` をクリックします。
    * **ワークシートツールバーから説明を追加または編集するには：**
        1.  列を選択します。
        2.  ワークシートツールバーの `description icon` をクリックします。
        3.  テキスト入力ボックスに説明を入力します。
        4.  `Save` をクリックします。

* **列の説明の表示 (Viewing column descriptions)**
    説明付きの列は、列ヘッダーの左上隅にある黄色いマーカーで識別できます。説明を表示するには、列ヘッダーにカーソルを合わせます。

* **列の非表示と再表示 (Hide or unhide columns)**
    列は、列メニューの 'Hide Column' アクションを使用して非表示にできます。非表示の列はスプレッドシートには表示されません。しかし、列ビューパネルからは引き続き表示され、操作可能です。列ビューパネルでは、非表示の列は表示されている隣の列と比較して「グレーアウト」して表示されます。
    非表示の列を再表示するには、その列のメニューから `Unhide Column` アクションを選択します。
    `Hide Other Columns` アクションを使用することもできます。これは選択した列を表示し、ワークシート内の他のすべての列を非表示にします。
    * *非表示の列はスプレッドシートからのみ非表示になります。ビジュアライゼーション、フィルター、計算列など、ワークシートの他の場所では引き続き使用できます。*

* **列の削除 (Delete columns)**
    列は、列メニューの 'Delete Column' アクションを使用して削除できます。
    * *列を削除すると、関連するフィルターが削除され、参照しているビジュアライゼーションに影響を与え、参照している計算列を壊します。*
    * *全てのワークシートの列アクションと同様に、列を削除しても基盤となるデータソースのデータには影響しません。*

* **複数列の選択 (Multi-column selection)**
    スプレッドシートと列ビューパネルの両方から複数の列を選択できます。範囲の列を選択するには、範囲の2番目の端点をクリックするときにshiftキーを押し続けます。複数の列を個別に選択および選択解除するには、各列をクリックするときに⌘キーを押し続けます。
    選択した列に対してアクションを実行するには、選択した列のいずれかの列メニューを開きます。すべての列アクションが複数選択された列に適用できるわけではありません。

**列の作成と計算 (Creating and calculating columns)**

* **新しい列の追加 (Adding a New Column)**
    テーブルの中間に新しい列を挿入するには、新しい列を配置したい場所の直前にある列のメニューから `Add New Column` を選択します。
    テーブルの最後またはグルーピングレベルの最後の列として新しい列を追加するには、列ビューパネルの関連する `Add New Column` ボタンをクリックします。

* **数式バーを使用する (Use the formula bar)**
    数式バーは、ワークシートでのデータ計算の中心です。これはワークシートの上部、スプレッドシートの上、ツールバーの下にあります。
    数式バーの数式は、常にワークシートで選択されている列に属します。列が選択されていないか、複数の列が選択されている場合、数式は表示されません。
    新しい数式を計算するには、まず新しい列を追加します。次に、数式バーに数式を入力します。入力中に、オートコンプリートされた関数名や列名が提案されます。数式を完成させたら、Enterキーを押すか、数式バーの右にある緑色のチェックマークをクリックします。
    Sigmaの関数インデックスをご覧ください。

**レベルのグルーピングを操作する (Working with level groupings)**

* **データをグループ化する (Group your data):**
    画面の右側で、グループ化したい列の名前を見つけます。その列を `Select Grouping Key` と書かれたボックスまでドラッグします。
    ワークシートの上部または側部にある列名の右側の矢印をクリックしてアクセスする列メニューを使用して、集計列を簡単に作成できます。集計列を作成すると、それは自動的に次のレベルのグループの下にネストされます。
    * *Holidayでグループ化し、売上データを合計する集計列を作成すると、新しい列はHolidayごとの総売上を表示します。*
    画面右側の列名リストからグループ化したい列の名前を探し、その列名を `Base Columns` リストの上にドラッグすると、新しいレベルを追加するオプションが表示されます。ワークシートには2つのレベルのデータグルーピングが表示されます。全てのグループレベルの下にデータの集計列を作成できます。

* **レベルを折りたたむ (Collapsing levels)**
    レベルを折りたたむと、必要なデータのみを表示するのに役立ちます。`Base Columns` ラベルの左にある二重矢印をクリックすることで、レベルを折りたたんだり展開したりできます。

**半構造化データを抽出する (Extract semi-structured data)**

SigmaがJSONまたはVariant列タイプを検出すると、列メニューのオプションに「Extract Columns」が表示されます。データが半構造化されており、「Extract Columns」オプションが表示されない場合は、型関数 `JSON` または `Variant` を使用して、Sigmaがデータの列をどのように解釈するかを変更できます。

#### 3-15. データセットの合計 (Dataset Totals)

合計（Totals）は、ワークシートの最上位レベルに存在する、単一値の列集計です。合計は、ワークシートの右側パネルにある列ビュータブの下で作成できます。計算された合計値は、その後ワークシートの[コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls)に表示されます。

**合計を作成する (Create a Total)**

1.  ワークシートの右側パネルにある**列ビュータブ**を開きます。
2.  `TOTALS` セクションの下にある `New Total...` をクリックします。
3.  リストから列を選択して、推奨される集計合計を自動的に作成します。または、`Add Empty Column` を選択して、独自の数式を記述します。
    * この例では、`[Sales Amount]` 列を選択します。これにより、`Sum([Sales Amount])` という数式を計算する新しい列 `[Sales Amount - Sum]` が自動的に作成されます。
4.  その列は右側の `TOTALS` リストに表示され、その数式は数式バーでアクセス可能になり、計算された値はコントロールパネルの `TOTALS` リストの下に表示されます。


#### 3-16. データセットのフィルター (Dataset filters)

フィルターを使用すると、特定の条件を満たす行のみを表示するようにデータを制限できます。Sigmaのワークシートフィルターは、データセットワークシートの左側パネルに直接配置されているコントロールパネル内にあります。この配置により、フィルターの値を変更しながら、同時にデータがリアルタイムで応答するのを見ることができます。

**ユーザー要件 (User requirements)**

データセットでフィルターを使用するには、`Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。

**フィルターの構成要素 (Anatomy of a filter)**

* **コントロールパネル (Control panel)**
    フィルターは、データセットワークシートタブの左側にあるワークシートコントロールパネル内にあります。このパネルには、ワークシートの合計（Totals）とパラメータも含まれます。

* **フィルターリスト (Filter list)**
    既存のすべてのフィルターは、コントロールパネルの `FILTERS` ヘッダーの下で利用できます。無効化されたフィルターはグレーアウトされます。

* **フィルター (Filter)**
    すべてのフィルタータイプは、フィルターリストに表示される際に同じ基本構造を持っています。
    以下は「Include」フィルターと「Range」フィルターの構成要素です。

    1.  **列タイプアイコン (Column type icon)**
        フィルターされている列のタイプを示すアイコンです。
    2.  **列名 (Column name)**
        フィルターに使用される列の名前です。ワークシートは同じ列に複数のフィルターを持つことができます。
    3.  **フィルタータイプ (Filter type)**
        このラベルは[フィルタータイプ](https://help.sigmacomputing.com/docs/dataset-filters#filter-types)を指定します。
    4.  **フィルター値入力 (Filter value input)**
        この入力コンポーネントは、フィルタータイプによって表示が異なります。フィルターしたい値を入力するために使用します。ワークシートデータは、フィルター値の選択をリアルタイムで反映して更新されます。
    5.  **フィルターの無効化/有効化トグル (Disable/Enable filter toggle)**
        ホバー時にのみ表示されます。トグルをクリックしてフィルターを無効化または再有効化します。フィルターが無効の場合、グレーになります。
    6.  **フィルターメニュー (Filter menu)**
        ホバー時にのみ表示されます。このメニューを開くと、編集や削除などの追加アクションが表示されます。
    7.  **Null値を含めるチェックボックス (Include Nulls Checkbox)**
        フィルターされた列にnull値を含めるかどうかを選択できます。「Include/Exclude」フィルターには「Include Nulls」チェックボックスは適用されません。代わりに、nullはフィルター値入力リストの値としてリストされます。Text Matchフィルターには適用されません。

**フィルターモーダル (The Filter Modal)**

フィルターモーダルを使用すると、SigmaのCreatorはフィルターを作成および編集できます。モーダルのフィールドオプションは、選択した列タイプとフィルタータイプによって異なります。
コントロールパネルのフィルターで直接値を選択する場合とは異なり、フィルターモーダルでの値の選択は、`Save` をクリックした後にのみワークシートデータに適用されます。

**フィルタータイプ (Filter Types)**

フィルターのフィルタータイプは、フィルターに設定できる値と、それらを選択できる形式を決定します。例えば、「include」フィルターは選択できるデータ値のリストを提供し、「range」フィルターは最小値および/または最大値を要求します。

Sigmaワークシートは7つのフィルタータイプをサポートしています。各フィルターで選択できるフィルタータイプは、フィルターが対象とする[列のタイプ](https://help.sigmacomputing.com/docs/dataset-worksheet-columns#column-value-types)に依存します。Json列はフィルターできない唯一の列タイプです。jsonデータをフィルターするには、まず[jsonオブジェクトからデータを抽出する](https://help.sigmacomputing.com/docs/dataset-worksheet-columns#extract-semi-structured-data)必要があります。

* **Include (含める)**
    * デフォルトのフィルタータイプ
    * 選択された値がデータに含まれます。他のすべての値は除外されます。
    * **値入力タイプ:** 選択可能な値のリスト
    * **サポートされる列タイプ:** テキスト, 数値, 日時
* **Exclude (除外する)**
    * 選択された値がデータから除外されます。
    * **値入力タイプ:** 選択可能な値のリスト
    * **サポートされる列タイプ:** テキスト, 数値, 日時
* **Range (範囲)**
    * 指定された範囲内の値のみがデータに含まれます。
    * 範囲は最小値/最大値を含みます。
    * **値入力タイプ:** 最小/最大 数値入力ボックス
    * **サポートされる列タイプ:** 数値
* **Date Range (日付範囲)**
    * このフィルタータイプは、固定および相対的な日付タイプの両方をサポートします。指定された範囲内の値のみがデータに含まれます。
    * 範囲は最小値/最大値を含みます。
    * **値入力タイプ:** 最小値と最大値の両方に固定および/または相対的な日付を選択するオプション付きの単一入力ボックス。
    * **サポートされる列タイプ:** 日付（固定）, 日付（相対）
* **Limit (制限)**
    * 仕様に基づいて列のデータをランク付けし、制限します。
    * **値入力タイプ:** ランク順序/方向のリスト（例：「First N」）、含める値の数の数値入力、ランクタイプ（例：`Rank`, `RankDense`, `RowNumber`）
    * **サポートされる列タイプ:** テキスト, 数値, 日付
* **Text Match (テキスト一致)**
    * フィルターは、入力テキストとデータの値との間の完全および部分一致を検索します。
    * **値入力タイプ:** 一致させる数式のリスト（例：`Contains`, `Starts with`, `Ends with`, `Like`）およびそれらの値を除外する対応物（例：Does not contain, Does not start with, Does not end with, Not like）、検索するテキストのテキスト入力ボックス、大文字と小文字を区別するかのチェックボックス。
    * **サポートされる列タイプ:** テキスト
* **Boolean (ブール値)**
    * TrueまたはFalse
    * true, false, nullでフィルターします。
    * **値入力タイプ:** 値のリスト
    * **サポートされる列タイプ:** 論理値: True, False

**フィルターを作成する (Create a filter)**

* **コントロールパネルからフィルターを作成する**
    1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)がまだ開いていない場合は、折りたたまれたCONTROLSバーまたはワークシートツールバーの `Show Controls` ボタンをクリックして開きます。
    2.  パネルの `FILTERS` セクションの右側にある `+` アイコンをクリックします。
    3.  `Add Filter` モーダルが画面に表示され、ワークシートからフィルターする列を選択するように求められます。
    4.  ドロップダウンリストから `Column` を選択します。
        * *注：選択する列のタイプによって、続くステップが決まります。これは、フィルタータイプとフィルター値が列タイプに依存するためです。この例では、Text (abc) 列を選択します。*
    5.  次に、ドロップダウンメニューから `Filter Type` を選択します。
        * *この例では、デフォルトの ‘Include Values’ フィルタータイプを使用します。*
    6.  `Filter value` の下で、フィルターする値を選択します。
        * *IncludeとExcludeの両方のフィルタータイプは、カウントでランク付けされた値のリストを提供します。順序付けられたリストをスクロールするか、検索を使用して値を見つけて選択します。*
    7.  `Save` をクリックして新しいフィルターを保存します。
        * *新しいフィルターはワークシートコントロールパネルに表示され、ワークシートのスプレッドシートインターフェースと並行して選択した値を変更できます。*

* **列メニューからフィルターを作成する**
    1.  フィルターしたい列の[列メニュー](https://help.sigmacomputing.com/docs/dataset-worksheet-columns#column-menus)を開きます。
    2.  メニューから `Add Filter...` を選択します。
    3.  `Add Filter` モーダルが画面に表示され、列が選択され、デフォルトの `Filter Type` が設定されています。
        * *注：選択した列のタイプによって、続くステップが決まります。この例では、Numeric (123) 列を選択しました。*
    4.  [任意] `filter type` を変更します。
        * *この例では、デフォルトの ‘Range’ フィルタータイプを使用します。*
    5.  `Filter value` の下で、フィルターしたい範囲を選択します。最小値と最大値の両方を指定するか、範囲の一端を開いたままにすることができます。
    6.  値を選択した後、フィルターにnull値を含めるかどうかを選択できます。デフォルトではnullが含まれます。
    7.  `Save` をクリックして新しいフィルターを保存します。
        * *新しいフィルターはワークシートコントロールパネルに表示され、そこで選択した値を変更できます。*

* **セルメニューからフィルターする**
    テーブルセルのコンテキストメニューを使用して、新しいinclude/excludeタイプのフィルターを作成したり、既存のものを変更したりすることが可能です。選択したセルの値でフィルターするには：
    1.  フィルターしたいセルを右クリックします。`cell menu` が開きます。
    2.  メニューから `Include` または `Exclude` を選択します。
        * *あなたの選択はワークシートに適用され、コントロールパネルの `Filters` リストに反映されます。*

**フィルターの値の選択を変更する (Modify a filter’s value selection)**
コントロールパネルからフィルターの値の選択に加えられた変更は、自動的にワークシートのデータに適用されます。値選択の入力フィールドは、フィルタータイプに依存します。

**フィルターを編集する (Edit a filter)**
以下の手順は、「Edit Filter」モーダルを開く方法を示します。ここから、フィルターの構造的な詳細を編集できます。
変更は `Save` を押すまで行われません。
* **コントロールパネルからフィルターを編集する**
    1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
    2.  FILTERSリストで、編集したいコントロールにカーソルを合わせ、キャレットアイコンをクリックしてドロップダウンメニューを開きます。
    3.  `Edit Filter` をクリックします。
        * *「Edit Filter」モーダルが開きます。目的の変更を加えて `Save` をクリックします。*

**フィルターを削除する (Delete a filter)**
以下の手順は、フィルターを永久に削除します。代わりに、[フィルターを一時的に無効にする](https://help.sigmacomputing.com/docs/dataset-filters#temporarily-disabling-a-filter)こともできます。
1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
2.  FILTERSリストで、削除したいフィルターにカーソルを合わせ、キャレットアイコンをクリックしてドロップダウンメニューを開きます。
3.  `Delete Filter` をクリックします。

**フィルターを一時的に無効にする (Temporarily disabling a filter)**
1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
2.  `FILTERS` リストで、無効にしたいコントロールにカーソルを合わせます。
3.  青いトグルスイッチをクリックしてフィルターを無効にします。

**フィルターの権限 (Filter permissions)**
SigmaのCreatorまたはAdminであれば、アクセス権のあるデータセットワークシートでフィルターを表示、作成、編集、削除できます。ただし、他のワークシートの変更と同様に、作業を公開するにはワークシートに対する編集権限が必要です。閲覧専用のアクセス権しかない場合は、ワークシートの変更を新しいワークシートとして保存できます。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。

#### 3-17. データセットのパラメータの作成と管理 (Create and manage dataset parameters)

データセットパラメータは、データセットワークシートに追加し、数式やカスタムSQLで参照できるカスタマイズ可能なフィールドです。データセットパラメータを作成して参照することで、計算で使用される値を動的に置き換えることができます。

what-if分析やユーザー入力分析には、定数値の代わりにパラメータを使用します。パラメータを使用すると、ユーザーはその値を非常に迅速に変更できます。例えば、製品の売上成長率を2%、5%、10%という可変のパーセンテージで比較したい場合、パラメータを使えばこの可変値を数式に素早く注入できます。

データセットパラメータは、コストのかかるワークブックのクエリのパフォーマンスを向上させることもできます。データセットパラメータを使用して、データを必要なものだけに絞り込みます。

データセットの代わりにデータモデルでパラメータを使用したい場合は、「[Pass a value from a workbook control to a data model control](https://help.sigmacomputing.com/docs/parameters-in-data-models)」を参照してください。

**ユーザー要件 (User requirements)**

* データセットでパラメータを**作成、編集、削除、使用**する機能には、以下が必要です。
    * `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
    * あなたはデータセットの所有者であるか、`Can edit` のデータセット権限を付与されている必要があります。
* データセットでパラメータを**表示**する機能には、以下が必要です。
    * `View datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
    * あなたはデータセットの所有者であるか、`Can view` のデータセット権限を付여されている必要があります。

**データセットワークシートでデータセットパラメータを表示する (View dataset parameters in a dataset worksheet)**

1.  Sigmaホームから、既存のデータセットを選択するか、新しいものを作成します。「[Create Datasets](https://help.sigmacomputing.com/docs/create-and-manage-datasets)」を参照してください。
2.  データセットを表示する際、データセットの `Worksheet` タブを表示しているときに、左パネルでデータセットパラメータにアクセスします。

左パネルでは、既存のすべてのデータセットパラメータが `Parameters` の下に表示されます。各パラメータについて、以下を確認できます。
* **Data type:** パラメータの値のタイプを表します。テキスト(abc)、数値(123)、日付(カレンダー)など。詳細は「[Supported data types and formats](https://help.sigmacomputing.com/docs/data-types)」を参照してください。
* **Parameter name:** パラメータの名前。
* **Parameter value:** パラメータの現在の値。データセットを編集する際、新しいパラメータ値を入力できます。パラメータの設定に応じて、リストから値を選択したり、テキストを入力したり、数値を入力したり、日付を選択したりできます。
* **Parameter menu:** パラメータを編集、複製、または削除するためのメニュー。メニューを開くには を選択します。このメニューはデータセットを編集中にのみ利用可能です。

**データセットパラメータを作成する (Create a dataset parameter)**

1.  データセットを開き、そのデータセットの `Worksheet` タブを開きます。
2.  `Edit` をクリックします。
3.  左のコントロールパネルがまだ開いていない場合は、ツールバーの `Show Controls` をクリックするか、`Controls` バーを選択して展開します。
4.  `Parameters` セクションで、`Add Parameter` をクリックします。
5.  `Add Parameter` モーダルが開きます。
6.  `Parameter Name` に、パラメータの名前を入力します。
7.  (任意) 説明を追加します。
8.  パラメータの `Data Type` (Text, Number, Date) を選択します。
9.  `Suggested Values` オプションが、パラメータの入力タイプを決定します。以下のいずれかを選択します。
    * **All:** データ型に応じて、テキスト、数値、または日付の値にすることができます。
    * **List:** カスタムの値オプションのセット。ユーザーはリスト内の任意の値を選択できます。「[Use a list of values in a dataset parameter](#use-a-list-of-values-in-a-dataset-parameter)」を参照してください。
10. (任意) パラメータの `Default Value` を指定します。
11. (任意) 日付または数値のデータ型の場合、パラメータ値の `Format` を指定します。
12. `Save` をクリックします。

パラメータを作成した後、以下のいずれかの方法で使用できます。
* データセットワークシートの左の `Controls` パネルで、値を変更する。
* 新しいデータセット列など、数式でパラメータを参照する。「[Reference a dataset parameter in a formula in a dataset worksheet](#reference-a-dataset-parameter-in-a-formula-in-a-dataset-worksheet)」を参照してください。
* ワークブックコントロールの選択に基づいてパラメータの値を更新する。「[Parameters in Workbooks](https://help.sigmacomputing.com/docs/parameters-in-workbooks)」を参照してください。

**データセットパラメータで値のリストを使用する (Use a list of values in a dataset parameter)**

1.  [データセットパラメータを作成する](https://help.sigmacomputing.com/docs/create-and-manage-dataset-parameters#create-a-dataset-parameter)手順に従い、`Suggested Values` で `List` を選択します。
2.  (任意) 日付または数値のデータ型の場合、パラメータ値の `Format` を指定します。例えば、数値を通貨としてフォーマットします。
3.  `Values List` に、各値を追加します。表示フォーマットを定義した場合、`Display Value` はそのフォーマットを反映します。
4.  (任意) `Default Value` ドロップダウンメニューで、リストから値の1つを選択します。
5.  `Save` をクリックします。

**データセットワークシートの数式でデータセットパラメータを参照する (Reference a dataset parameter in a formula in a dataset worksheet)**

ワークシートの列の数式で、データセットパラメータを名前で参照できます。数式はパラメータの値を使用し、パラメータの値が変更されると自動的に更新されます。

例えば、`Revenue` 列を持つデータセットに対して、`Min Sales Amount` パラメータを作成し、売上収益が最小販売額より大きいかどうかを評価する数式を計算することができます。
1.  データセットに新しい列を追加します。
2.  新しい列の数式バーに、角括弧で囲んだデータセットパラメータの名前を入力します。例： `[Min Sales Amount]`
3.  数式を反映するように列の名前を変更します。例： `Min Sales Param`
4.  パラメータリストで、パラメータの値を更新し、列の変更を観察します。
5.  列の数式を変更して、計算でパラメータを使用します。例えば、列の各行の `Revenue` が `Min Sales Amount` パラメータ値より大きいかどうかを、数式 `[Revenue] > [Min Sales Amount]` を使用して評価します。
    * Sigmaは自動的に列のブール値（論理値）を計算します。
6.  パラメータリストで、パラメータの値を変更し、列のtrue/false値の変更を観察します。
    * 新しいパラメータ値を入力すると、計算列は自動的に更新されます。

**データセットパラメータでデータセットワークシートをフィルタリングする (Filter a dataset worksheet with a dataset parameter)**

データセットパラメータに基づいてデータセットワークシートをフィルタリングするには：
1.  パラメータを作成します。「[Create a dataset parameter](https://help.sigmacomputing.com/docs/create-and-manage-dataset-parameters#create-a-dataset-parameter)」を参照してください。
2.  列の数式でパラメータを参照します。「[Reference a dataset parameter in a formula in a dataset worksheet](#reference-a-dataset-parameter-in-a-formula-in-a-dataset-worksheet)」を参照してください。
3.  その列のフィルターを作成します。
    1.  列メニューから、`Add Filter` を選択します。
    2.  `Add Filter` モーダルで、フィルタータイプと、データセットでフィルターするフィルター値を選択します。例えば、True値のみを表示するように選択します。
    3.  `Save` をクリックします。
    * フィルターはサイドパネルの `Filters` セクションに表示されます。パネルからパラメータとフィルターを更新できます。

**SQLでデータセットパラメータを参照する (Reference a dataset parameter in SQL)**

接続されたデータプラットフォームに対して[SQLクエリを記述して](https://help.sigmacomputing.com/docs/write-custom-sql)、データセットを作成したり、ワークブック要素を生成したりできます。SQLクエリでデータセットパラメータを使用するには、パラメータの名前を二重中括弧で囲みます：
`{{<dataset-parameter-name>}}`

SQLステートメントを更新してパラメータを参照した後、パラメータ値の変更はSQLソースに伝播し、データをリフレッシュします。

SQLでデータセットパラメータを参照するには：
1.  パラメータを作成します。
2.  ワークブックで、SQLからデータ要素を作成します。「[Create a data element](https://help.sigmacomputing.com/docs/create-a-data-element)」を参照してください。
3.  SQLを記述する際、パラメータ名を二重中括弧で囲んで参照して追加します。名前のスペースはハイフンに置き換えます：
    `{{<parameter-name>}}`
    * 例：
    ```sql
    select * from EXAMPLES.PLUGS_ELECTRONICS.F_POINT_OF_SALE
      where SALES_AMOUNT > {{min-sales-amount}}
    ```
4.  パラメータ値が単一引用符付きでSQLに渡される場合、パラメータ名の前に特別なキーワード「#raw」を付けることで、これらの引用符を削除できます：
    `{{#raw <parameter name>}}`
    > 🚩
    > `#raw` 構成値を使用すると、行レベルのセキュリティがバイパスされ、セキュリティの脆弱性が生じる可能性があります。
5.  SQLを保存した後、パラメータに値を入力して結果をテストし、データ要素の出力を確認します。

詳細と例については、「[Write custom SQL](https://help.sigmacomputing.com/docs/write-custom-sql)」と「[Create a dataset from SQL](https://help.sigmacomputing.com/docs/create-a-dataset-from-sql)」を参照してください。

**データセットパラメータを削除する (Delete a dataset parameter)**

データセットパラメータを永久に削除するには：
1.  データセットのワークシートタブに移動します。
2.  `Edit` をクリックします。
3.  左のコントロールパネルがまだ開いていない場合は、ツールバーの `Show Controls` をクリックするか、`Controls` バーを選択して展開します。
4.  `Parameters` リストで、削除したいパラメータにカーソルを合わせ、キャレットをクリックしてドロップダウンメニューを開きます。
5.  `Delete` をクリックします。

#### 3-18. データセットでCSVを使用する (Using CSVs in Datasets)

SigmaのデータセットにCSVデータをアップロードすることができます。CSVをアップロードすると、SigmaはそのCSVのコピーを直接あなたのデータウェアハウスに保存します。そのため、この機能は組織管理者によって、あなたの組織と個々のウェアハウス接続の両方で有効にされている必要があります。

**システムとユーザー要件 (System and user requirements)**

データセットにCSVデータをアップロードする機能には、以下が必要です。
* [CSVアップロード機能](https://help.sigmacomputing.com/docs/enable-csv-uploads)があなたの組織で有効になっている必要があります。
* `Upload CSV` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
* あなたはデータセットの所有者であるか、`Can edit` のデータセット権限を付与されている必要があります。

**CSVデータのストレージ (CSV data storage)**

CSVファイルがSigmaにアップロードされると、そのデータは新しいテーブルとして自動的に[あなたのデータウェアハウスに書き戻され](https://help.sigmacomputing.com/docs/set-up-write-access)ます。あなたの組織に書き込みアクセスが有効なウェアハウスが複数ある場合、単一の保存先を選択するオプションが与えられます。

ウェアハウスに保存されたCSVデータは、ファイルアップロード時に作成されたデータセットを通じてのみアクセス可能です。接続のテーブルとしてリストされているのは表示されません。しかし、CSVデータセットは、同じウェアハウスに保存されている[他のデータと結合する](https://help.sigmacomputing.com/docs/join-data)ことができます。

**CSVの削除 (CSV deletion)**

アップロードされたCSVを参照しているデータセットがSigmaから削除されると、ウェアハウスに作成された関連テーブルは24時間以内に自動的に削除されます。

**CSVからデータセットを作成する (Create Dataset from a CSV)**

以下の手順は、CSVファイルをアップロードして新しいデータセットを作成する方法をガイドします。
1.  左側のナビゲーションパネルで `+ Create New` をクリックします。
2.  ドロップダウンメニューで `Dataset` を選択します。
3.  データソース選択ページが開きます。
4.  データソースとして `CSV` を選択し、アップロードページに移動します。
5.  提供されたリストから `Connection` を選択します。選択した接続が、あなたのファイルがアップロードされるウェアハウスです。書き込みアクセスが有効なデータウェアハウスが一つしかない場合、それはデフォルトで選択されます。
6.  `File Upload` セクションで、ページにドラッグ＆ドロップするか、`Browse` をクリックしてCSVファイルをアップロードします。
7.  CSVを追加すると、データのプレビューが表示されます。プレビューから、列を含めるか除外するかを選択したり、解析オプションを調整したり、必要に応じてエラーに対処したりできます。
8.  `Explore` をクリックしてアップロードを完了します。

**既存のCSVを置き換える (Replace an existing CSV)**

既存のデータセットの基になるCSVを置き換えるには、以下を実行します。
1.  置き換えたいCSVを含むデータセットを開きます。
2.  データセットヘッダーから `Worksheet` タブを選択し、`Edit` をクリックします。
3.  右側のパネルで `Data Sources` タブに移動します。
4.  置き換えたいCSVソースの `•••` メニューを開き、`Replace CSV` をクリックします。
5.  コンピュータからファイルを選択するよう促されます。
6.  新しいCSVを選択すると、`Edit Source` ページが開きます。データをプレビューし、ファイルの解析オプションを指定します。
7.  新しいCSVデータソースに満足したら、`Done` をクリックします。

#### 3-19. データセットのリネージ (Dataset Lineage)

ウェアハウステーブルとデータセットの「Lineage」タブでは、あなたのデータセットやウェアハウステーブルがSigma内のどこで使用されているか、そしてあなたのデータセットが依存している全てのソースを確認できます。これにより、特定のデータセットやウェアハウステーブルに変更を加えた場合に何が影響を受けるかを確認できます。

**データソース (Data sources)**

データソースはデータセットに表示されます。これは、あなたのデータセットによってデータのソースとして直接使用されているウェアハウステーブルとデータセットをリストアップしたものです。

**参照 (References)**

参照はテーブルとデータセットの両方に表示されます。これは、現在のテーブルまたはデータセットを下流でソースとして使用している全てのワークブックとデータセットをリストアップしたものです。

リネージを見ることで、以下のような疑問に答えることができます。
* この列はどこから来たのか？
* このデータはどのように計算されたのか？
* このデータセットを変更した場合、どのワークブックが影響を受けるか？

* #### 3-20. データセットの共有 (Share datasets)

Sigmaデータセットを組織内の他の人々と共有することができます。
ドキュメントの所有者または組織の管理者は、Sigmaドキュメントのアクセス権限を[共有、修正、または取り消す](https://help.sigmacomputing.com/docs/share-content#share-a-document)ことができます。

**権限タイプ (Permission types)**

データセットは `Can View` と `Can Edit` の2つの権限タイプをサポートしており、共有されたドキュメントに対して以下の権限が付与されます。詳細は、「[Folder and document permissions](https://help.sigmacomputing.com/docs/folder-and-document-permissions)」を参照してください。

* **閲覧可能 (Can View)**
    * 閲覧、コピーの作成、および[ワークブックからのエクスポートの送信とスケジュール設定](https://help.sigmacomputing.com/docs/send-and-schedule-exports)ができます。
    * データセットをワークブックや他のデータセットのデータソースとして使用できます。

* **編集可能 (Can Edit)**
    * 全ての `Can View` 権限。
    * 編集、公開、共有ができます。
    * 削除、移動、名前の変更を含むコンテンツの管理ができます。

**データセットを共有する (Share a dataset)**

1.  データセットを開きます。
2.  `Permissions` タブを選択します。
3.  ページの右上隅にある `Add Permission` をクリックして、`Share` モーダルを開きます。
4.  入力して、チームおよび/または個々のメンバーを追加します。
5.  各チームおよび/またはメンバーの権限タイプを選択します。
6.  [任意] `Add a Message` の下にメール通知文を入力するか、`Send an email notification` のチェックを外します。
7.  `Save` をクリックして権限を付与します。

**アクセス権を修正または取り消す (Modify or revoke access)**

1.  データセットを開きます。
2.  `Permissions` タブを選択します。
3.  被付与者の隣にある縦の `•••` メニューをクリックします。
4.  [任意] アクセス権を完全に取り消すには、`Revoke Grant` をクリックします。
5.  代わりに権限を修正するには、`Edit Grant` をクリックします。
6.  `Who has Access` タブが開くので、クリックします。
7.  新しいアクセス/権限タイプを選択するには、チームまたはメンバーの右側にある `Access Type` ドロップダウンメニューを使用します。
8.  `Save` をクリックします。

**コンテンツへのアクセスリクエストに応答する (Respond to a request for access to content)**

ユーザーがあなたのコンテンツにアクセスしようとして権限がない場合、彼らは即時アクセスをブロックするエラーページを通じてアクセスをリクエストできます。これにより、`Request to Access` のメール通知がトリガーされます。

アクセスのリクエストに応答するには、以下を実行します。

1.  メール通知内の `Respond to the Request` ボタンをクリックします。
2.  Sigmaが `Share Dataset` モーダルと共に開かれ、現在のアクセスリクエストを表示できます。任意で、権限ドロップダウンメニューをクリックして、ユーザーが持つべきアクセスレベルを選択します。
    * *注：ユーザーには、そのアカウントタイプが許可するよりも高いアクセス権を付与することはできません。*
3.  必要に応じて `Approve` をクリックします。`Approve` が選択されると、リクエストは `Share Dataset` モーダルから削除され、ユーザーは `Who Has Access` タブにリストされます。
4.  または、`Deny` をクリックします。`Deny` が選択されると、リクエストは `Share dataset` モーダルから削除されます。
5.  `Save` をクリックするか、`Share Dataset` モーダルを閉じます。コンテンツへのアクセスリクエストに関するあなたの決定は、どちらの方法でも保存されます。

6.  #### 3-21. データセットの列を構成する (Configure Dataset Columns)

まず、データセットヘッダーの `Edit` ボタンをクリックします。次に、`Columns` タブをクリックします。

**列の可視性を設定する (Set Column Visibility)**

列のデフォルトの可視性を選択します。
* **Included columns (含まれる列):** デフォルトでワークブックに追加されます。
* **Available columns (利用可能な列):** デフォルトではワークブックに追加されません。
* **Restricted columns (制限された列):** ワークブックでは利用できません。

変更を保存するには、`Publish` をクリックします。

**列をフォーマットする (Format Columns)**

1.  フォーマットしたい列を見つけ、列名の隣にある矢印をクリックして列メニューを開きます。
2.  変更を保存するには、`Publish` をクリックします。

**列の説明 (Column Descriptions)**

1.  データセットヘッダーの `Edit` ボタンをクリックします。
2.  `Column` タブをクリックして開きます。
3.  列の説明入力フィールドに新しい説明を入力します。
4.  変更を保存するには、`Publish` をクリックします。

5.  #### 3-22. データセットのリンク (Dataset Links)

リンクは、2つのデータソース間に事前定義された結合経路を作成します。リンクを定義すると、ユーザーはデータセットに基づいて、リンクされたデータソースからワークブックに列を簡単に追加できます。Sigmaは、あなたのデータベースに既に存在するデータリレーションシップを自動的に取り込みます。もしウェアハウスに外部キーが設定されていれば、それらのリレーションシップは自動的に「Links」タブに表示されるはずです。

リンクを介して追加されたデータは、常に左結合（Left Join）で表示されます。リンクは、多対一（Many-to-One）または一対一（One-to-One）のリレーションシップのみをサポートします。ソースオブジェクトの各行は、ターゲットオブジェクトで最大でも一つの結果しか持つべきではありません。そうでない場合、リンクを使用するワークブックに誤った結果（意図しない行の増殖、ファンアウト）がもたらされ、後続の計算やチャートに影響を与える可能性があります。

Sigmaのリンクの強力な点は、テーブル間のリンクを作成する以上のことができる点にあります。Sigma内の任意の2つのデータソース間にリンクを作成できます。メトリクスを定義するデータセットを作成し、それをウェアハウスのテーブルにリンクして、ユーザーが追加の顧客情報を引き出せるようにすることができます。2つのデータセット間、2つのウェアハウステーブル間、またはその他の任意の組み合わせでリンクを作成できます。リンクを使用すると、ユーザーを制限することなく、探索の経路を作成できます。

さらに、Sigmaはデータベーステーブル間のリレーションシップを設定するためにあなたが行った作業を保持します。

複数のリンクされたテーブル上でSigmaを実行する場合、リンクを持つ基盤となるテーブルが、プライマリデータソースで既に関係を定義済みであることを確認する必要があります。リンクを作成した後、すべてのリンクされた列はデータセットの「Worksheet」タブに表示され、必要な計算列を作成できます。「[Use linked columns in workbooks](https://help.sigmacomputing.com/docs/use-linked-columns-in-workbooks)」を参照してください。

**リンクを作成する (Create Links)**

1.  左側のナビゲーションメニューを使用して、リンクを作成したいデータセットまたはテーブルに移動します。
2.  `Links` タブを開きます。
3.  右上の `Edit` ボタンをクリックします。
4.  `Add Link` をクリックして他のソースへのリンクを追加します。
5.  左側のメニューを使用して、接続したいデータソースを選択します。ソースデータがターゲットデータと一対一または多対一の関係にあることを確認してください。
6.  データソースを選択すると、プレビューが表示されます。
7.  ページヘッダーの `Next` をクリックします。
8.  画面の右側で、結合列と結合結果をプレビューします。
9.  ページヘッダーの `Accept` をクリックします。
10. これで、新しいリンクが `Links` タブにリスト表示されます。
11. `Publish` をクリックして、新しいリンクを保存し、公開します。

リンクの使用に関する詳細は、「[Use linked columns in workbooks](https://help.sigmacomputing.com/docs/use-linked-columns-in-workbooks)」を参照してください。

#### 3-23. SQLからデータセットを作成する (Create a dataset from SQL)

データセットを作成する方法の一つは、ウェアハウス内のデータに対してSQLを記述することです。SQLベースのデータセットは、SQLクエリを受け取り、他の人が追加分析の基盤として使用できる再利用可能なデータソースに変換します。データセットはデータベースに[マテリアライズする](https://help.sigmacomputing.com/docs/dataset-materialization-api)こともでき、クエリの高速化に役立ちます。データセットに加えられた変更は、下流の依存関係に伝播します。

データセットの作成に関する詳細は、「[Create and manage datasets](https://help.sigmacomputing.com/docs/create-and-manage-datasets)」を参照してください。

**要件 (Requirements)**

この機能を使用するには、`Write SQL` および `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
カスタムSQLを実行するには、接続全体に対する `Can use` アクセス権が必要です。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。SQLエディタは、組織内の少なくとも一つの接続に対して接続レベルのアクセス権を持っている場合にのみ表示されます。
既存のSigmaデータセットやワークブック要素をSQLで参照するには、接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が構成されている必要があります。

**カスタムSQLを記述してデータセットを作成する (Create a dataset by writing custom SQL)**

独自のSQLクエリをデータに対して記述してデータセットを作成するには：
1.  **Sigmaホーム**を開きます。
2.  ナビゲーションパネルで `+ Create New` をクリックし、`Dataset` を選択します。
3.  `Select a Data Source` ページで、`SQL` オプションを選択します。
4.  サイドパネルで `Select a Connection` をクリックし、クエリを実行したい接続を選択します。
5.  クエリエディタに、カスタムSQLを入力します。Sigmaはガイドするためのオートコンプリート候補を提供します。
6.  `Run` を選択してSQLクエリを実行します。キーボードショートカットも使用できます：WindowsではCTRL-Enter、MacではCMD-Returnです。
7.  結果が期待通りであることを確認した後、`Get Started` を選択してデータセットを作成します。

カスタムSQLの記述に関する詳細は、「[Write custom SQL](https://help.sigmacomputing.com/docs/write-custom-sql)」を参照してください。

**SQLから作成したデータセットを修正する (Modify a dataset created from SQL)**

データセットの作成に使用したSQLを編集するには、以下を実行します。
1.  修正したいデータセットを開きます。
2.  `Edit` をクリックし、`Worksheet` タブを選択します。
3.  サイドパネルで、データソースパネルを開きます。
4.  `Custom SQL` について、`More` > `Edit Source` を選択します。
5.  開いたクエリエディタで、カスタムSQLを修正します。`Run` をクリックして、クエリが期待通りの結果を返すことを検証します。
6.  `Done` をクリックしてクエリを保存します。
7.  `Publish` をクリックしてデータセットを更新します。

**既存のSigmaデータセットを参照する (Reference existing Sigma datasets)**

データプラットフォームに作成された[ウェアハウスビュー](https://help.sigmacomputing.com/docs/dataset-warehouse-views)の完全修飾名を使用して、既存のSigmaデータセットをSQLで参照できます。もしデータセットにロケーションまたはデータセットウェアハウスビューが利用できない場合は、作成してください。

完全修飾名は、データプラットフォーム内のデータセットのロケーションとウェアハウスビューの名前の組み合わせです。
`SELECT * FROM <location>.<dataset_warehouse_view_name>`

データセットの完全修飾名を特定するには、データセットを表示しているときに `More info` を選択します。

`Location` フィールドは、データセットを含むデータプラットフォーム内のデータベースまたはカタログとスキーマを提供し、`Dataset` フィールドは参照できるビュー名を提供します。

> 💡
> 完全修飾名をクリップボードにコピーするには、`More` () をクリックし、`Copy path` を選択します。

SQLステートメントでSigmaデータセットから個々の列を参照するには、列名を二重引用符で囲みます。例：
```sql
SELECT "Customer Id" FROM DATABASE.SCHEMA.DATASET_WAREHOUSE_VIEW_NAME


#### 3-24. データセットのウェアハウスビューの作成と管理 (Create and manage dataset warehouse views)

ウェアハウスビューは、あなたのデータプラットフォーム内の仮想テーブルであり、Sigmaやあなたのデータエコシステム内の他の任意のアプリケーションを使用してクエリを実行することができます。Sigmaでモデリングしたデータに基づいてウェアハウスビューを作成することで、クエリを簡素化し、関連性のある最新のデータセットをデータベースから直接取得できます。

このドキュメントでは、データセットのウェアハウスビューと、それらをどのように活用するかについて説明します。ワークブックやデータモデル用のウェアハウスビューの作成に関する詳細は、「[Create and manage warehouse views](https://help.sigmacomputing.com/docs/warehouse-views)」を参照してください。

**システム要件 (System requirements)**

データセットのウェアハウスビューを利用するには、あなたの組織の接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。

> 📘
> この機能は、すべてのデータプラットフォーム接続でサポートされているわけではありません。あなたの接続がサポートしているかを確認するには、「[Supported data platforms and feature compatibility](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

**データセットのウェアハウスビューについて (About dataset warehouse views)**

サポートされている接続で書き込みアクセスが有効になっている場合、Sigmaはその接続のデータを使用する任意のデータセットに対して、自動的にウェアハウスビューを作成します。データセットをデータベーステーブルとして保存する代わりに、ウェアハウスビューは、データセットによって定義された特定のクエリロジックを表現するSQLステートメントを保存します。

Sigmaがウェアハウスビューを作成すると、データプラットフォームとSigmaの間にライブリンクが確立されます。ビューはデータセットを信頼できる唯一の情報源（source of truth）として参照し、データの最新バージョンを反映するように自動的に更新されます。

**データセットのウェアハウスビュー vs. マテリアライゼーション (Dataset warehouse views vs. materializations)**

どのデータセットに対しても、Sigmaは最大2つのビューを作成できます。
* データセットの生成したSQLにアクセスできる**ウェアハウスビュー**。
* Sigmaが生成した[マテリアライゼーション](https://help.sigmacomputing.com/docs/dataset-materialization-api)にアクセスできる**マテリアライズドビュー**（データセットにマテリアライゼーションが構成され、スケジュールされている場合）。

Sigmaは、データセットの変更が公開されるたびにウェアハウスビューを保存します。したがって、ウェアハウスビューにクエリを実行すると、データソースからライブデータを取得します。しかし、マテリアライズドビューにクエリを実行すると、最後にスケジュールされたマテリアライズドテーブルからデータを取得するため、取得したデータがライブデータと異なる場合があります。

**データセットのウェアハウスビューにクエリを実行する (Query a dataset warehouse view)**

SQLクエリでデータセットのウェアハウスビューを参照するには、ビューのパスを使用します。
1.  Sigmaでデータセットを開きます。
2.  情報アイコンをクリックして、データセットの詳細を表示します。
3.  `Warehouse views` セクションで、`Dataset` フィールドの `More` をクリックし、`Copy path` を選択します。このパスを使用して、SigmaまたはSQLをサポートするあなたのデータエコシステム内の任意のアプリケーションから、データセットのモデリングされたデータにアクセスします。

**制限事項 (Limitations)**

* データセットでパラメータが使用されている場合、ウェアハウスビューはパラメータのデフォルト値のみを反映します。
* SQLデータセットが非修飾SQL（SQLパスが明示的に定義されていない）を使用している場合、ビューはそのデータセットおよびそれを参照するどのデータセットに対してもエラーを表示します。

**不十分なデータベース権限 (Insufficient database grants)**

接続で書き込みアクセスが有効になっているにもかかわらず、ウェアハウスビューの詳細に `Insufficient permissions` という警告が表示される場合は、あなたのデータプラットフォームでの権限が不十分である可能性があります。関連するすべてのアクセス権が付与されていることを確認するには、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」で概説されている指示とコマンドを参照してください。

例えば、Snowflakeでは、デスティネーションデータベースに対する `USAGE` 権限が必要ですが、Sigmaが使用する書き戻しスキーマに対しては、`USAGE`, `CREATE TABLE`, `CREATE VIEW`, `CREATE STAGE` という権限も付与されている必要があります。

#### 3-25. サポートされるデータ型とフォーマット (Supported data types and formats)

Sigmaは、効果的な分析とレポーティングを促進するために、様々なデータ型とフォーマットをサポートしています。データ型は、取得データ¹および直接入力データ²に適用され、Sigmaがあなたのデータをどのように構造化し、解釈し、操作するかを決定します。データフォーマットは、データを明確で意味のある方法で表示することを可能にします。

このドキュメントでは、サポートされているデータ型を定義し、データ型のフォーマットと制約の概要を説明します。

¹ **取得データ**とは、Sigmaが接続されたクラウドデータウェアハウス（CDW）またはデータベース管理システム（DBMS）からソースとするデータを指します。Sigmaはデータを取得し、ネイティブのCDWまたはDBMSのデータ型に対応する型に変換します。ネイティブのデータ型サポートが存在しない場合、Sigmaはデータをテキストに変換します。
² **直接入力データ**とは、CSVを通じてアップロードされたり、入力テーブルに手動で入力されたりするデータを指します。

**Sigmaのデータ型 (Sigma data types)**

Sigmaは以下のデータ型をサポートしています。
* **Text (テキスト):** テキスト情報を表す文字列。
* **Number (数値):** 数値や定量的情報を表す数字。
* **Date (日付):** 特定の期間や時点を表す日付値。
* **Logical (論理値):** 二元的または条件的な状態を表すブール値（trueまたはfalse）。
* **Variant (バリアント):** 他のデータ型の値を一つ以上表す半構造化データ。
* **Geography (地理):** 地理的な位置や特徴を表す空間データ。

ワークブックでは、`Element properties` > `Columns` リストまたは `Column details` モーダルのアイコンを参照することで、列のデータ型を識別できます。

---

**テキスト (Text)**
テキストデータ型は、テキスト情報を表す非構造化の文字列（文字、数字、記号、スペース）をサポートします。
SigmaがサポートしていないCDWまたはDBMSのデータ型によって表されるデータを取得した場合、データはデフォルトでテキストに変換されます。
テキストデータに対する操作のために提供されている関数のリストについては、「[Text functions overview](https://help.sigmacomputing.com/docs/text-functions)」を参照してください。

---

**数値 (Number)**
数値データ型は、数値や定量的情報を表す構造化された数字をサポートします。
接続されたCDWまたはDBMSで整数、固定小数点数、または浮動小数点数として表されるすべてのデータは、Sigmaの数値データ型にマッピングされます。数値の精度はMicrosoft Excelと同様に扱われます。整数はint64にキャストされ、最大19桁の精度を持つことができます。一方、固定小数点数と浮動小数点数はfloat64にキャストされ、15〜17桁の有効数字を持ちます。Sigmaはまた、小数点の前後に最大19桁を持つ[入力テーブル](https://help.sigmacomputing.com/docs/input-tables-overview)を使用した直接入力値もサポートしています。

> 💡
> 最大桁数を超え、数学的な操作を必要としない正確な数値を表示する必要がある場合（例：口座番号、シリアル番号、その他の識別子）、`Text`関数を使用して列の値をテキスト文字列に変換してください。

* **数値フォーマット (Number formats)**
    数値データは以下のフォーマットで表示できます。

| フォーマット | 例 |
| :--- | :--- |
| Plain text | 1234.56 |
| Number | 1,234.56 |
| Percent | 12.34% |
| Scientific | 1.23e4 |
| SI units | 1.2k |
| Currency | $1234.56 |
| Financial | (1,234.56) |
| Whole number | 1,234 |

* **カスタム数値フォーマット (Custom number format)**
    デフォルトの数値フォーマットオプションに加えて、データ用のカスタム数値フォーマットを構成できます。
    特定の数値列にカスタム数値フォーマットを構成するには：
    1.  目的の列を選択し、`Format` ()を選択し、次に `Custom Number` を選択します。
    2.  関連するフィールドを埋めて、カスタムフォーマットを構成します。`Examples` セクションには、構成がどのように見えるかのプレビューが表示されます。
        * **Format string:** フォーマット文字列を定義します。構文情報については、D3ドキュメントの[formatLocale](https://d3-wiki.readthedocs.io/zh_CN/master/Format-Locale/)を参照してください。
          * 例：`.2s` はSI表記と有効数字2桁を表示 `1.2k` / `.0%` は丸められたパーセンテージを表示 `123456%` / `#x` はプレフィックス付き16進数を表示 `0x4d3`
        * **Currency symbol:** 通貨単位。
        * **Decimal symbol:** 数値の整数部分と小数部分の間の区切り文字。
        * **Digit grouping symbol:** 数値グループ間の区切り文字。
        * **Digit grouping size:** グループ化記号間の希望する桁数。例：`3, 2, 4` の桁数グループサイズを持つ数値は `123, 45, 6789` となります。
        * **Prefix:** データの前に付加される標準的な数値。
        * **Suffix:** データの後に付加される標準的な数値。
        * **Display null as:** null値を表示するための定数。
    3.  `Apply` を選択します。

---

**日付 (Date)**
日付データ型は、特定の時点を表す構造化された日付値をサポートします。
Sigmaは、組織のデフォルトタイムゾーンに対して相対的な日時を表示します。データを異なるタイムゾーンで表示するには、`ConvertTimezone`関数を使用してください。
日付データに対する操作のために提供されている関数のリストについては、「[Date functions overview](https://help.sigmacomputing.com/docs/date-functions)」を参照してください。

* **日付フォーマット (Date formats)**
    日付データは以下のフォーマットで表示できます。

| フォーマット | 例 |
| :--- | :--- |
| Date | 01/31/2023 |
| ISO date | 2023-01-31 |
| Long date | January 31, 2023 |
| Month year | Jan 2023 |
| Date time | 01/31/2023 03:04:05 PM |
| ISO date time | 2023-01-31 15:05:05 |
| Time | 03:04 PM |

カスタム日付フォーマットを構成することもできます。詳細は、「[Define custom date formats](https://help.sigmacomputing.com/docs/define-custom-date-formats)」を参照してください。

---

**論理値 (Logical)**
論理データ型は、二元的または条件的な状態を表す構造化されたブール値（trueまたはfalse）をサポートします。

* **論理フォーマット (Logical formats)**

| フォーマット | 例 |
| :--- | :--- |
| Boolean | true<br><br>false |

---

**バリアント (Variant)**
バリアントデータ型は、テキスト、数値、日付を含む他のデータ型の値を一つ以上表す半構造化データをサポートします。
接続されたCDWまたはDBMSのすべての半構造化データ（variant, array, object型を含む）は、Sigmaのバリアントデータ型にマッピングされます。

* **バリアントフォーマット (Variant formats)**

| フォーマット | 例 |
| :--- | :--- |
| JSON | {"name":"Alex Lee","age":30,"email":"alex@example.com"} |
| GeoJSON | {"type":"Feature","geometry":{"type":"Point","coordinates":[-73.98, 40.74]},"properties":{"name":"Empire State Building","category":"Landmark"}} |

---

**地理 (Geography)**
地理データ型は、地理的な位置や特徴を表す構造化された空間データをサポートします。
"intersect"と"within"演算子を使用して、地理データに対して地理空間結合を実行できます。
* **Intersect (交差):** 地理空間オブジェクトが交差または重なり合う両方のデータセットから行を返します。
* **Within (内包):** あるデータセットの地理空間オブジェクトが、別のデータセットの地理空間オブジェクト内に完全に含まれる行を返します。

> 📘
> 地理データ型は、SnowflakeおよびBigQuery接続でのみ利用可能です。Sigmaは他のCDWまたはDBMS接続からWKTデータや他の地理空間フォーマット（GeoJSONを除く）を取得しますが、それはテキストデータ型として表示されます。

地理データに対する操作のために提供されている関数のリストについては、「[Geography functions overview](https://help.sigmacomputing.com/docs/geography-functions)」を参照してください。

* **地理フォーマット (Geography formats)**

| フォーマット | 例 |
| :--- | :--- |
| Well-known text<br>(WKT) | POINT (10 20)<br><br>LINESTRING (30 40, 50 60, 70 80)<br><br>POLYGON ((0 0, 10 0, 10 10, 0 10, 0 0))<br><br>MULTIPOINT (10 20, 30 40, 50 60)<br><br>MULTILINESTRING ((0 0, 10 10, 20 20), (30 30, 40 40, 50 50))<br><br>MULTIPOLYGON (((0 0, 10 0, 10 10, 0 10, 0 0)), ((20 20, 30 20, 30 30, 20 30, 20 20))) |
