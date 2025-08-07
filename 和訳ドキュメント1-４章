# Sigma日本語ドキュメント 

#### 1-1-1. Sigmaについて (About Sigma)

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

#### 1-2-1. シグマの基礎 (Sigma Basics)

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

#### 1-1-2. Sigmaの歩き方 (Get around in Sigma)

**Sigmaのホームページ**

Sigmaにログインすると、ホームページが表示されます。以下の図と説明は、このページの主要な部分を解説するものです。一部の要素は、あなたのユーザー権限によっては表示されない場合があります。
<img width="1910" height="1031" alt="e3309f6130fed7b81ccd77b3130631371e495cd7b2d1cf8f14f7c7bd15f92794-getaroundinsigma" src="https://github.com/user-attachments/assets/784d3479-6be4-438f-a999-1ab7f813309b" />

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

### 1-2-1. Sigmaのサンプル接続 (Sigma's sample connection)

Sigma組織を作成すると、私たちは自動的にあなたを私たちのサンプルのSnowflakeまたはDatabricksウェアハウスに接続します。この接続は`Sigma sample connection`という名前で、あなたと組織のメンバーに、初めてのSigma体験をすぐに始められるよう、様々なアクセス可能なデータを提供することを目的としています。

#### **サンプルのワークブック (Example workbooks)**
すべてのSigmaユーザーは、サインアップ時に一連のサンプルワークブックテンプレートを提供されます。すべてのサンプルは`Sigma sample connection`のデータ上に構築されています。これらのサンプルは、あなたの`Templates`ギャラリーで表示できます。「[ワークブックテンプレートを始める](https://help.sigmacomputing.com/docs/get-started-with-workbook-templates)」を参照してください。

#### **サンプルデータからワークブックを作成する (Create a workbook from sample data)**
Sigmaのサンプル接続からワークブックを作成することで、Sigmaであなた自身のデータを使用するのがどのようなものかを体験できます。「[ワークブックを作成する](https://help.sigmacomputing.com/docs/create-a-workbook)」を参照してください。

#### **サンプル接続を非表示にする (Hide the sample connection)**
組織の管理者は、組織のSigmaサンプル接続を非表示にできます。組織のメンバーは、接続リストにそれが表示されなくなります。しかし、サンプル接続の上に構築されたコンテンツは、引き続き表示され、使用可能です。
1.  管理ポータルにアクセスします。
2.  管理ポータルのサイドパネルで、`Account`を選択します。
3.  `Features`セクションの下で、`Sample connection`の隣にあるトグルをオンにします。

### 1-2-2-1. ワークブックテンプレートを始める (Get started with workbook templates)

ワークブックテンプレートを使用すると、ユーザーはワークブックの構造をテンプレート化して共有し、迅速かつ一貫性のある再利用が可能になります。

Sigmaは、Sigmaが作成した一連のサンプルを含む、あなたが利用できるすべてのテンプレートをTemplatesギャラリーページにリストします。ホームページの左側ナビゲーションパネルからTemplatesページにアクセスします。
<img width="1449" height="869" alt="03849a4-Screen_Shot_2021-10-28_at_2 12 01_PM" src="https://github.com/user-attachments/assets/04750dda-4139-43aa-a357-3255682c3f07" />

### 1-2-1-2. HubSpotキャンペーン分析テンプレート (HubSpot Campaign Analysis template)

HubSpotキャンペーン分析テンプレートは、HubSpotのマーケティングデータを可視化します。これにより、マーケティング専門家は以下の方法で、職務の中核タスクを実行できます。
* HubSpotデータを迅速に構成する
* キャンペーンデータを分析・比較する
* Sigma内で直接マーケティングキャンペーンを構築する
* 新しいキャンペーンをダウンロードし、*.csvファイルとして保存する

テンプレートの概要については、こちらのビデオをご覧ください。

#### **システムとユーザー要件 (System and user requirements)**
HubSpotキャンペーン分析テンプレートを使用するには、以下が必要です。
* 実際のデータを使用したい場合、組織が関連するHubSpotデータを含むデータソースに接続されている必要があります。それ以外の場合は、Sigmaのサンプルデータでテンプレートを利用できます。
* `Can create, edit, and publish workbooks`権限が有効になっているアカウントタイプを割り当てられている必要があります。
* あなたがテンプレートの所有者であるか、`Can use`または`Can edit`のテンプレートアクセス権を付与されている必要があります。

#### **テンプレートから新しいワークブックを作成する (Create a new workbook from the template)**
1.  Sigmaの`Templates`ギャラリーページを開きます。
2.  `HubSpot Campaign Analysis Template`を探してクリックします。テンプレートが探索として開かれ、独自のデータに交換するよう促すダイアログが表示されます。
3.  サンプルデータでワークブックを閲覧するには、`Dismiss`をクリックします。<img width="524" height="215" alt="1cbac86-use-your-data-dialog" src="https://github.com/user-attachments/assets/25f3100f-11e7-41fe-9377-1077a6cdadc1" />

4.  このサンプルデータを独自のデータに置き換えるには、`Swap Now`をクリックします。<img width="797" height="473" alt="be40a40-template-hubspot-swap-data-sources" src="https://github.com/user-attachments/assets/c973ae54-5e9c-439d-85ef-0a212b998b48" />
  `Swap Now`をクリックすると、Sigmaは`Swap Data Sources`ページを開きます。Sigmaは、現在のソースの構造に一致するテーブルを接続から検索します。
  一致するものが見つからない場合は、手動で正しいテーブルを探すことができます。
5.  `REPLACE WITH`セクションの下にあるソースの隣にある編集()ボタンをクリックして、一致したソースを置き換えます。
    * `HUBSPOT_CONTACTS`, `HUBSPOT_EMAIL_CAMPAIGNS`, `HUBSPOT_EMAIL_SENDS` の3つの有効な形式のテーブルが必要です。
6.  モーダルから新しいテーブルを選択します。
7.  交換する正しいテーブルが指定されたら、`Swap`をクリックします。
8. ページが更新され、あなたのデータが表示されます。
9. ワークブックを確認して、正しいデータがあることを確認します。組織で使用、パーソナライズ、公開できるワークブックを作成するには、ヘッダーの`Save As`をクリックし、新しいワークブックを保存します。

#### **このテンプレートについて (About this template)**
このテンプレートは、組織内のEメールマーケティングキャンペーンのワークフローと分析をサポートするように設計されています。
このテンプレートには、`Email Campaign Analysis`, `Campaign Comparison`, `Build a Campaign`, `Config & Docs`のページがあります。

##### **Eメールキャンペーン分析 (Email Campaign Analysis)**
* **フィルター (Filters):**
    * Email Send Timestamp: 日時セレクター
    * Email Campaign Type: `All`, `Batch Email`など
    * Email Campaign Sub Type: `All`, `VIP`, `E-books`など
* **KPIs:**
    * `Campaigns`, `Emails Sent`, `Contacts`, `Unsubscribes`の全体数を報告します。
* **インタラクティブチャート付きKPIs:**
    * `Delivery Rate`, `Open Rate`, `CTR`, `Unsubscribe Rate`の`Overall Percentage`と`Percentage change`を報告します。
* **キャンペーンインサイト (Campaign Insights):**
    * **フィルター:** Time Bin, Line Value
    * **コンボチャート1:** 時間経過に伴う選択された`Line value`の折れ線グラフと、`Total Deliveries`, `Total Opens`の棒グラフ。
    * **コンボチャート2:** `Campaign SubType`別の選択された`Line value`の`Avg %`の棒グラフ。
* **エンゲージメント (Engagements):**
    * **サマリー:** `Pivot Value`として選択されたメトリックのパフォーマンスが最も良い日と最も悪い日のレポート。
    * **ピボットテーブル:** 選択された`Pivot Value`を、`Weekday`列と`Hour`行で集計します。
* **キャンペーンドリルダウン (Campaign Drill down):**
    すべてのキャンペーンをキャンペーンタイプ別にグループ化し、個々のキャンペーンの粒度でより詳細な調査を可能にします。

##### **キャンペーン比較 (Campaign Comparison)**
過去と現在のキャンペーンの堅牢なA/B分析を実施して、将来より良いメールキャンペーンを構築するための成功要因を特定できます。
* **選択 (Selection):** グループAのキャンペーンとグループBのキャンペーンを別々に選択するセクション。
* **平均 (Averages):** `Average Emails Sent`, `Average Delivery Rate`などを含む、各キャンペーンのグルーピングのメトリックのレポート。
* **チャート:** 各キャンペーンのグループごとに棒グラフ。`Group A Campaigns`と`Group B Campaigns`のそれぞれについて`Sends`, `Deliveries`, `Opens`, `Clicks`を並べて比較します。
* **比較メトリック (Comparison metric):** メトリックを選択し、迅速な視覚分析のためにプロットするセクション。
* **比較分析 (Comparative analysis):** 選択されたXとYのメトリックをマジッククアドラントチャートにプロットするセクション。
* **キャンペーン比較データ (Campaign comparison data):** 選択された各キャンペーンのすべてのデータを組み合わせ、`Campaign A`と`Campaign B`としてグループ化されたテーブル。

##### **キャンペーンを構築する (Build a Campaign)**
新しいキャンペーンを迅速に開始するために、`Build`ページは以下のガイダンスとセレクターを提供します。
* **コンタクトをインポート (Import Contacts):** `Campaign Comparison`ページでのキャンペーンのグループ分析に基づいて、受信者のメールアドレスを選択します。
* **構築 (Build):** コンタクトデータテーブルからコンタクトを追加するセクション。
    * **Companies (会社):** コンタクトテーブルの`Companies`のリストから選択します。
    * **Job Titles (役職):** コンタクトテーブルの`Job Titles`のリストから選択します。
* **キュレート＆エクスポート (Curate & Export):** 新しいキャンペーンの参加者リストを絞り込むのに役立つセクション。

##### **設定＆ドキュメント (Config & Docs)**

**構成オプション (Configuration options)**を選択します。前のページ、特に`Campaign Comparison`では、ユニークイベントまたは全イベントのいずれかと、集計結果を使用します。

* **エンゲージメントイベント (Engagement events):** `Unique`（ユニーク）または`Total`（合計）のエンゲージメントイベントのいずれかを選択します。
* **合計または平均メトリクス (Total or average metrics):** `Average`（平均）または`Total`（合計）オプションのいずれかを選択します。

**ベンチマーク (Benchmarks)**を指定します。これらは`Email Campaign Analyses`ページでキャンペーンの成功を測るために使用できます。
考えられる各`Line value`には、独自のベンチマークがあります。

| ベンチマーク | 説明 |
| :--- | :--- |
| **Open Rate Benchmark %** | この測定のベンチマークを、10進数値として設定します。例えば、開封率35%の場合は、0.35と入力します。 |
| **Unsubscribe Rate Benchmark %** | この測定のベンチマークを、10進数値として設定します。例えば、購読解除率0.5%の場合は、0.005と入力します。|
| **CTR Benchmark %** | この測定のベンチマークを、10進数値として設定します。例えば、CTR 1%の場合は、0.01と入力します。|
| **CTOR Benchmark %** | この測定のベンチマークを、10進数値として設定します。例えば、CTOR 5%の場合は、0.05と入力します。|

### 1-2-1-3. Snowflake利用状況テンプレート (Snowflake usage templates)

SigmaのSnowflake利用状況テンプレートは、あなたの会社のSnowflakeの消費量とパフォーマンスを理解するのに役立つ、正確で詳細な、事前構築済み分析を提供します。これらのテンプレートは、記述的分析と処方的分析を組み合わせて、Snowflake利用状況データへの制約のない分析を開始するための基盤を提供します。Sigmaは以下のテンプレートを提供しています。
* コストモニタリング (Cost monitoring)
* パフォーマンスモニタリング (Performance monitoring)
* ユーザーアクティビティ (User activity)
* リーダーコスト (Reader cost)

#### **ユーザー要件 (User requirements)**
あなたの会社のSnowflake利用状況データでSnowflake利用状況テンプレートを表示するには、以下が必要です。
* あなたは組織の`Admin`であるか、`View usage dashboard`権限が有効になっているアカウントタイプを割り当てられている必要があります。
* あなたの接続は、各テンプレートに対応する適切なSnowflake利用状況スキーマへのアクセス権を持っている必要があります（「[Snowflakeでロールに権限を付与する](#grant-privileges-to-a-role-in-snowflake)」を参照）。

接続のSnowflakeアクセスに関係なく、テンプレートを起動することで、サンプルのSnowflake利用状況データでテンプレートを表示できます。

#### **Snowflake利用状況テンプレートの種類 (Types of Snowflake usage templates)**
各テンプレートの説明、データ、および権限は以下の通りです。

* **コストモニタリング (Cost Monitoring)**
    組織内のすべてのアカウントにわたるコンピューティングとストレージのコストをカバーします。あなたのSnowflake組織全体の契約消費量、コンピューティングコスト、ストレージコストを追跡します。
    * `ORGANIZATION_USAGE`スキーマに対する`SELECT`アクセス権。このスキーマは、プライマリSnowflakeアカウントにのみ存在します。

* **パフォーマンスモニタリング (Performance Monitoring)**
    個々のSnowflakeアカウントのクエリを監視します。クエリのパフォーマンス、ウェアハウスのアクティビティ、およびその他のパフォーマンスメトリックを追跡します。
    * `ACCOUNT_USAGE`スキーマに対する`SELECT`アクセス権。

* **ユーザーアクティビティ (User Activity)**
    個々のSnowflakeアカウントのユーザーを監視します。Snowflakeユーザーがウェアハウスとデータベースをどのように使用するかを追跡します。
    * `ACCOUNT_USAGE`スキーマに対する`SELECT`アクセス権。

* **リーダーコスト (Reader Cost)**
    個々のSnowflakeアカウントのリーダーアカウントのコンピューティングコストを監視します。
    * `READER_ACCOUNT_USAGE`スキーマに対する`SELECT`アクセス権。

#### **接続のロールを変更する (Change the role of a connection)**
値はユーザー属性によって設定される場合があります。アクセス権によっては、変更できない場合があります。
1.  Sigmaの管理ポータルを開きます。
2.  左側のパネルから`Connections`ページを選択します。
3.  接続リストからあなたの接続を選択します。
4.  `Connection Details`で、`Edit`をクリックします。
5.  `Edit connection`ページで、`Connection Credentials`セクションまでスクロールします。
6.  `Role`の定義を変更します。
7.  `Save`をクリックします。

#### **Snowflakeでロールに権限を付与する (Grant privileges to a role in Snowflake)**
Snowflake利用状況テンプレートを使用するには、Sigmaの[Snowflakeへの接続](https://help.sigmacomputing.com/docs/connect-to-snowflake)のロールに、適切なスキーマへのアクセス権を付与する必要があります。

すべてのテンプレートが同じスキーマで実行されるわけではないことに注意してください。特定のスキーマのロール、権限、および許可を理解するには、SnowflakeのAccount Usageドキュメントを参照してください。

#### **Snowflake利用状況テンプレートから新しいワークブックを作成する (Create a new workbook from a Snowflake Usage Template)**
あなたの会社のSnowflake利用状況データを表示するには、以下の手順に従ってSnowflake利用状況テンプレートからワークブックを作成します。

1.  ホームページに移動します。
2.  左のナビゲーションペインで、Templatesギャラリーページを選択します。
3.  使用したいSnowflake Usage Templateをクリックします。
4.  このページは最初にサンプルのSnowflake利用状況データを表示します。
5.  このサンプルデータをあなた自身のSnowflake利用状況データに置き換えるには、Swap Nowをクリックします。
    * サンプルデータでワークブックを表示するには、Dismissをクリックします。
6.  Swap Nowをクリックすると、Swap Data Sourcesページが開きます。Sigmaは、現在のソースの構造に一致するテーブルを接続から検索します。
    * Snowflake利用状況テーブルは構造が一貫しているため、完全に互換性のある一致があるはずです。一致が見つからない場合は、手動で正しいテーブルを探すことができます。
7.  Replace Withセクションで、置き換えたい一致したソースを探し、Editをクリックします。
8.  モーダルから新しいテーブルを選択します。
9.  交換する正しいテーブルを見つけたら、Swapをクリックします。ページが更新され、あなたのデータが表示されます。
10. ワークブックを確認して、正しいデータがあることを確認します。
11. テンプレートから編集可能で公開可能なワークブックを作成するには、ヘッダーのSave Asをクリックし、新しいワークブックを保存します。

#### **既知の問題とSnowflakeの概念 (Known issues and Snowflake concepts)**

##### **アップロードが遅いまたはタイムアウトする (Slow upload or timeout)**
Snowflake利用状況ワークブックのアップロードが遅い、またはタイムアウトする場合、パフォーマンスを改善できます。
ロード時間が遅い、またはクエリがタイムアウトするのは、ビジーなウェアハウスの大規模なテーブルで実行されるクエリの複雑さのために、ウェアハウスがリクエストに応答するのに苦労している場合に一般的です。ロード時間が遅い場合、Sigmaはクエリが2分以上実行されているとリクエストをタイムアウトします。
クエリの実行時間を確認し、タイムアウトを表示するには、ワークブックのクエリ表示モーダルにアクセスしてください。
ワークブックのロード時間を改善するには、日付をより小さな日付範囲にフィルタリングします。SnowflakeのOrganizationおよびAccount Usageテーブルは時間でパーティション分割されているため、日付でフィルタリングするとパフォーマンスが向上します。

##### **ソース交換時のエラー (Errors when source swapping)**
テンプレートでテーブルを交換する際に、エラーやNULLデータが発生することがあります。エラーを避けるために、交換するテーブルが以下の条件を満たしていることを確認してください。
* 同じ接続からであること
* 正しいスキーマからであること
* 空でないこと

これらを確認するには、Swap Data Sourcesモーダルを開き、各テーブルの接続を確認します。
Snowflakeは時々、セカンダリSnowflakeアカウントにORGANIZATION_USAGEスキーマを提供しますが、空のままにします。Cost monitoringテンプレートがこの空のスキーマを参照し、エラーが発生することがあります。これは、ソースの指示をプライマリアカウントのORGANIZATION_USAGEスキーマを使用するように変更することで修正できます。

##### **Snowflakeの組織 vs. アカウント (Snowflake organization vs. account)**
組織は主要なSnowflakeオブジェクトです。それは事実上、Snowflakeアカウントのコレクションです。一つまたは多くのアカウントを含むことができ、そのうちの一つだけがプライマリアカウントです。このプライマリアカウントには、SNOWFLAKEデータベース内にORGANIZATION_USAGEスキーマが提供されます。他の（セカンダリ）アカウントは、デフォルトではこのスキーマにアクセスできません。
アカウントは、ウェアハウス、データベース、ユーザー、ロールなどのコレクションです。各アカウントは組織の子であり、独自のACCOUNT_USAGEおよびREADER_ACCOUNT_USAGEスキーマを持っています。これらのスキーマには、このアカウントのみのデータが含まれており、同じ組織内の他のアカウントに関する情報はありません。

##### **現在のデータ (Current data)**
テンプレートのコピーをあなた自身のデータに添付して起動した後、Snowflake利用状況テンプレートは常に最新のデータを表示します。テンプレートは、Snowflakeによって管理されるSnowflake提供のビューに依存しており、現在のデータ（最大数時間の遅延）を提供します。

##### **テンプレートの更新 (Updating templates)**
Sigmaがテンプレートを更新し、SUTのような共有テンプレートに変更を公開すると、そのテンプレートにアクセスできるすべてのSigma組織は、そのテンプレートから起動されるすべての新しいワークブックでそれらの変更を見ることができます。テンプレートの以前のバージョンから作成されたワークブックは、更新を見ることができません。

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
#### 2-1-1-1. Snowflakeへの接続 (Connect to Snowflake)

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

1.Snowflake接続を作成するには、Sigmaで以下のステップを実行します。
2.接続を追加し、接続詳細を指定する
3.  接続資格情報を指定する
4.  認証方法を構成する：
    * キーペア認証でSnowflakeに接続する
    * OAuthでSnowflakeに接続する
    * 基本認証でSnowflakeに接続する
5.  書き込みアクセスを構成する
6.  接続機能を構成する

**接続を追加し、接続詳細を指定する (Add a connection and specify connection details)**

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。`Add new connection` ページが表示されます。
3.  `Connection details` で、以下を指定します。
    * **Name:** 新しい接続の `Name` を入力します。Sigmaはこの名前を接続リストに表示します。
    * **Type:** `Snowflake` タイルを選択します。

#### **接続資格情報を指定する (Specify your connection credentials)**

`Connection Credentials` セクションで、必須項目を入力します。

* [任意] プロキシサーバーを使用してSnowflakeにアクセスする場合は、`Use Custom Host` トグルをオンにし、`Snowflake Custom Host` 名を入力します。
* `Account` フィールドに、Snowflakeのアカウント名を入力します。アカウント名のフォーマット方法の詳細は、Snowflakeドキュメントの「[Using an account name as an identifier](https://docs.snowflake.com/en/user-guide/connecting.html#using-an-account-name-as-an-identifier)」を参照してください。
* `Warehouse` フィールドに、Snowflakeにリストされているウェアハウス名を入力します。
    > 📘
    > ユーザー属性を使用してウェアハウスを設定するには、`Warehouse` フィールドの `Set by user attributes` をクリックします。「[Configure user attributes on a Snowflake connection](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照してください。
* `Warehouse` フィールドをユーザー属性を使用して設定し、この接続で入力テーブルを使用する予定がある場合は、`Service Account Warehouse` フィールドに、動的ウェアハウス切り替えの場合にサービスアカウントが使用できるウェアハウス名を提供してください。「[Dynamic Role Switching with Snowflake QuickStart](https://help.sigmacomputing.com/docs/dynamic-role-switching-quickstart)」の「Warehouse Switching」を参照してください。
* `Authentication` の隣にあるキャレット()をクリックし、認証方法を選択し、選択した方法の必須フィールドを入力します。
    * [キーペア認証でSnowflakeに接続する](#connect-to-snowflake-with-key-pair-authentication)
    * [OAuthでSnowflakeに接続する](#connect-to-snowflake-with-oauth)
    * [基本認証でSnowflakeに接続する](#connect-to-snowflake-with-basic-authentication)

> 🚩
> Snowflakeは、プログラムによるサービスユーザーにはキーペア認証またはOAuthの使用を推奨しており、認証ポリシーでそれを強制することができます。Snowflakeブログの「[Snowflake Strengthens Security with Default Multi-Factor Authentication and Stronger Password Policies](https://www.snowflake.com/blog/snowflake-strengthens-security-default-multi-factor-authentication-stronger-password-policies/)」を参照してください。

---

##### **キーペア認証でSnowflakeに接続する (Connect to Snowflake with key pair authentication)**

公開鍵と秘密鍵のRSAキーペアの組み合わせを使用して接続を認証するには、認証方法として `Key Pair` を選択します。
この方法では、公開鍵と秘密鍵が既に作成されており、公開鍵で構成されたSnowflakeユーザーが必要です。Snowflakeドキュメントの「[Key-pair authentication and key-pair rotation](https://docs.snowflake.com/en/user-guide/key-pair-auth)」を参照してください。多要素認証（MFA）ポリシーが適用されている場合は、このユーザーをMFAポリシーから除外してください。すべての前提条件ステップとキーのローテーション方法の詳細なウォークスルーについては、「[Snowflake Key-pair Auth QuickStart](https://help.sigmacomputing.com/docs/snowflake-key-pair-auth-quickstart)」を参照してください。

1.  `User` フィールドに、公開鍵で構成されたSnowflakeの`login_name`を入力します。Snowflakeでは、`login_name`はユーザー名とは異なります。Snowflakeの`describe user`コマンドを使用して、任意のユーザーの`login_name`を見つけます。`describe user`コマンドのすべての有効な名前は、Snowflakeの`all_user_names`コマンドで見つけます。
2.  `Private Key` フィールドに、ヘッダーを含む秘密鍵のテキストを貼り付けます。<img width="614" height="491" alt="f0e02b9c4a1497cfdb9733877596878be2c3735b9f19fd8740cce5a780be9a5f-connection_credentials_private_key1" src="https://github.com/user-attachments/assets/7380d113-fb27-447e-a75e-150dd06a0e3e" />

3.  [任意] 構成している場合は、`Private Key Passphrase` を入力します。
4.  [任意] この接続で使用するSnowflakeの `Role` を入力します。ロールが提供されない場合は、Snowflakeでのユーザーのデフォルトロールが使用されます。
    > 📘
    > ユーザー属性を使用してロールを設定するには、`Role` フィールドの `Set by user attributes` をクリックします。「[Configure user attributes on a Snowflake connection](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照してください。
5.  `Role` フィールドをユーザー属性を使用して設定し、この接続で入力テーブルを使用する予定がある場合は、動的ロール切り替えの場合にサービスアカウントが使用できる `Service Account Role` を提供してください。設定しない場合、サービスアカウントのロールはSnowflakeでユーザーに設定されたデフォルトロールになります。「[Dynamic Role Switching with Snowflake QuickStart](https://help.sigmacomputing.com/docs/dynamic-role-switching-quickstart)」を参照してください。
    次に、追加オプションについては「[書き込みアクセスを構成する](#configure-write-access)」および「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

##### **OAuthでSnowflakeに接続する (Connect to Snowflake with OAuth)**

`Authentication`ドロップダウンから`OAuth`を選択して、接続の認証方法として構成します。

> 📘
> 接続へのユーザー認証のために一意のOAuthアプリケーションを構成するオプション（つまり、組織レベルで使用するOAuth構成を再利用しないことを選択する）は、パブリックベータ機能であり、制限の対象となります。
> 「[Use different OAuth configurations for authenticating users to your connections than you use for your Sigma organization (Beta)](https://help.sigmacomputing.com/docs/oauth-for-connections-overview)」を参照してください。

1.  [任意] 外部IdPを使用してSigma組織へのユーザー認証にOAuthを使用しており、組織で[複数のIDプロバイダー](https://help.sigmacomputing.com/docs/configure-multiple-idps-for-an-organization)が有効になっていない場合、この接続に組織レベルのOAuth構成を再利用するオプションがあります。既存のOAuth構成を再利用するには、`Use organization-level OAuth configuration`の隣にあるトグルをオンにします。このトグルをオンにした場合は、ステップ3に進みます。
2.  組織レベルのOAuth構成がない場合、組織で[複数のIDプロバイダー](https://help.sigmacomputing.com/docs/configure-multiple-idps-for-an-organization)が有効になっている場合、または組織レベルのOAuth構成を再利用したくない場合は、この接続用に一意のOAuth構成を設定します。
    * `OAuth Features`セクションのフィールドを入力する前に、「[Configure a Sigma OAuth application](https://help.sigmacomputing.com/docs/configure-okta-oauth-for-sigma#configure-a-sigma-oauth-application)」の手順を完了してください。
a.  [任意] OAuthトークンのアクセスをさらに指定するために、追加の`Scopes`を入力します。デフォルトのスコープ`openid`, `profile`, `email`, `session:role-any`は必須です。デフォルトのスコープ`offline_access`は推奨されますが必須ではありません。これらのスコープの詳細については、「Configure a Sigma OAuth application」のステップ3を参照してください。
    > 📘
    > Microsoft Entra IDをIdPとして使用している場合、`session:role-any`スコープの前に、Microsoft Entra IDのExpose an APIページの「Scopes defined by this API」の下にあるアプリケーションID URIを付けます。結果のスコープは次のパターンに従います： `https://<your_azure_domain>/<your_app_UUID>/session:role-any`
b.  `Metadata URI`フィールドに、OAuthメタデータURIを入力します。
c.  `Client ID`フィールドに、OAuthアプリケーションのクライアントIDを入力します。
d.  [任意] OAuthアプリケーションでPKCEを有効にしなかった場合は、`Client Secret`フィールドにOAuthアプリケーションのクライアントシークレットを入力します。
e.  [任意] この接続をさらに認証するためにProof Key for Code Exchangeを使用したい場合は、`Require PKCE`の隣のボックスをチェックします。
f.  [任意] この接続をさらに認証するためにJSON Web Tokensを使用したい場合は、`Use JWT bearer tokens`の隣のボックスをチェックします。
3.  `Service Account`が必要かどうかを判断します。サービスアカウントを構成する理由は3つあります。
    * この接続で書き込みアクセスを有効にする場合。
    * Sigmaのパブリック埋め込み機能を使用する場合。
    * 管理者が個々のワークブックを各個人のOAuth資格情報ではなくサービスアカウントを使用して実行するように構成したい場合。
4. サービスアカウントが必要な場合は、`Service Account`スイッチをオンにし、Snowflakeサービスアカウントの`User`と`Password`を入力します。
    > 📘
    > サービスアカウントは、Sigmaでの管理目的で作成されたSnowflakeユーザーです。他のSnowflakeユーザーと同じです。ユーザーには接続で使用したいロールが付与されている必要があり、そのロールにはウェアハウスに対する`USAGE`権限が付与されている必要があります。MFAポリシーが適用されている場合は、サービスアカウントをこのポリシーから除外してください。
    > サービスアカウントは、接続上の他のすべてのOAuthアカウントと同様に、OAuthユーザーリストに追加する必要があります。
5. [任意] この接続で使用するSnowflakeの`Role`を入力します。ロールが提供されない場合は、Snowflakeでのユーザーのデフォルトロールが使用されます。
次に、追加オプションについては「[書き込みアクセスを構成する](#configure-write-access)」および「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の`Create`をクリックして接続を作成します。

##### **基本認証でSnowflakeに接続する (Connect to Snowflake with basic authentication)**

ユーザー名とパスワードで接続するには、認証方法として `Basic Auth` を選択します。

> 🚩
> Sigma Computingは、Snowflakeへの接続時に基本認証の使用から移行することを推奨しています。セキュリティを向上させるために、代わりにキーペアまたはOAuth認証を使用してください。
> 多要素認証（MFA）ポリシーが適用されている場合は、このユーザーをMFAポリシーから除外してください。

1.  `User` フィールドに、Snowflakeの`login_name`を入力します。Snowflakeでは、`login_name`はユーザー名とは異なります。Snowflakeの`describe user`コマンドを使用して、任意のユーザーの`login_name`を見つけます。`describe user`コマンドのすべての有効な名前は、Snowflakeの`all_user_names`コマンドで見つけます。
2.  `Password` フィールドに、Snowflakeのパスワードを入力します。
3.  [任意] この接続で使用するSnowflakeの `Role` を入力します。ロールが提供されない場合は、Snowflakeでのユーザーのデフォルトロールが使用されます。
    > 📘
    > ユーザー属性を使用してロールを設定するには、`Role` フィールドの `Set by user attributes` をクリックします。「[Configure user attributes on a Snowflake connection](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照してください。
4.  `Role` フィールドをユーザー属性を使用して設定し、この接続で入力テーブルを使用する予定がある場合は、動的ロール切り替えの場合にサービスアカウントが使用できる `Service Account Role` を提供してください。設定しない場合、サービスアカウントのロールはSnowflakeでユーザーに設定されたデフォルトロールになります。「[Dynamic Role Switching with Snowflake QuickStart](https://help.sigmacomputing.com/docs/dynamic-role-switching-quickstart)」を参照してください。
次に、追加オプションについては「[書き込みアクセスを構成する](#configure-write-access)」および「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

---

#### **書き込みアクセスを構成する (Configure write access)**

書き込みアクセスは、以下の機能に必要です。
* CSV upload
* Materialization
* Input tables
* Warehouse views

> 📘
> バイナリの入出力は `hex` 形式に設定する必要があります。Snowflakeドキュメントの「[Binary input and output](https://docs.snowflake.com/en/user-guide/binary-input-output)」を参照してください。

書き込みアクセスを構成する手順は、接続に使用される認証方法によって異なります。あなたの認証オプションに一致する指示に従ってください。
* [基本認証またはキーペア認証を使用する接続で書き込みアクセスを構成する](#configure-write-access-on-a-connection-with-basic-auth-or-key-pair-auth)
* [OAuthを使用する接続で書き込みアクセスを構成する](#configure-write-access-on-a-connection-with-oauth)

##### **基本認証またはキーペア認証を使用する接続で書き込みアクセスを構成する (Configure write access on a connection with Basic Auth or Key Pair Auth)**
書き込みアクセスを構成するには、Snowflakeで専用のデータベースとスキーマを設定し、必要な権限を付与する必要があります。
書き込みアクセスを有効にする前に、Sigma接続の構成に使用するSnowflakeユーザーに、以下の権限を持つロールを付与してください。

| オブジェクト | 権限 |
| :--- | :--- |
| **Database** | USAGE |
| **Schema** | USAGE, CREATE TABLE, CREATE VIEW, CREATE STAGE |

> 📘
> 動的テーブルで増分マテリアライゼーションを実行するには、接続で使用されるプライマリロールに、Snowflakeドキュメントの「[Privileges to create a dynamic table](https://docs.snowflake.com/en/user-guide/dynamic-tables-privileges)」にリストされている権限も付与されている必要があります。

`Enable write access` の隣にあるスイッチをオンにします。次に、以下のフィールドを構成します。
1.  `Write database` フィールドに、Sigmaが書き戻しデータを保存するデータベースの名前を入力します。
2.  `Write schema` フィールドに、Sigmaが書き戻しデータを保存するデータベーススキーマを入力します。
3.  [任意] `Materialization warehouse` フィールドに、マテリアライゼーションを実行するクエリを実行するための別のウェアハウスを入力します。
4.  [任意] デフォルトでは、Sigmaは増分マテリアライゼーションに動的テーブルを使用します。動的テーブルを使用したくない場合は、`Use dynamic tables` スイッチをオフにします。
次に、追加オプションについては「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

##### **OAuthを使用する接続で書き込みアクセスを構成する (Configure write access on a connection with OAuth)**
書き込みアクセスを構成するには、Snowflakeで専用のデータベースとスキーマを設定し、必要な権限を付与する必要があります。すべての前提条件ステップについては、「[Configure OAuth with write access](https://help.sigmacomputing.com/docs/oauth-with-write-access)」を参照してください。
`Enable write access` の隣にあるスイッチをオンにします。次に、以下のフィールドを構成します。
2.  SnowflakeがSigmaからの書き戻しデータを保存する `Destination` を少なくとも1つ提供します。`DATABASE.SCHEMA` の形式を使用します。
3.  [任意] 必要に応じて、追加のデスティネーションを入力します。
4.  [任意] `Input table edit log destination` フィールドに、この接続上の入力テーブルへのすべての編集をログに記録するための追加の `DATABASE.SCHEMA` デスティネーションを提供します。
5.  [任意] `Materialization warehouse` フィールドに、マテリアライゼーションを実行するクエリを実行するための別のウェアハウスを入力します。
6.  [任意] デフォルトでは、Sigmaは増分マテリアライゼーションに動的テーブルを使用します。動的テーブルを使用したくない場合は、`Use dynamic tables` スイッチをオフにします。
次に、追加オプションについては「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

---

#### **接続機能を構成する (Configure connection features)**

`Connection Features` セクションで、以下を指定します。

1.`Connection timeout` フィールドに、タイムアウトまでの時間（秒）を指定します。デフォルトは120秒です。最大は600秒（10分）です。
2. [任意] `Use friendly names` スイッチをオフにすると、Sigmaが自動で列名を読みやすくするのをやめます。
3. [任意] `Export warehouse` フィールドに、エクスポートクエリ用に作成された仮想ウェアハウスの名前を入力します。詳細は、「[Configure an export warehouse](https://help.sigmacomputing.com/docs/configure-an-export-warehouse)」を参照してください。

#### **接続作成を完了する (Finish creating your connection)**

接続の全てのパラメータを指定した後、`Create` をクリックします。
1.画面右上の`Create`をクリックして接続を作成します。Sigmaは画面に接続の概要を表示します。

2.`Browse Connection` をクリックし、`Add permission` をクリックして、組織内のユーザーにデータアクセスを許可します。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。

3.左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。
<img width="1270" height="463" alt="df1cae029a961e4beaffb79b6dca5804b6c2e02d17f610bd9d2d34a4bc750625-browse-snowflake-connection" src="https://github.com/user-attachments/assets/8d0b5fc1-1861-4093-8d56-0c5f7d844222" />

* #### 2-1-1-2. Snowflake接続でユーザー属性を構成する (Configure user attributes on a Snowflake connection)

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

6.`Create` をクリックすると、属性は `User Attributes` の下に表示されます。
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
 サービスアカウントを使用する既存の接続でユーザー属性を構成している場合は、ステップ5に進みます。
3.  `Snowflake`をクリックします。<img width="1094" height="222" alt="977f0d3-1" src="https://github.com/user-attachments/assets/4380208b-a8e6-4f8a-826b-cd04dec7d97c" />
4.  `Connect to Snowflake`ドキュメントの一般的な構成手順に従います。<img width="698" height="549" alt="ba388cb-2" src="https://github.com/user-attachments/assets/800f9f73-3848-43a1-a213-e62b1905aa2f" />
5.  `Warehouse`フィールドの`More Menu`をクリックして、以前に構成したウェアハウス属性を参照して選択します。<img width="560" height="150" alt="46d72ce-3" src="https://github.com/user-attachments/assets/96cae90c-d072-4471-a0fe-ee837badeea5" />

6.  `Role`フィールドの`More Menu`をクリックして、以前に構成したロール属性を参照して選択します。OAuthアクセスは選択解除する必要があります。<img width="497" height="163" alt="ac05166-4" src="https://github.com/user-attachments/assets/0f84abdc-4569-4100-bc66-64d73acab9de" />


7.これで、あなたのSnowflake接続は、Snowflakeで設定されたロールとウェアハウスを動的に使用するように構成されました。

#### **セキュアな埋め込みでの使用 (Use with secure embeds)**
接続で属性を構成した後、セキュアな埋め込みURLで外部ユーザーに属性を渡すことができます。埋め込みでロールとウェアハウスの属性を使用するには、パラメータをURL（埋め込みパスURL）に追加する必要があります。
> 📘
> `Role`属性の場合、この構成はセキュアな埋め込みの期間中、行レベルのセキュリティを強制します。

##### **セキュアな埋め込みURLにパラメータを追加する (Add parameters to a secure embed URL)**
セキュアな埋め込みで属性を渡すためには、両方の属性のパラメータを埋め込みURLに追加する必要があります。
埋め込みURLでは、属性は次のようにフォーマットされるべきです。

**:ua_{nameofattribute}=value
//example
:ua_warehouse=wh:**

以下の例では、属性はセキュアな埋め込みURLの末尾に追加されています。

**https://app.sigmacomputing.com/embed/1qmpD5yiMIRvb6dI8l4pzK
?:nonce=35df8548-c7e5-4d35-92da7f8114843999
&:session_length=3600
&:client_id=9319bfb04ae48af48bbee8f702669c085a38b6a73f43d32htd70a3cd6ee4h9iu
&:time=1654709460
&:external_user_id=12
&:external_user_team=Team%20A%2CTeam%20B
&:email=[harold@mycoolcompany.com](mailto:harold@mycoolcompany.com)
&:account_type=explorer
&:mode=userbacked
&:ua_warehouse=wh1
&:signature=j323557c82b26103faf65314db41ebc51ea9n3a61795ef22f45ep0aed1f4182493**

セキュアな埋め込みURLへのパラメータ追加に関する詳細は、「[Embed URL parameters](https://help.sigmacomputing.com/docs/embed-url-parameters)」および「[Example embed API and URL](https://help.sigmacomputing.com/docs/example-embed-api-and-url)」を参照してください。

#### 2-1-1-3. エクスポートウェアハウスを構成する (Configure an export warehouse)

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
3.  **接続概要の「Connection Details」セクションに移動し、「Edit」をクリックします。**<img width="1149" height="329" alt="connection-details_edit" src="https://github.com/user-attachments/assets/03bea798-f025-4ee6-a152-a3d902467237" />

4.  **「Connection Features」セクションで、「Export Warehouse」フィールドを探し、エクスポートクエリ用に作成した仮想ウェアハウスの名前を入力します。**<img width="827" height="362" alt="connection-features_add-export-warehouse" src="https://github.com/user-attachments/assets/865d13b0-8a46-49cb-8728-c13e2c4d4fee" />

5.  **「Save」をクリックして、指定されたウェアハウス経由ですべてのスケジュールされた、直接の、オンデマンドのエクスポートを実行するようにします。**

> 📘
> エクスポートウェアハウスは、プライマリウェアハウスの接続キューサイズを継承します。エクスポートウェアハウスに異なるキューサイズを設定するには、サポートにお問い合わせください。
>
> #### 2-1-4. Snowflake接続またはユーザーの入力テーブルアクセスを復元する (Restore input table access for a Snowflake connection or user)

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

* #### 2-1-2-1. Databricksへの接続 (Connect to Databricks)
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

#### **Databricksを構成する (Configure Databricks)**

SigmaにDatabricks接続を追加する前に、Databricksで以下のステップを完了してください。

1.  まだ存在しない場合は、Databricks SQLウェアハウスを作成します。Databricksドキュメントの「[Create a SQL warehouse](https://docs.databricks.com/en/sql/admin/sql-warehouses.html#create-a-sql-warehouse)」を参照してください。
2.  このSQLウェアハウスへの接続に使用するユーザーまたはサービスプリンシパルが、そのコンピュートリソースに対する`Can use`または`Can manage`の権限を持ち、全てのワークスペースユーザーが`Can use`の権限を持っていることを確認してください。
3.  `Auto stop`設定を構成します。この設定に関する情報は、Databricksドキュメントの「[Configure SQL warehouse settings](https://docs.databricks.com/en/sql/admin/sql-warehouses.html#configure-sql-warehouse-settings)」を参照してください。
    * サーバーレスSQLウェアハウスを実行している場合、Sigmaは`Auto stop`を有効にし、10分または15分に設定することを推奨します。
    * ProまたはクラシックSQLウェアハウスを実行している場合、SQLエンドポイントが中断状態のときに最初のクエリがタイムアウトしたり遅くなったりしないように、Databricksエンドポイントの`Auto stop`を無効にしてください。
4.  SQLウェアハウスへのデータアクセスを構成します。Databricks SQLウェアハウスを使用してデータをクエリするためには、DatabricksをSigmaに接続するために使用するユーザー、グループ、またはサービスプリンシパルが、データへの基盤となるアクセス権を持っている必要があります。Unity Catalogでこれらの権限を設定する手順については、Databricksドキュメントの「[Manage privileges in Unity Catalog](https://docs.databricks.com/en/data-governance/unity-catalog/manage-privileges/index.html)」を参照してください。
    * カタログレベルで、全てのアカウントユーザーに`USE CATALOG`と`USE SCHEMA`権限を付与します。
    * スキーマレベルで、全てのアカウントユーザーに`BROWSE`, `EXECUTE`, `READ VOLUME`, `SELECT`権限を付与します。
    * この接続で書き込みアクセス機能を有効にする予定がある場合は、書き込みアクセス用に定義した専用のデータベースとスキーマのスキーマレベルで、全てのアカウントユーザーに`MODIFY`と`CREATE TABLE`権限も付与します。
    * これらの権限の詳細については、Databricksドキュメントの「[Unity Catalog privileges and securable objects](https://docs.databricks.com/en/data-governance/unity-catalog/securable-objects-privileges.html)」を参照してください。
    > 📘
    > 従来のHiveメタストアを使用して権限を管理している場合、権限モデルは異なります。従来のHiveメタストアで同等の権限を設定するには、Databricksドキュメントの「[Hive metastore privileges and securable objects (legacy)](https://docs.databricks.com/en/data-governance/hive-metastore/privileges.html)」を参照してください。`hive_metastore`カタログからデータを同期したい場合、そのカタログ内のテーブルには`READ_METADATA`権限が必要です。
5.  SQLウェアハウスの`Connection details`画面から`Server hostname`と`HTTP path`を取得します。これらの値は、次のステップでSigmaのDatabricks接続を構成する際に必要になります。
6.  このSQLウェアハウスへの接続に使用するユーザーまたはサービスプリンシパルのためのアクセストークンを作成します。作成するトークンの種類は、SigmaでDatabricks接続を構成する際に使用する認証方法によって異なります。トークン作成の手順については、Databricksドキュメントの「[Authentication for Databricks tools and APIs](https://docs.databricks.com/en/dev-tools/auth/index.html)」を参照してください。

#### **SigmaでDatabricks接続を作成する (Create a Databricks connection in Sigma)**

SigmaでDatabricks接続を作成するには、以下のステップを実行します。
1.  接続を追加し、接続詳細を指定する
2.  接続資格情報を指定する
3.  書き込みアクセスを構成する
4.  接続機能を構成する

##### **1. 接続を追加し、接続詳細を指定する (Add a connection and specify connection details)**
1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。`Add new connection` ページが表示されます。
3.  `Connection Details` セクションで、以下を指定します。
    * **Name:** 新しい接続の `Name` を入力します。Sigmaはこの名前を接続リストに表示します。
    * **Type:** `Databricks` タイルを選択します。

##### **2. 接続資格情報を指定する (Specify your connection credentials)**
`Connection Credentials` セクションで、必須項目を入力します。
1.  `Host` フィールドに、SQLウェアハウスの `Connection details` 画面にある `Server hostname` フィールドの値を入力します。
2.  `HTTP path` フィールドに、SQLウェアハウスの `Connection details` 画面にある `HTTP path` フィールドの値を入力します。
3.  `Authentication` の隣にあるキャレット()をクリックし、認証方法を選択します。
    * 接続をOAuthで認証したい場合は、`OAuth` を選択します。
    * それ以外の場合は、`Basic Auth` を選択し、Databricksでトークンを生成してSigma接続を認証します。手順については、Databricksドキュメントの「[Databricks personal access tokens for service principals](https://docs.databricks.com/en/dev-tools/auth/pat-v2.html)」を参照してください。
4.  次に、接続の認証にOAuthを使用している場合は、「[OAuth機能を構成する](https://help.sigmacomputing.com/docs/connect-to-databricks#configure-oauth-features)」に進みます。OAuthを使用していない場合は、「[書き込みアクセスを構成する](https://help.sigmacomputing.com/docs/connect-to-databricks#configure-write-access)」および「[接続機能を構成する](https://help.sigmacomputing.com/docs/connect-to-databricks#configure-connection-features)」に進みます。または、接続の構成が完了した場合は、右上の `Create` をクリックして接続を作成します。

##### **OAuth機能を構成する (Configure OAuth features)**

`Authentication`ドロップダウンから`OAuth`を選択して、接続の認証方法として構成します。

> 📘
> 接続へのユーザー認証のために一意のOAuthアプリケーションを構成するオプション（つまり、組織レベルで使用するOAuth構成を再利用しないことを選択する）は、パブリックベータ機能であり、制限の対象となります。
> 「[Use different OAuth configurations for authenticating users to your connections than you use for your Sigma organization (Beta)](https://help.sigmacomputing.com/docs/oauth-for-connections-overview)」を参照してください。

1.  [任意] Databricks認証サーバーを使用してSigma組織へのユーザー認証にOAuthを使用しており、組織で[複数のIDプロバイダー（IdP）](https://help.sigmacomputing.com/docs/configure-multiple-idps-for-an-organization)が有効になっていない場合、この接続にそのOAuth構成を再利用するオプションがあります。そのためには、`Use organization-level OAuth configuration`の隣にあるトグルを有効にします。このトグルを有効にした場合は、ステップ3に進みます。
    * 組織の認証方法としてOAuthを使用していない場合、または組織で複数のIdPが有効になっている場合、このオプションは表示されません。外部IdP（Okta, Microsoft Entra ID, Auth0, or PingIndentity）を使用している場合、Databricksは外部IdPを使用した認証をサポートしていないため、このトグルを有効にしないでください。
2.  組織レベルのOAuth構成がない場合、組織で[複数のIdP](https://help.sigmacomputing.com/docs/configure-multiple-idps-for-an-organization)が有効になっている場合、または組織レベルのOAuth構成を再利用したくない場合は、この接続用に一意のOAuth構成を設定します。
    * `OAuth Features`セクションのフィールドを入力する前に、「[Configure a custom OAuth application for Sigma in Databricks Authorization Server](https://help.sigmacomputing.com/docs/configure-databricks-oauth)」の手順を完了してください。
3.  [任意] OAuthトークンのアクセスをさらに指定するために、追加の`Scopes`を入力します。デフォルトのスコープ`openid`, `profile`, `email`, `all-apis`は必須です。デフォルトのスコープ`offline_access`は必須ではありません。
4.  `Metadata URI`フィールドに、OAuthメタデータURIを入力します。この値を取得する方法については、「[Determine your metadata URI for your Databricks Authorization Server](https://help.sigmacomputing.com/docs/configure-databricks-oauth#determine-your-metadata-uri)」を参照してください。
5.  `Client ID`フィールドに、OAuthアプリケーションのクライアントIDを入力します。この値を取得する方法については、「[Configure a custom OAuth application for Sigma in Databricks Authorization Server](https://help.sigmacomputing.com/docs/configure-databricks-oauth)」を参照してください。
6.  `Client Secret`フィールドに、OAuthアプリケーションのクライアントシークレットを入力します。この値を取得する方法については、「[Configure a custom OAuth application for Sigma in Databricks Authorization Server](https://help.sigmacomputing.com/docs/configure-databricks-oauth)」を参照してください。この値を入力して保存すると、Sigmaはそれを表示しません。
7.  `Service Account`が必要かどうかを判断します。サービスアカウントを構成する理由は3つあります。
    * この接続で書き込みアクセスを有効にする場合、サービスアカウントが必要です。
    * Sigmaのパブリック埋め込み機能を使用する場合、サービスアカウントが必要です。
    * 管理者が個々のワークブックを各個人のOAuth資格情報ではなくサービスアカウントを使用して実行するように構成したい場合、サービスアカウントが必要です。
8.  サービスアカウントが必要な場合は、`Service Account`のトグルを有効にし、そのサービスアカウントの`Access token`を入力します。手順については、Databricksドキュメントの「[Databricks personal access tokens for service principals](https://docs.databricks.com/en/dev-tools/auth/pat-v2.html)」を参照してください。
9.  次に、接続の認証にOAuthを使用している場合は、「OAuth機能を構成する」に進みます。OAuthを使用していない場合は、「書き込みアクセスを構成する」および「接続機能を構成する」に進みます。または、接続の構成が完了した場合は、右上の`Create`をクリックして接続を作成します。

##### **接続機能を構成する (Configure connection features)**
`Connection Features` セクションで、以下を指定します。

* **Connection timeout (接続タイムアウト):**
    タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。デフォルトは120秒です。最大は600秒（10分）です。
* **[任意] Use friendly names (分かりやすい名前を使用する):**
    このスイッチをオフにすると、Sigmaが自動でデータソースの列名を読みやすくするのをやめます。例えば、`Use friendly names`がオンの場合、データベースの列`ORDER_NUMBER`は`Order Number`として表示されます。
* **[任意] Enable Hive metastore (Hiveメタストアを有効にする):**
    Sigmaで`hive_metastore`カタログを表示・使用したい場合は、このスイッチをオンにします。デフォルトではオフです。

##### **接続作成を完了する (Finish creating your connection)**
接続の全てのパラメータを指定した後、`Create`をクリックします。
1. 画面右上の`Create`をクリックして接続を作成します。Sigmaは画面に接続の概要を表示します。

2. `Browse Connection`をクリックし、次に`Add permission`をクリックして、組織内のユーザーに接続アクセスを許可します。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。<img width="1347" height="567" alt="b31514d9ab39f7df1c969c6dc7b9abbbdd61d7eccd43909d8c72826a33ce7f7f-databricks-newly-created-connection" src="https://github.com/user-attachments/assets/33a28340-d19d-42e1-9399-1ca085158ecf" />

3. 左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。
<img width="1336" height="381" alt="fdbc21c43fc31c87438bba5aef11a8bdb03d055fcd10e4fe004485e7cd04fb12-databricks-browse-connection" src="https://github.com/user-attachments/assets/a07c3b8a-ed9b-48d3-987e-8d01673c851e" />

#### **Databricks Partner Connect**
DatabricksはSigmaのパートナーの1つなので、そのインターフェースを通じて迅速に接続を確立できます。Databricksドキュメントの「[What is Databricks Partner Connect?](https://docs.databricks.com/en/partner-connect/index.html)」を参照してください。

### 2-1-3-1. Redshiftへの接続 (Connect to Redshift)

SigmaはAmazon Redshiftへの安全な接続をサポートしています。
このドキュメントでは、あなたの組織をAmazon Redshiftウェアハウスに接続する方法を説明します。

> 📘
> Amazon Redshift接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

#### **要件 (Requirements)**

* **あなたのSigma組織にて：**
    * あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* **AWSにて：**
    * 構成済みのクラスターを持つAmazon Redshiftデータウェアハウスへのアクセス権が必要です。この接続で入力テーブルを使用している場合、ノードサイズは`ra3.4xlarge`以上が推奨されます。

#### **Amazon Redshiftを構成する (Configure Amazon Redshift)**

あなたのSigma組織でAmazon Redshift接続を追加する前に、AWSマネジメントコンソールで以下のステップを完了してください。

1.  あなたのAmazon Redshiftクラスターをパブリックアクセス可能に変更し、それに接続するためのElastic IPアドレスを割り当てます。
2.  セキュリティグループを作成し、そのセキュリティグループのインバウンドおよびアウトバウンドルールにSigmaのIPアドレスを追加します。IPアドレスはSigma UIの接続構成ページから取得します。「[Add Sigma IPs to the allowlist](https://help.sigmacomputing.com/docs/connect-to-data-sources#add-sigma-ips-to-the-allowlist)」を参照してください。
3.  あなたのAmazon Redshiftクラスターにセキュリティグループをアタッチします。
4.  あなたのSigma組織への接続のためのサービスアカウントとして機能するAmazon Redshiftユーザーを作成します。
5.  このユーザーに、Redshiftクラスター内の関連する全てのスキーマに対する`USAGE`権限と、それらのスキーマ内の関連する全てのテーブルに対する`SELECT`許可を付与します。スキーマに追加される可能性のある追加のテーブルに対しても、このユーザーが同じ権限を持つように構成します。
    * 権限付与に関するドキュメントは、Amazon Redshiftデータベース開発者ガイドの「[GRANT](https://docs.aws.amazon.com/redshift/latest/dg/r_GRANT.html)」を参照してください。
    * **SQLステートメントの例:**
        ```sql
        CREATE USER your_sigma_service_account_name password ‘a_secure_password’; 
        GRANT USAGE ON SCHEMA your_schema_name TO your_sigma_service_account_name;
        GRANT SELECT ON ALL TABLES IN SCHEMA your_schema_name TO your_sigma_service_account_name;
        ALTER DEFAULT PRIVILEGES IN SCHEMA your_schema_name
        GRANT SELECT ON TABLES TO your_sigma_service_account_name;
        ```
6.  [任意] [ストアドプロシージャアクション](https://help.sigmacomputing.com/docs/stored-procedure-actions)を実行したい場合は、サービスアカウントユーザーに、Sigmaから実行したいストアドプロシージャを含む任意のスキーマに対する`USAGE`と、全てまたは特定のストアドプロシージャに対する`EXECUTE`権限を付与します。
    * **SQLステートメントの例:**
        ```sql
        GRANT USAGE ON SCHEMA your_sproc_schema_name TO your_sigma_service_account_name;
        GRANT EXECUTE ON ALL PROCEDURES IN SCHEMA your_sproc_schema_name TO your_sigma_service_account_name;
        ```
7.  [任意] CSVアップロード、マテリアライゼーション、入力テーブル、ウェアハウスビューなどの書き込みアクセス機能を活用したい場合は、Sigmaの書き戻し機能がデータ書き込みに使用できる専用のスキーマを作成します。
    * そのスキーマに対する`CREATE`権限をあなたのユーザーに付与し、そのスキーマ内の全てのテーブルに対する`SELECT, INSERT, UPDATE, DELETE`を付与します。スキーマに追加される可能性のある追加のテーブルに対しても、あなたのユーザーが同じ権限を持つように構成します。
    * **SQLステートメントの例:**
        ```sql
        GRANT USAGE, CREATE ON SCHEMA your_write_schema_name TO your_sigma_service_account_name;
        GRANT SELECT, INSERT, UPDATE, DELETE ON ALL TABLES IN SCHEMA your_write_schema_name TO your_sigma_service_account_name;
        ALTER DEFAULT PRIVILEGES IN SCHEMA your_write_schema_name
        GRANT SELECT, INSERT, UPDATE, DELETE ON TABLES TO your_sigma_service_account_name;
        ```

#### **SigmaでAmazon Redshift接続を作成する (Create an Amazon Redshift connection in Sigma)**

Amazon Redshift接続を作成するには、Sigma UIで以下のステップを実行します。
1.  接続を追加し、接続詳細を指定する
2.  接続資格情報を指定する
3.  書き込みアクセスを構成する
4.  接続機能を構成する

##### **1. 接続を追加し、接続詳細を指定する**
1.  画面右上のユーザーアイコンをクリックします。
2.  ドロップダウンメニューで、`Add connection`を選択します。
3.  `Connection Details`セクションで、以下を指定します。
    * **Name:** 新しい接続の`Name`を入力します。
    * **Type:** `Redshift`タイルを選択します。

##### **2. 接続資格情報を指定する**
`Connection Credentials`セクションで、必須項目を入力します。
* `Host`フィールドに、あなたのRedshiftクラスターの`General Information`画面にある`Endpoint`フィールドの値を入力します。
  * *例: `cluster.abcd.us-west-1.redshift.amazonaws.com`*
* `Port`フィールドに、あなたのクラスターのポート番号を入力します。
  * *例: `5439`*
* `User`および`Password`フィールドに、あなたのSigma組織に接続するために作成したAmazon Redshiftユーザーのユーザー名とパスワードを入力します。
* `Database`フィールドに、あなたのクラスターのデータベース名を入力します。
* [任意] `Enable TLS`トグルをオンにして、接続のTLS暗号化を有効にします。
* [任意] `SSH Tunnel`トグルをオンにしてSSH経由で接続し、`Tunnel host`と`Tunnel port`を入力します。
* 次に、追加オプションについては「[書き込みアクセスを構成する](#configure-write-access)」および「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の`Create`をクリックして接続を作成します。

##### **3. 書き込みアクセスを構成する**
書き込みアクセスは、以下の機能に必要です。
* CSV upload
* Materialization
* Input tables
* Warehouse views

書き込みアクセスを構成するには、Sigmaがデータ書き込みに使用できる専用のスキーマをAmazon Redshiftで設定し、そのスキーマに対する必要な権限をサービスアカウントに付与する必要があります。
1.  この接続で書き込みアクセスを許可するには、`Enable write access`の隣にあるトグルをオンにします。
2.  `Write schema`フィールドに、Sigmaが書き戻しデータを保存するために作成した専用スキーマの名前を入力します。
3.  次に、追加オプションについては「[接続機能を構成する](#configure-connection-features)」を参照してください。または、接続の構成が完了した場合は、右上の`Create`をクリックして接続を作成します。

##### **4. 接続機能を構成する**
`Connection Features`セクションで、以下を指定します。
* `Connection timeout`フィールドに、タイムアウトまでの時間（秒）を指定します。デフォルトは120秒です。最大は600秒（10分）です。
* [任意] `Use friendly names`トグルをオフにすると、Sigmaが自動で列名を読みやすくするのをやめます。

##### **接続作成を完了する**
1. 接続の全てのパラメータを指定した後、`Create`をクリックします。
画面右上の`Create`をクリックして接続を作成します。Sigmaは画面に接続の概要を表示します。
2. `Browse Connection`をクリックし、`Add permission`をクリックして、組織内のユーザーに接続アクセスを許可します。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。<img width="1324" height="564" alt="641ba71f977c5cce33b88891c248aa71586a969ad54446c8619b176863dc76cb-redshift-new-connection" src="https://github.com/user-attachments/assets/5689b38f-1520-4381-ace6-e7148f367b3e" />

3. 左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。<img width="1336" height="381" alt="c740f832f805473e7f35bebecd259c33c6c024c3485d4c340d11b9ff16c6c0cb-redshift-browse-connection" src="https://github.com/user-attachments/assets/1849e235-3f8d-4d4b-9aee-4e470b693eab" />

#### 2-1-4-1. BigQueryへの接続 (Connect to BigQuery)
SigmaはMySQL（リリース8.0以上）への安全な接続をサポートしています。
このドキュメントでは、あなたの組織をMySQLデータベースに接続する方法を説明します。

> 📘
> MySQL接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

* **お客様 (Customers)**
  この機能へのアクセスは、アカウント担当者を通じてリクエストしてください。
* **見込み客の皆様 (Prospects)**
  この機能へのアクセスは、弊社[セールスチーム](https://www.sigmacomputing.com/contact-sales/)を通じてリクエストしてください。

#### **要件 (Requirements)**
* あなたのSigma組織における管理者権限。詳細は、「[User account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* 関連するデータベースとテーブルに対する `READ` 権限を持つMySQLアカウント。CSVデータをアップロードする予定がある場合は、アカウントは `WRITE` 権限を持っている必要があります。
* SigmaはMySQLバージョン8.0以上をサポートしています。
* データストアに接続する際に使用するアカウントに過剰な権限を付与しないことをお勧めします。例えば、SYSADMINレベルのアクセスは必要ありません。
* Azure上のMySQLは、デフォルトでは名前付きタイムゾーンを持っていません。そのため、Sigmaが正しく動作するためには、タイムゾーンデータをMySQLデータベースにロードする必要があります。そうしないと、接続設定時にエラーが発生する可能性があります。Microsoftのドキュメント「[Populating the time zone tables](https://learn.microsoft.com/en-us/azure/mysql/single-server/how-to-server-parameters#populating-the-time-zone-tables)」を参照してください。これはAWSやGCP上のMySQLでは問題になりません。

#### **接続を作成する (Create a connection)**
接続を作成するには、以下の基本的なステップに従います。

1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection` を選択します。
3.  Add new connections` ページが表示されます。

4. Connection detailsで、以下を指定します。
* **Name**
    新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
    ここでは、`MySQL connection` を使用します。
* **Type**
    使用するデータウェアハウスを表すタイルを選択します。
    ここでは、`MySQL` タイルをクリックします。

5. **Connection Credentialsセクションで、以下を指定します。**
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
6. **Connection Featuresセクションで、以下を指定します。**
* **Connection timeout**
    タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
    デフォルトは120（2分）。最大は600（10分）。
* **Use friendly names**
    このスイッチはデータソースの列名をより読みやすくします。
    例えば、データベースの列 `ORDER_NUMBER` は `Order Number` として表示されます。
    デフォルトでオン。

7. **Write Accessセクションで、書き込みアクセスが必要かどうかを決定します。**
詳細は、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」を参照してください。
* **Enable write access**
    `CSV upload` と `Materialization` に必要です。
    デフォルトでオフ。
    もしオンにする場合は、`Write schema` フィールドを指定します。
* **Write schema**
    Sigmaがテーブルを書き込むスキーマ。
    `Enable write access` がオンの場合にのみ表示されます。

8. **接続の全てのパラメータを指定したら、`Create`をクリックします。**

9. 接続が正常に作成されると、Sigmaはそれを画面に表示します。
10. 接続を確認するには、`Browse Connection` をクリックし、表示されるデータベースとテーブルを探索します。
11. `Add Permission` をクリックして、組織内のユーザーにデータアクセス権を付与します。
詳細は、「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
12. 新しい接続は、あなたのアカウントにある接続のリストにも表示されます。


* #### 2-1-5-1. AlloyDBへの接続 (Connect to AlloyDB)

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
3.  `Add new connections` ページが表示されます。

4.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`AlloyDB connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`AlloyDB` タイルをクリックします。

5.  `Connection Credentials` セクションで、以下を指定します。
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
        クエリを実行します。
      * **Enable TLS (TLSを有効にする)**
    任意。このスイッチは接続のTLS暗号化を有効または無効にします。
    デフォルトで有効。
* **SSH Tunnel (SSHトンネル)**
    任意。このスイッチはセキュアなリモートログインのためのSSHプロトコルを有効にします。詳細は、「[Connect through SSH](https://help.sigmacomputing.com/docs/connect-through-ssh)」を参照してください。
    デフォルトで無効。
    もしオンにする場合は、`Tunnel host`と`Tunnel port`フィールドを指定します。
* **Tunnel host (トンネルホスト)**
    トンネルサーバーへのパス。これはURLまたはIPアドレスです。
    `SSH Tunnel`がオンの場合にのみ表示されます。
* **Tunnel port (トンネルポート)**
    トンネルが接続するポート。
    `SSH Tunnel`がオンの場合にのみ表示されます。

6. ##### **Connection Featuresセクションで、以下を指定します。**
* **Connection timeout (接続タイムアウト)**
    タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
    デフォルトは120（2分）。最大は600（10分）。
* **Use friendly names (分かりやすい名前を使用する)**
    このスイッチはデータソースの列名をより読みやすくします。
    例えば、データベースの列`ORDER_NUMBER`は`Order Number`として表示されます。
    デフォルトでオン。

7. ##### **Write Accessセクションで、書き込みアクセスが必要かどうかを決定します。**
詳細は、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」を参照してください。
* **Enable write access (書き込みアクセスを有効にする)**
    `CSV upload`と`Materialization`に必要です。
    デフォルトでオフ。
    もしオンにする場合は、`Write schema`フィールドを指定します。
* **Write schema (書き込みスキーマ)**
    Sigmaがテーブルを書き込むスキーマ。
    `Enable write access`がオンの場合にのみ表示されます。

8. ##### **接続の全てのパラメータを指定したら、`Create`をクリックします。**

9. 接続が正常に作成されると、Sigmaはそれを画面に表示します。
10.接続を確認するには、`Browse Connection`をクリックし、表示されるデータベースとテーブルを探索します。
11.`Add Permission`をクリックして、組織内のユーザーにデータアクセス権を付与します。
詳細は、「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
12. 新しい接続は、あなたのアカウントにある接続のリストにも表示されます。

#### **AlloyDBクラスタの資格情報を特定する (Locate your AlloyDB cluster credentials)**
1.  Google Cloudコンソールで、`Clusters`ページに移動します。
2.  Sigmaに接続する予定のクラスタをクリックします。
3.  クラスタページが表示されます。 そこには、Sigmaへの接続に必要な資格情報がリストされています。

* #### 2-1-6-1. MySQLへの接続 (Connect to MySQL)

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
3.   Add new connections` ページが表示されます。

4.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`MySQL connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`MySQL` タイルをクリックします。

5.  `Connection Credentials` セクションで、以下を指定します。
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

6.  `Connection Features` セクションで、以下を指定します。
    * **Connection timeout**
        タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
        デフォルトは120（2分）。最大は600（10分）。
    * **Use friendly names**
        このスイッチはデータソースの列名をより読みやすくします。
        例えば、データベースの列 `ORDER_NUMBER` は `Order Number` として表示されます。
        デフォルトでオン。

7.  `Write Access` セクションで、書き込みアクセスが必要かどうかを決定します。
    * 詳細は、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」を参照してください。
    * **Enable write access**
        `CSV upload` と `Materialization` に必要です。
        デフォルトでオフ。
        もしオンにする場合は、`Write schema` フィールドを指定します。
    * **Write schema**
        Sigmaがテーブルを書き込むスキーマ。
        `Enable write access` がオンの場合にのみ表示されます。

8.  接続の全てのパラメータを指定したら、`Create` をクリックします。

9.  接続が正常に作成されると、Sigmaはそれを画面に表示します。
10. 接続を確認するには、`Browse Connection` をクリックし、表示されるデータベースとテーブルを探索します。
11. `Add Permission` をクリックして、組織内のユーザーにデータアクセス権を付与します。
詳細は、「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
12. 新しい接続は、あなたのアカウントにある接続のリストにも表示されます。

#### 2-1-7. PostgreSQLへの接続 (Connect to PostgreSQL)

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
3.  * `Add new connections` ページが表示されます。

4.  `Connection details` で、以下を指定します。
    * **Name**
        新しい接続の `Name` を指定します。Sigmaはこの名前を接続リストに表示します。
        ここでは、`PostgreSQL connection` を使用します。
    * **Type**
        使用するデータウェアハウスを表すタイルを選択します。
        ここでは、`PostgreSQL` タイルをクリックします。
5.  **Connection Credentialsセクションで、以下のフィールドを指定します。**
* **Host**
    あなたのデータベースへのパス。
    これはURLまたはIPアドレスです。
    「[Connection credentials](#connection-credentials)」を参照してください。
* **Port**
    Sigmaがホストへの接続に使用するポート。
    PostgreSQLのデフォルトポートは `5432` です。
* **User**
    PostgreSQLデータウェアハウスへの接続に使用するユーザー名またはアカウント。
    例：`test`
* **Password**
    PostgreSQLアカウントの `User` に対応するパスワードを入力します。
* **Database**
    クエリを実行する予定のデータベースの名前。
* **Enable TLS**
    任意。
    このスイッチは接続のTLS暗号化を有効または無効にします。
    デフォルトで有効。
* **SSH Tunnel**
    任意。
    このスイッチはセキュアなリモートログインのためのSSHプロトコルを有効にします。詳細は、「[Connect through SSH](https://help.sigmacomputing.com/docs/connect-through-ssh)」を参照してください。
    デフォルトで無効。
    もしオンにする場合は、`Tunnel host` と `Tunnel port` フィールドを指定します。
* **Tunnel host**
    トンネルサーバーへのパス。
    これはURLまたはIPアドレスです。
    `SSH Tunnel` がオンの場合にのみ表示されます。
* **Tunnel port**
    トンネルが接続するポート。
    `SSH Tunnel` がオンの場合にのみ表示されます。

6. **Connection Featuresセクションで、以下を指定します。**
* **Connection timeout**
    タイムアウト（またはキャンセル）までの時間（秒単位）。Sigmaがクエリ結果の返却を待つ時間です。
    デフォルトは120（2分）。
    最大は600（10分）。
* **Use friendly names**
    このスイッチはデータソースの列名をより読みやすくします。
    例えば、データベースの列`ORDER_NUMBER`は`Order Number`として表示されます。
    デフォルトでオン。
7. **Write Accessセクションで、書き込みアクセスが必要かどうかを決定します。**
詳細は、「[Set up write access](https://help.sigmacomputing.com/docs/set-up-write-access)」を参照してください。
* **Enable write access**
    `CSV upload`と`Materialization`に必要です。
    デフォルトでオフ。
    もしオンにする場合は、`Write schema`フィールドを指定します。
* **Write schema**
    Sigmaがテーブルを書き込むスキーマ。
    `Enable write access`がオンの場合にのみ表示されます。

8.  **接続の全てのパラメータを指定したら、`Create`をクリックします。**

9. 接続が正常に作成されると、Sigmaはそれを画面に表示します。
10. 接続を確認するには、`Browse Connection`をクリックし、表示されるデータベースとテーブルを探索します。
11. `Add Permission`をクリックして、組織内のユーザーにデータアクセス権を付与します。
詳細は、「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
12. 新しい接続は、あなたのアカウントにある接続のリストにも表示されます。

#### **Sigma用にPostgreSQLを構成する (Configure PostgreSQL for Sigma)**

以下のステップに従って、Sigmaに接続するためにPostgreSQLを構成します。

1.  EC2コンソールで、**Elastic IP**に移動します。<img width="700" height="682" alt="0f87750-8" src="https://github.com/user-attachments/assets/8e13ab6f-718a-40a0-8d7d-7dac18f49752" />

2.  **Elastic IP Address**を作成します。
    * このステップは、IPアドレスを公開アクセス可能にするために必要です。
3.  **Allocate Elastic IP address**をクリックします。<img width="613" height="84" alt="fa5e5e5-9" src="https://github.com/user-attachments/assets/750a4cd9-9631-4a07-8a0a-46455feda2f0" />

4.  **Allocate**をクリックします。
5.  あなたのRedshiftクラスターに戻り、**Actions**をクリックします。
6.  **Modify publicly accessible setting**をクリックします。
7.  **Enable**をクリックし、**Elastic IP Address**ドロップダウンで作成した**Elastic IP address**を選択します。<img width="682" height="418" alt="ce17489-10" src="https://github.com/user-attachments/assets/d38f31d3-f4a2-433a-8795-eb0f9b435ace" />

8.  EC2コンソールで、**Security Groups**に移動します。<img width="687" height="593" alt="193ce25-11" src="https://github.com/user-attachments/assets/2518bc4c-5184-48df-8b36-cd0d95e364b9" />

9.  **Create security group**ページで、セキュリティグループに名前と説明を付けます。<img width="511" height="202" alt="bb7fe1b-12" src="https://github.com/user-attachments/assets/5a0f7b26-a85d-48da-9539-cac4bb5bd920" />

    * 注：VPCは、共通のセキュリティと相互接続を共有するインフラ、プラットフォーム、アプリケーションサービスによって構成されるエラスティックネットワークです。
10. SigmaのIPアドレスを**Inbound rules**と**Outbound rules**の両方に追加します。<img width="1243" height="319" alt="6791ad9-13" src="https://github.com/user-attachments/assets/684f442c-f87b-492d-b59f-8ff55b4471d5" />

    * **GCP Sigma hosting :** `104.197.169.18`, `104.197.193.23`
    * **AWS Sigma hosting:** `44.229.241.60`, `54.188.54.135`
11. あなたのPostgreSQLクラスターに戻り、**Properties**タブをクリックします。. **Network and security settings**タブの**Edit**をクリックします。<img width="596" height="140" alt="75bddb9-14" src="https://github.com/user-attachments/assets/0af6ef90-8cb2-40a2-aeaf-7fecc2e0db78" />

12. 作成した**VPC Security Group**を選択し、**Save Changes**をクリックします。<img width="700" height="589" alt="85727e9-15" src="https://github.com/user-attachments/assets/0ed3268a-6e5d-4192-a757-386d7abc3cf9" />

##### **データ権限 (Data permissions)**
既存のPostgreSQLユーザーを使用したくない場合は、Sigma用に新しいユーザーを作成してください。書き込みアクセスを活用したい場合は、Sigma用にスキーマを作成し、そのスキーマに対する全ての権限をあなたのユーザーに付与してください。Sigmaでアクセスする予定の全てのスキーマに対して `USAGE` を、全てのテーブルに対して `SELECT` を付与するようにしてください。

```sql
create user sigma_user password ‘123’;
create schema sigma_write;
grant all privileges on schema sigma_write to sigma_user;
grant usage on schema public to sigma_user;
grant select on all tables in schema public to sigma_user;
```

<img width="514" height="248" alt="b7ac16d-16" src="https://github.com/user-attachments/assets/a103ca32-5883-444d-b232-d435d3dc3925" />

##### **接続資格情報 (Connection credentials)**
あなたのPostgreSQLクラスターの `General Information` セクションで、`Endpoint` の仕様を見つけてコピーします。これがSigmaの `Host` フィールドの値です。
<img width="676" height="165" alt="248cb87-17" src="https://github.com/user-attachments/assets/61fd7fb5-012f-438c-a5d7-bb5549bdf4e7" />

### 2-13. Starburstへの接続 (Connect to Starburst)

Sigmaは、Snowflake、Databricks、BigQuery、またはPostgreSQLデータウェアハウスに接続するために、TrinoのSaaSディストリビューションであるStarburst Galaxyの使用をサポートしています。

このドキュメントでは、あなたのSigma組織を[Starburst Galaxy](https://www.starburst.io/platform/starburst-galaxy/)クラスターに接続する方法を説明します。

> 📘
> Starburst接続とのSigma機能の互換性に関する情報は、「[Region, warehouse, and feature support](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

#### **要件 (Requirements)**
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* Sigmaがアクセスする必要のある全てのテーブルに対する`Select from table`権限と、クラスターに対する`Use cluster`権限を持つStarburst Galaxyサービスアカウントの資格情報が必要です。

#### **Starburst接続を作成する (Create a Starburst connection)**
1.  画面右上のユーザーアイコンをクリックします。
    * ユーザーアイコンは通常、あなたのイニシャルで構成されています。
2.  ドロップダウンメニューで、`Add connection`を選択します。
3.　`Add new connection`ページが表示されます。
4.  `Connection details`で、以下を指定します。
    * **Name:** 新しい接続の`Name`を入力します。Sigmaはこの名前を接続リストに表示します。
    * **Type:** `Starburst`を選択します。
5.  `Connection Credentials`セクションで、フィールドを入力します。
    * **Host:** URLまたはIPアドレスとしての、あなたのStarburst Galaxyクラスターのアドレス。
    * **Port:** SigmaがあなたのStarburst Galaxyクラスターに接続するためのポート。
    * **User:** あなたのStarburst管理者によって設定されたサービスアカウントのユーザー名。
    * **Password:** あなたのStarburst管理者によって設定されたサービスアカウントのパスワード。
6.  (任意) `Connection features`セクションで、必要に応じてデフォルト値を調整します。
    * **Connection timeout:** タイムアウトまでの時間（秒単位）。デフォルトは120秒、最大は600秒です。
    * **Use friendly names:** この設定はデフォルトでオンになっており、データソースの列名をより読みやすくします。
7.  接続の全てのパラメータを指定したら、`Create`をクリックします。Sigmaは画面に接続の概要を表示します。
<img width="1101" height="166" alt="d0d5a22-connectionsummary" src="https://github.com/user-attachments/assets/f0d41072-3fb4-4e6d-a7f5-64d96cd0d109" />
8.  `Browse Connection`をクリックし、次に`Add permission`をクリックして、組織内のユーザーにデータアクセスを許可します。
<img width="1034" height="510" alt="452f1a2-Addpermissions" src="https://github.com/user-attachments/assets/c6f74fef-dadb-4b7b-8a44-09ca987097aa" />
9.  左側のナビゲーションパネルを使用して、接続内のデータベースとテーブルを探索します。
<img width="1386" height="332" alt="5493f7d-exploreconnection" src="https://github.com/user-attachments/assets/55321f57-4e72-4c59-9e0b-308a1e120138" />
10. 新しい接続は、あなたのアカウントにある接続のリストにも表示されます。

### 2-1-9. Azure SQL Databaseへの接続 (Connect to Azure SQL Database)

SigmaはAzure SQL Databaseへの安全な接続をサポートしています。
このドキュメントでは、あなたのSigma組織を[Azure SQL Database](https://azure.microsoft.com/en-us/products/azure-sql/database)に接続する方法を説明します。

#### **要件 (Requirements)**
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* データベースのネットワーク設定を構成するために、Azureで適切なアクセス権を持っている必要があります。
* サポートされているインスタンスタイプを持っている必要があります。「[インスタンスタイプを確認する](#verify-my-instance-type)」を参照してください。

#### **インスタンスタイプを確認する (Verify my instance type)**
インスタンスタイプを確認するには、データベースインスタンスで以下のクエリを実行します。
`select serverproperty('ProductMajorVersion'),serverproperty('EngineEdition')`

`EngineEdition`が`5`のインスタンスがサポートされています。
以下の場合、代わりにSQL Server 2022接続を使用してください。
* `EngineEdition`が`1`, `2`, `3`, `4`で、`ProductMajorVersion`が`16.x`の場合
* `EngineEdition`が`8`の場合
「[Connect to SQL Server 2022](https://help.sigmacomputing.com/docs/connect-to-sql-server-2022)」を参照してください。
クエリ出力の解釈に関する情報は、Microsoftのドキュメント「[SERVERPROPERTY](https://learn.microsoft.com/en-us/sql/t-sql/functions/serverproperty-transact-sql)」を参照してください。

#### **Azure SQL Database接続を作成する (Create an Azure SQL Database connection)**
1.  画面右上のユーザーアイコンをクリックします。
2.  ドロップダウンメニューで、`Add connection`を選択します。
3.  `Connection Details`セクションで、以下を指定します。
    * **Name:** 新しい接続の`Name`を入力します。
    * **Type:** `Azure SQL DB`を選択します。

SigmaのIPアドレスを許可するために、Azureデータベースのネットワーク設定を構成する必要があります。これを行うには、Azureのドキュメント「[Network Access Controls](https://learn.microsoft.com/en-us/azure/azure-sql/database/network-access-controls-overview)」を参照してください。必要なSigmaのIPは、`Connection Credentials`セクションの`Server`フィールドの下にあります。

##### **Connection Credentialsセクションで、以下を指定します。**
* **Server:** 完全修飾ホスト名またはIPアドレス。「[サーバー接続情報を取得する](https://learn.microsoft.com/en-us/azure/azure-sql/database/connect-query-portal)」に関するMicrosoftのドキュメントを参照してください。
* **Database:** クエリを実行したいデータベースの名前。
* **Port:** SigmaがAzure SQL Databaseクラスターに接続するためのポート。デフォルトポートは1433です。
* **User:** Azure SQL Database管理者によって設定されたサービスアカウントのユーザー名。
* **Password:** Azure SQL Database管理者によって設定されたサービスアカウントのパスワード。

##### **Connection Featuresセクションで、以下を指定します。**
* **Connection Timeout:** タイムアウトまでの時間（秒）。デフォルトは120秒、最大は600秒です。
* **Use friendly names:** この設定はデフォルトでオンになっており、データソースの列名をより読みやすくします。

##### **接続作成を完了する**
`Browse Connection`をクリックし、次に`Add permission`をクリックして、組織内のユーザーにデータアクセスを許可します。
左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。新しい接続は、あなたのアカウントにある接続のリストにも表示されます。

#### **書き込みアクセスを構成する (Configure write access)**
書き込みアクセスは[マテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)に必要です。書き込みアクセスを構成するには、専用のデータベースとスキーマを設定し、必要な権限を付与する必要があります。
1.  Sigma接続の構成に使用するAzure SQL Databaseユーザーに、以下の権限を持つロールを付与します。

| オブジェクト | 権限 |
| :--- | :--- |
| **Schema** | CREATE TABLE, CREATE VIEW, ALTER |

2.  Sigmaで、`Connections`に移動し、Azure SQL Database接続を選択して`Edit`を選択します。
3.  `Enable write access`トグルをオンにし、以下を構成します。
    * `Write schema`フィールドに、Sigmaが書き戻しデータを保存するデータベーススキーマを入力します。

#### **機能の制限 (Feature Limitations)**
現在、Azure SQL Database接続は以下の機能をサポートしていません。
* Sigmaで作成されたデータセットウェアハウスビュー
* ワークブックウェアハウスビュー
* クラウドストレージへのエクスポート
* OAuth接続
* Sigma結果IDキャッシュ
* ロールとウェアハウス切り替えのためのユーザー属性
* 書き戻し機能：CSVアップロード、入力テーブル
* 地理データ型
* すべての地理関数
* 特定のパススルー関数（Geography, Variant, Logical）
* 特定のウィンドウ関数（CumulativeCorr, MovingCorr, Corr）
* CTEを含むカスタムSQL

### 2-1-10. SQL Server 2022およびAzure SQL Managed Instanceへの接続

#### **要件 (Requirements)**
* SQL Server 2022は、仮想マシン上にあるか、インターネット経由で公開アクセス可能であるか、または[Azure SQL Managed Instance](https://azure.microsoft.com/en-us/products/azure-sql/managed-instance)である必要があります。他のバージョンのSQL Serverはサポートされていません。
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* データベースのネットワーク設定を構成するために、Azureで適切なアクセス権を持っている必要があります。
* サポートされているインスタンスタイプを持っている必要があります。「[インスタンスタイプを確認する](#verify-my-instance-type)」を参照してください。

#### **インスタンスタイプを確認する (Verify my instance type)**
インスタンスタイプを確認するには、データベースインスタンスで以下のクエリを実行します。
`select serverproperty('ProductMajorVersion'),serverproperty('EngineEdition')`

以下を持つインスタンスがサポートされています。
* `EngineEdition`が`1`, `2`, `3`, `4`で、`ProductMajorVersion`が`16.x`
* `EngineEdition`が`8`

`EngineEdition`が`5`の場合は、Azure SQL Database接続を使用してください。「[Connect to Azure SQL Database](https://help.sigmacomputing.com/docs/connect-to-azure-sql-database)」を参照してください。
クエリ出力の解釈に関する情報は、Microsoftのドキュメント「[SERVERPROPERTY](https://learn.microsoft.com/en-us/sql/t-sql/functions/serverproperty-transact-sql)」を参照してください。

#### **SQL Server 2022またはAzure SQL Managed Instance接続を作成する**
1.  画面右上のユーザーアイコンをクリックします。
2.  ドロップダウンメニューで、`Add connection`を選択します。
3.  `Connection Details`セクションで、以下を指定します。
    * **Name:** 新しい接続の`Name`を入力します。
    * **Type:** `SQL Server`を選択します。

4. SigmaのIPを許可するために、データベースのネットワーク設定を構成する必要があります。これを行うには、Azureのドキュメント「[Network Access Controls](https://learn.microsoft.com/en-us/azure/azure-sql/database/network-access-controls-overview)」を参照してください。必要なSigmaのIPは、Connection CredentialsセクションのServerフィールドの下にあります。

5. **Connection Credentialsセクションで、以下を指定します。**
* **Server:** 完全修飾ホスト名またはIPアドレス。「[Connect to SQL Server](https://learn.microsoft.com/en-us/sql/database-engine/configure-windows/connect-to-sql-server-when-system-administrators-are-locked-out)」に関するMicrosoftのドキュメントを参照してください。
* **Port:** SigmaがSQL Serverに接続するためのポート。デフォルトポートは1433です。
* **User:** SQL Server管理者によって設定されたサービスアカウントのユーザー名。
* **Password:** SQL Server管理者によって設定されたサービスアカウントのパスワード。

6. **Connection Featuresセクションで、以下を指定します。**
* **Connection Timeout:** タイムアウトまでの時間（秒）。デフォルトは120秒、最大は600秒です。
* **Use friendly names:** この設定はデフォルトでオンになっており、データソースの列名をより読みやすくします。

7.  **接続作成を完了する**
8. `Browse Connection`をクリックし、次に`Add permission`をクリックして、組織内のユーザーにデータアクセスを許可します。
左側のナビゲーションパネルを使用して、接続のスキーマやテーブルを探索します。新しい接続は、あなたのアカウントにある接続のリストにも表示されます。
<img width="1048" height="441" alt="c98c5ff04834a29fca916cd7b2f97d69392e38a7ab3fb0de743a4e509fc3d9cd-sqlserver" src="https://github.com/user-attachments/assets/53b4db4c-0e16-47ee-96b4-fd74f1fc15a3" />

#### **書き込みアクセスを構成する (Configure write access)**
書き込みアクセスは[マテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)に必要です。書き込みアクセスを構成するには、専用のデータベースとスキーマを設定し、必要な権限を付与する必要があります。
1.  Sigma接続の構成に使用するSQL Server 2022/Azure SQL Managed Instanceユーザーに、以下の権限を持つロールを付与します。

| オブジェクト | 権限 |
| :--- | :--- |
| **Database** | CREATE TABLE |
| **Schema** | CREATE TABLE, CREATE VIEW, ALTER |

2.  Sigmaで、`Connections`に移動します。SQL Server 2022/Azure SQL Managed Instance接続を選択し、`Edit`を選択します。
3.  `Enable write access`トグルをオンにし、以下のフィールドを構成します。
    * `Write database`フィールドに、Sigmaが書き戻しデータを保存するデータベースの名前を入力します。
    * `Write schema`フィールドに、Sigmaが書き戻しデータを保存するデータベーススキーマを入力します。

#### **機能の制限 (Feature Limitations)**
現在、SQL Server 2022/Azure SQL Managed Instance接続は以下の機能をサポートしていません。
* Sigmaで作成されたデータセットウェアハウスビュー
* クラウドストレージへのエクスポート
* OAuth接続
* Sigma結果IDキャッシュ
* ロールとウェアハウス切り替えのためのユーザー属性
* 書き戻し機能：CSVアップロードと入力テーブル
* 地理データ型
* すべての地理関数
* 特定のパススルー関数（AggGeography, CallGeography）
* 特定のウィンドウ関数（CumulativeCorr, MovingCorr, Median）
* CTEを含むカスタムSQL

### 2-2-1. 書き込みアクセスを設定する (Set up write access)

[入力テーブル](https://help.sigmacomputing.com/docs/input-tables-overview)、[ウェアハウスビュー](https://help.sigmacomputing.com/docs/warehouse-views)、[マテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)、および[CSVアップロード](https://help.sigmacomputing.com/docs/upload-csv-data)といった機能の使用を有効にするために、書き込みアクセスを設定します。

> 📘
> あなたの組織が接続の認証にOAuthを使用している場合、追加の構成ステップがあります。詳細は「[Configure OAuth with write access](https://help.sigmacomputing.com/docs/oauth-with-write-access)」を参照してください。

#### **システムとユーザーの要件 (System and user requirements)**
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* 書き込み先のデスティネーションを作成し、権限を構成するために、あなたのクラウドデータウェアハウス（CDW）で必要な権限を持っている必要があります。

#### **あなたのデータプラットフォームで、書き込みアクセスのためのデスティネーションと権限を設定する**
書き込みアクセスを設定するためには、Sigmaがあなたのデータプラットフォームで十分な権限を持っていることを確認してください。

各CDWは、固有のデータベース構造と権限モデルを持っています。あなたのCDWのドキュメントに従って、Sigmaがデータを書き戻すために使用できるデスティネーションを作成し、あなたが構成した認証情報を使用してSigmaが書き戻しを実行できるように、必要な権限を適用してください。

> 💡
> 設計上、あなたが書き込みアクセス用に構成したデスティネーションは、Sigmaの接続エクスプローラーパネルには表示されません。Sigmaがこのデスティネーションに書き込むデータは、閲覧したり使用したりできる形式にはなっていません。書き込みアクセスの目的のためには、別のデータベース、またはデータベースとスキーマの組み合わせを構成してください。

#### **Sigmaで書き込みアクセスを構成する (Configure write access in Sigma)**
1.  画面右上のユーザーメニューで`Administration`を選択します。
2.  左側のパネルから`Connections`ページを選択します。
3.  接続を表示するために、リスト内の既存の接続をクリックします。
4.  `Edit`をクリックします。
5.  `Write access`の下にある`Enable write access`のスイッチをオンにします。
6.  Sigmaは書き込みアクセスのための追加情報を要求します。この情報は、あなたのCDWの仕様に依存します：`Snowflake`, `BigQuery`, `PostgreSQL`, `Redshift`, `Databricks`, `AlloyDB`, および `MySQL`。
7.  フォームへの入力を完了したら、`Save`をクリックします。

### 2-2-2. OAuthでの書き込みアクセスを構成する (Configure OAuth with write access)

Sigmaでは、[入力テーブル](https://help.sigmacomputing.com/docs/input-tables-overview)、[ウェアハウスビュー](https://help.sigmacomputing.com/docs/warehouse-views)、[ワークブックとデータモデルのマテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)、および[CSVアップロード](https://help.sigmacomputing.com/docs/upload-csv-data)のような書き込みアクセス機能で、OAuthの権限管理の利点を活用できます。

このドキュメントでは、Sigmaオブジェクト（書き込みアクセス機能を使用して作成または編集されたもの）のための安全で効率的な書き戻しワークフローを有効にするために、OAuth接続を構成する方法について説明します。OAuthと一般的な使用法に関する詳細は、「[OAuthを構成する](https://help.sigmacomputing.com/docs/configure-okta-oauth-for-sigma)」を参照してください。

> 📘
> 設計上、あなたが書き込みアクセス用に構成したデスティネーションは、Sigmaの接続エクスプローラーパネルには表示されません。Sigmaがこのデスティネーションに書き込むデータは、閲覧したり使用したりできる形式にはなっていません。書き込みアクセスの目的のためには、別のデータベース、またはデータベースとスキーマの組み合わせを構成してください。

#### **システムとユーザー要件 (System and user requirements)**
OAuth接続を書き込みアクセスで構成する機能には、以下が必要です。
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* Sigmaの書き込みアクセス機能で使用されるすべての書き込みデスティネーションのスキーマパス（入力テーブルの編集ログデスティネーションのスキーマパスを含む）を提供できる必要があります。
* また、入力テーブルの編集ログデスティネーションに書き込む権限を持つサービスアカウントの資格情報を提供できる必要もあります。
    * Snowflakeの場合、サービスアカウントはSnowflakeの編集ログデスティネーションスキーマに対する`CREATE`権限が必要です。
    * Databricksの場合、サービスアカウントは`DATA EDITOR`権限が必要です。

#### **書き込みアクセス機能を持つOAuthについて (About OAuth with write access features)**
書き込みアクセス機能を持つOAuth接続を使用するには、Sigmaは一つ以上のスキーマをSigmaオブジェクトデータの書き込みデスティネーションとして指定することを要求します。OAuthはデータウェアハウス内の各個人ユーザーに付与されたデータ権限を使用するため、それらのユーザーは構成された書き戻しデスティネーションへの書き込みを承認されている必要があります。

ユーザーが特定のデスティネーションへの書き込みを承認されているかどうかを判断するために、SigmaはCDW内のユーザーの対応するユーザーアカウント（サービスアカウントではない）を利用して、各書き込みデスティネーションスキーマにテーブルを作成しようと試みます。テーブルが正常に作成された場合、そのスキーマの書き込みアクセスが確認され、検証テーブルは削除されます。Sigmaはユーザーがログインする際に検証プロセスを開始し、承認された書き込みデスティネーションはセッションの期間中キャッシュされ、クエリの頻度を減らします。
> 🚧
> 書き込みアクセス検証プロセスによって作成されたテーブルは、`SIGDS`で始まるオブジェクト名で簡単に識別できます。書き込みアクセス機能の適切な機能を確保するために、`SIGDS`プレフィックスを持つテーブルは変更しないでください。

ユーザーがOAuth接続の書き込みデスティネーションとして指定された一つのスキーマへの書き込みのみを承認されている場合、彼らが作成するSigmaオブジェクトはデフォルトでそのデスティネーションに書き込まれます。それ以外の場合、Sigmaはオブジェクトを作成する際に、ユーザーが複数のデスティネーションから選択できるようにします。
> 💡
> Snowflakeでは、書き込み権限はSnowflakeのプライマリまたはセカンダリロールを通じてユーザーに付与できます。ただし、オブジェクトを作成する能力はプライマリロールを通じて付与される必要があります。

##### **ウェアハウスビュー、マテリアライゼーション、CSVアップロードの書き戻しアーキテクチャ**
以下のステップは、OAuth接続がSigmaにワークブックのウェアハウスビュー、ワークブックとデータモデルのマテリアライゼーション、およびCSVアップロードをCDWに書き込むことを可能にする方法を説明します。
1.  Sigma UIで、ユーザーは指定された書き込みデスティネーションでSigmaオブジェクトを作成または編集します。
2.  Sigma UIはオブジェクトデータをSigmaのWebサービスに送信します。
3.  SigmaのWebサービスは、SigmaデータベースからユーザーのOAuth資格情報を取得します。
4.  SigmaのWebサービスは、ユーザーのOAuth資格情報を適用してCDWへのアクセスを承認し、オブジェクトデータを指定された書き込みデスティネーションスキーマに書き込みます。
<img width="950" height="491" alt="fef8d78e33e588b5c30bb60baa76566d312d9d9676ae928c01c8adedcfaed0bf-Screenshot_2024-08-27_at_3 12 39_PM" src="https://github.com/user-attachments/assets/2edeed86-61ae-419a-b0af-046b04203462" />

#### **入力テーブルを持つOAuthについて (About OAuth with input tables)**
組織が入力テーブルを利用する場合、書き込みアクセスでOAuthを有効にするには、スキーマを入力テーブルの編集ログデスティネーションとして指定する必要があります。
編集ログ（先行書き込みログまたはWALとも呼ばれる）は、ユーザーアクティビティと結果として生じるシステム操作（編集レコードとして保存される入力テーブルデータを含む）に関連する情報を保存する、入力テーブルの変更のシーケンシャルな記録です。
Sigmaはまた、CDWの編集ログデスティネーションスキーマに書き込むために必要な権限が付与されたサービスアカウントの資格情報を提供することも要求します。
> 🚧
> 編集ログに対応するテーブルとすべての入力テーブルは、`SIGDS`で始まるオブジェクト名で簡単に識別できます。適切な入力テーブルの機能を確保するために、`SIGDS`プレフィックスを持つテーブルは変更しないでください。

#### **入力テーブルの書き戻しアーキテクチャ (Write-back architecture for input tables)**
以下のステップは、OAuth接続がSigmaにCDWに入力テーブルを書き込むことを可能にする方法を説明します。
1.  Sigma UIで、ユーザーは指定された書き込みデスティネーションで入力テーブルを作成または編集します。
2.  Sigma UIはオブジェクトデータをSigmaのWebサービスに送信します。
3.  SigmaのWebサービスは、Sigmaデータベースから接続のサービスアカウント資格情報を取得します。
4.  SigmaのWebサービスは、サービスアカウント資格情報を適用してCDWアクセスを承認し、入力テーブルの変更情報を編集ログデスティネーションスキーマに書き込みます。
5.  SigmaのWebサービスは、Sigmaデータベースから**ユーザー**のOAuth資格情報を取得します。
6.  SigmaのWebサービスは、**ユーザー**のOAuth資格情報を適用してCDWアクセスを承認し、オブジェクトデータを指定された書き込みデスティネーションスキーマに書き込みます。
<img width="1151" height="489" alt="062ff4a5d9669ebb6b6c9edaa61856a240ea4e28c77bf485c2ac4d226fddae2f-Screenshot_2024-08-27_at_3 15 09_PM" src="https://github.com/user-attachments/assets/9a6d5f45-67cf-493e-8ac6-36cea9661618" />

#### **入力テーブルを持つOAuthにアップグレードする際のベストプラクティス (Best practices when upgrading to OAuth with input tables)**

組織が入力テーブルを使用する場合、非OAuth接続をOAuthを使用するようにアップグレードする際には、以下の情報とベストプラクティスに注意することが重要です。

アップグレード前に接続に書き込まれた入力テーブルは、以前のデスティネーションスキーマが新しい書き込みデスティネーションとして構成されているかどうかに関係なく、Sigmaで引き続き表示できます。ただし、ユーザーが既存の入力テーブルに書き込みを続けるには、CDW内の以前のデスティネーションスキーマへの書き込み権限が付与されている必要があります。

OAuthを使用したシームレスな移行のために、編集ログデスティネーションは、アップグレード前に接続の書き戻しデスティネーションとして構成されていたのと同じスキーマパスでなければなりません。編集ログデスティネーションとして異なるスキーマパスを構成する必要がある場合は、編集ログに対応するテーブルも新しいデスティネーションに移動する必要があります。

例えば、Snowflakeでは、以下のSQLステートメントを使用して編集ログテーブルを新しいデスティネーションに移動します。
```sql
ALTER TABLE {original_db}.{original_schema}.{original_table} RENAME TO {new_db}.{new_schema}.{new_table};
```

各接続には、`SIGDS`という名前の単一の編集ログテーブルがあります。複数の接続が同じ編集ログデスティネーションを使用する場合、そのデスティネーションスキーマには`SIGDS_WAL`プレフィックスを持つ複数のテーブルが含まれることがあります。特定の接続に対して正しい編集ログテーブルを移動するようにしてください。

### 2-2-2-1. サービスアカウントの資格情報でワークブックを実行する (Run a workbook with service account credentials)

サービスアカウントを持つOAuth接続からのデータで作成されたワークブックでは、管理者は各ユーザーのOAuth資格情報の代わりに、サービスアカウントを使用してクエリを実行するようにワークブックを構成できます。

所有者がSigmaに長時間ログインしない場合、OAuthトークンは期限切れになる可能性があります。これが発生すると、そのユーザーによって構成されたスケジュールされたエクスポートとマテリアライゼーションのスケジュールは失敗します。この制限は、サービスアカウントの資格情報でワークブックを実行することで回避できます。

この設定は、Sigmaがデータをクエリし、ワークブックの権限を評価する方法を変更します。以下の表を参照して、動作を比較してください。

| ワークブックの接続 | `Run as service account`は構成されているか？ | Sigmaがデータをクエリし、権限を評価する方法 |
| :--- | :--- | :--- |
| **非OAuth接続を使用するワークブック** | N/A | Sigmaはワークブック所有者の[ソースデータへの権限](https://help.sigmacomputing.com/docs/data-permissions)を評価し、次に接続設定で設定されたユーザーアカウントの資格情報を使用してクエリを実行します。 |
| **OAuth接続を使用するワークブック** | **はい** | Sigmaは、Sigma内から閲覧されるか、スケジュールされたレポートの一部として実行されるたびに、データ接続のサービスアカウント資格情報を使用してワークブックの公開バージョンにクエリを実行します。これにより、ワークブックに[権限](https://help.sigmacomputing.com/docs/share-a-workbook)を持つどのユーザーも、クラウドデータウェアハウスでの権限に関係なく、それを表示できます。 |
| **OAuth接続を使用するワークブック** | **いいえ** | Sigmaは常に組織メンバーのOAuth資格情報でクエリを実行します。これには、ユーザーが他人の所有するワークブックを閲覧している場合も含まれます。 |
| **OAuth接続と非OAuth接続の両方からのデータを使用するワークブック** | **はい** | OAuth接続からのデータについては、Sigmaはサービスアカウント資格情報を使用します。<br>非OAuth接続からのデータについては、Sigmaはワークブック所有者の権限を評価し、接続設定の資格情報を使用します。 |
| **OAuth接続と非OAuth接続の両方からのデータを使用するワークブック** | **いいえ** | OAuth接続からのデータについては、Sigmaは常にユーザーのOAuth資格情報を使用します。<br>非OAuth接続からのデータについては、Sigmaはワークブック所有者の権限を評価し、接続設定の資格情報を使用します。 |
| **異なるOAuth構成を持つ2つの異なるOAuth接続からのデータを使用するワークブック** | **はい** | Sigmaは、各データ接続のサービスアカウント資格情報を使用してワークブックの公開バージョンにクエリを実行します。 |
| **異なるOAuth構成を持つ2つの異なるOAuth接続からのデータを使用する-ワークブック** | **いいえ** | Sigmaは、各接続用に構成されたユーザーのOAuth資格情報で常にクエリを実行します。 |

#### **要件 (Requirements)**
* ワークブックでこの設定を構成するには、`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* `Run as service account`オプションは、以下の基準を満たすOAuth接続を使用するワークブックでのみ利用可能です。
    * OAuth接続用にサービスアカウントが構成されている。
    * OAuthが組織レベルで構成されている。（この機能は独立したOAuthを持つ接続では利用できません。）

#### **個々のワークブックをサービスアカウントとして実行する (Run an individual workbook as a service account)**
1.  ワークブックを`Published`モードで開きます。
2.  キャレット()をクリックしてワークブックメニューを開きます。
3.  `Share…`を選択します。
4.  `Run as service account`の隣にあるトグルをオンにします。

### 2-2-3 接続で使用されるロールを動的に割り当てる (Dynamically assign roles used by a connection)

割り当てられたユーザー属性の値に基づいて、特定のユーザーまたはユーザーチームが、それをサポートする新規または既存の接続で使用するロールを動的に割り当てることができます。

> 📘
> この機能は、すべてのデータプラットフォーム接続でサポートされているわけではありません。あなたの接続がサポートしているかを確認するには、「[サポートされているデータプラットフォームと機能の互換性](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

動的に割り当てられたロールを使用して、埋め込みユーザーのチームがセキュアに埋め込まれたコンテンツにアクセスするために使用すべきロールを割り当てるなど、さまざまなユースケースのユーザーアクセスを管理します。接続で複数のロールを使用することで、Sigmaで手動で行レベルのセキュリティやセキュリティポリシーを再作成する代わりに、データプラットフォームで定義された行レベルのセキュリティを活用できます。

> 📘
> このオプションは、キーペア認証でのみ使用できます。OAuthを使用してSigmaをデータプラットフォームに接続している場合、このオプションは使用できません。

接続で属性を構成した後、セキュアな埋め込みURLで外部の埋め込みユーザーに属性を割り当てることもできます。詳細は、「[埋め込みコンテンツのデータへのアクセスを制限する](https://help.sigmacomputing.com/docs/restrict-access-to-data-in-embedded-content)」を参照してください。

> 💡
> Snowflake接続の場合、`Warehouse`ユーザー属性を使用して仮想ウェアハウスを動的に割り当てることもできます。ウェアハウスを動的に割り当てることで、例えばSigmaをセキュアに埋め込む場合に、顧客ごとにコンピューティングコストを個別に管理できます。

#### **要件 (Requirements)**
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* また、この構成をサポートするために、データプラットフォームが設定されていることを確認する必要があります。
    * 各ロールは、接続に関連付けられたユーザーまたはユーザーアカウントに付与されている必要があります。
    * 各ロールには、関連するデータベースオブジェクトを使用するための権限が付与されている必要があります。
    * Snowflakeのウェアハウスを動的に割り当てる場合、特定のウェアハウスで使用されるSnowflakeロールには、そのウェアハウスに対する少なくとも`USAGE`権限が付与されている必要があります。

#### **ユーザー属性を構成する (Configure user attributes)**
接続でユーザー属性を設定するには、まず`Role`ユーザー属性を作成し、それを関連するユーザーおよびユーザーのチームに割り当てる必要があります。
1.  `Role`ユーザー属性を作成します。データプラットフォーム構成の適切なデフォルトロールに相当するデフォルト値を設定します。
2.  `Role`ユーザー属性をユーザーとチームに割り当てます。ユーザー属性の値を、各チームまたはユーザーがデータにアクセスする際に使用してほしいロール名に設定します。
> 💡
> `Warehouse`属性についても同じ手順が適用されます。

手順については、「[ユーザー属性を構成する](https://help.sigmacomputing.com/docs/user-attributes)」を参照してください。

#### **接続でユーザー属性を設定する (Set user attributes on a connection)**
ユーザーとチームにユーザー属性を作成して割り当てた後、新規または既存の接続でユーザー属性を使用するように構成します。
1.  お使いのデータプラットフォームの接続を作成する手順に従います。
    * Snowflake
    * PostgreSQL
    * AlloyDB
    * MySQL
2.  (Snowflakeのみ) `Connection Credentials`セクションの`Warehouse`フィールドで、`Set by user attribute`を選択して、以前に構成した`Warehouse`属性を参照して選択します。
3.  `Connection Credentials`セクションの`Role`フィールドで、`Set by user attribute`を選択して、以前に構成した`Role`属性を参照して選択します。
4.  接続の設定を完了します。接続を作成または保存すると、変更が有効になります。

#### **セキュアな埋め込みでの使用 (Use with secure embeds)**
「[埋め込みコンテンツのデータへのアクセスを制限する](https://help.sigmacomputing.com/docs/restrict-access-to-data-in-embedded-content)」を参照してください。

### 2-2-4. SSH経由で接続する (Connect through SSH)

Sigmaは、`PostgreSQL`、`Redshift`、`AlloyDB`、および`MySQL`接続に対して、Secure Shell (SSH) 経由での接続をサポートしています。

SSHプロトコルは、クライアントとサーバーが安全なチャネル上で通信する、セキュアなリモートシェルプロトコルです。これには3つのレイヤーがあります。
* **トランスポート層:** サーバーとクライアント間の通信を保護し、データの暗号化と復号化を監視し、接続の整合性を保護し、データをキャッシュし、データ圧縮を実行します。
* **認証層:** 各セッションの開始時にクライアント認証を実行します。
* **接続層:** 認証成功後に通信チャネルを管理します。

SSHチャネルは、公開鍵暗号を使用してクライアントを認証します。接続を確立した後、SSHは情報を暗号化してサーバーとクライアント間で安全に交換します。これにより、特定のネットワークインフラストラクチャに依存しないデータセキュリティが提供されます。

#### **要件 (Requirements)**
* あなたのSigma組織における管理者権限。「[account types](https://help.sigmacomputing.com/docs/account-type-and-license-overview)」を参照してください。
* PostgreSQL, Redshift, AlloyDB, または MySQLデータベース。

#### **SSHサーバーのパラメータ (SSH server parameters)**
SSH接続を有効にするには、以下のSigma情報をシステム管理者に送信してください。

| | |
| :--- | :--- |
| **公開鍵** | `ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCfBoABeXmQjlx+Sc8V3WWMMPQKtFUEeRhg64WrZ0Om922TpJum1967LzGkHP/RIdZa95S0m8WRbGOzl9TeSzUz3jz2/NOxfwzzv/UKGsytzrkWaUZICPK/HlHF7kYWAT6gxMP3MGALwepYWwtPBAk+R3tba+T7siZYjI0URY+uFg329CiRuilPZ3AtsPoXQqEH3sdTPfT6RUKytiVSwCZgwsnzp4LyE2lSGTKRvMm90S+k5rPeQ20N9A6LAtLrFjCpaOwEqPK7JFJqAamOcST7mI/lYsB7+f6BuH8I7Vq+1xdHFEQ1Uy1KelxLcwdJ5FAsjdGPWb1pKYZInXfd/CxnFMyr++PVYOz6xCAxpfWzCn6zCYUieqsjUPk5mYxz4+tc7ejuWUTHf/htiPfW2JwUObt8xo0y4xIJ8G4qzueovlz5BxWyA55OfjOOqNU7OsyRMvqkSQrfvWtfD3T8RrL82fOUewGFur3RJYD1/Nj9RX8cZDjDipxStarFO1ORBDWwSzNPHkn/xzNWc/IsSPKsN9ZATFkUIN1PXjCqqhVhIrLCFb63DLK9xjo3JdQ40oYjHN1YCKLF5E2f+kjz4jZZSjvN+uDDp2BjV5a75bQvZjXOB32gjNnjZdi6krZEh9z//3NKj55zwqynjn0JTq3/dgQFYItVP4F4/bJORBcUfQ== info@sigmacomputing.com` |
| **ユーザー** | `sigmacomputing` |
| **Sigma IPアドレス** | SigmaのアウトバウンドIPアドレスは、Sigma管理ポータルのすべての個々の接続ページにリストされています。 |

##### **SigmaのIPを取得する (Get Sigma IPs)**
アプリからSigmaのIPを取得するには、以下の手順に従います。
1.  管理ポータルを`Connection`ページで開きます。
2.  任意の接続を選択するか、`Create Connection`をクリックします。
3.  接続資格情報の下にあるIPアドレスを探します。

#### **SSH経由でSigmaに接続する (Connect to Sigma through SSH)**
1.  SigmaのSSH公開鍵をダウンロードまたは保存します。
2.  あなたの許可リストにSigmaのIPを追加します。
3.  SSHユーザーアカウントを作成し、`sigmacomputing`と名付けます。
    * ユーザー`sigmacomputing`は公開鍵を通じて認証されます。
4.  あなたのSSHサーバーの指示に従って、Sigmaの公開鍵を承認します。
5.  ほとんどのサーバーでは、SSHのデフォルトポートは22です。これはSigmaのデフォルトポートでもあります。
    あなたのSSHサーバーのポートがSigmaのポートと一致することを確認してください。
6.  Sigmaで、管理ポータル内の接続ページに移動します。
    a.  `Connection Credentials`の下で、`SSH Tunnel`をオンにします。
    これらのパラメータを設定します。
    * **Tunnel host:** これはあなたのIPアドレスです。
    * **Tunnel port:** この値はあなたのSSHサーバーのポートと一致する必要があります。
<img width="630" height="173" alt="9c7e113-connection-ssh" src="https://github.com/user-attachments/assets/11e25b89-a787-4c98-8e68-0d5988cf4205" />
7. 既存の接続を編集している場合は、`Save`をクリックします。
   新しい接続を作成している場合は、`Connection features`, `Write access`などの指定を続行します。

### 2-2-5-1. AWS PrivateLink接続 (AWS PrivateLink Connections)

Sigma組織がAmazon Web Services (AWS)で実行されている場合、AWS PrivateLinkを使用してデータに安全に接続できます。AWS PrivateLinkは、パブリックインターネット経由でトラフィックを送信することなく、AWS Virtual Private Cloud (VPC)間に接続を作成できるセキュリティ機能です。Sigmaは、PrivateLinkをサポートするすべてのAmazonリージョンで、AWS PrivateLinkを介してクラウドデータプラットフォームに接続できます。

PrivateLinkのセキュリティ上の利点と内部構造に関する詳細は、AWSドキュメントの「[AWS PrivateLink](https://aws.amazon.com/privatelink/)」を参照してください。

このドキュメントでは、SigmaからデータプラットフォームへのAWS PrivateLink接続を設定する方法について説明します。

#### **システムとユーザー要件 (System and user requirements)**
すべてのAWS PrivateLink接続には、以下が必要です。
* AWSで実行されているSigma組織。
    > ❗️
    > 注：プライベートリンクを使用するには、Sigma組織がデータプラットフォームと同じクラウド上にある必要があります。組織がAzureを使用している場合は、「[Azure Private Link connections](https://help.sigmacomputing.com/docs/azure-private-link-connections)」を参照してください。
* Sigmaで`Admin`アカウントタイプを割り当てられている必要があります。「[User account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* AWS VPCにデプロイされたSnowflake（セルフマネージドまたはVPS）、Redshift、MySQL、SQL Server 2022、Starburst、Postgresデータウェアハウス、または任意のAWSリージョンにあるカスタムプロキシサーバー。
    > 📘
    > この機能は、BigQueryウェアハウスや、Azure、GCP、VMwareクラウドで実行されているセルフマネージドウェアハウスをサポートしていません。

データプラットフォームと特定のPrivateLink構成方法によっては、追加の要件が適用される場合があり、以下の対応するセクションに記載されます。

#### **PrivateLinkでデータに接続する (Connecting to your data with PrivateLink)**
以下の手順は、既存のパブリック接続をPrivateLinkを使用するように更新する場合と、PrivateLinkを使用する新しい接続を作成する場合の両方をカバーしています。PrivateLinkを設定するプロセスは、組織が使用するデータプラットフォームによって異なります。
* Snowflake
* Redshift
* Databricks
* MySQL, SQL Server 2022, PostgreSQL, Starburst, およびカスタムプロキシサーバー (e.g. secuPi)

#### **Snowflake**
PrivateLinkを介したSnowflakeへの接続は、Snowflakeの構成に依存します。
* `Business Critical`（またはそれ以上）エディションのSnowflake顧客で、Virtual Private Server (VPS)またはプロキシサーバーを使用していない場合は、SnowflakeのPrivateLink統合を介して接続できる可能性があります。「[SnowflakeのPrivateLink統合で接続する](#connect-with-snowflakes-privatelink-integration)」を参照してください。
* Snowflake顧客で、Virtual Private Server (VPS)またはプロキシサーバーを使用している場合は、「[独自のVPCを介してSnowflakeに接続する](#connect-to-snowflake-via-your-own-vpc)」を参照してください。

##### **SnowflakeのPrivateLink統合で接続する (Connect with Snowflake’s PrivateLink Integration)**
SnowflakeのPrivateLink統合により、Sigmaはデータを収容しているSnowflake VPCに直接、PrivateLinkを介して安全な接続を作成できます。SigmaとあなたのSnowflakeウェアハウス間のトラフィックは、AWSバックボーン上のみを通過します。あなた自身のアマゾンアカウントやVPCは必要ありません - Snowflakeによって管理されるウェアハウスのみがAWS VPC内に存在する必要があります。

* **追加要件 (Additional requirements)**
    * SnowflakeはPrivateLinkサポートのために`Business Critical`エディション（またはそれ以上）を要求します。
    * あなたのSigmaアカウントエグゼクティブに連絡して、Sigma組織の適格性を確認してください。
    * SnowflakeアカウントがVPSを使用しているか、プロキシサーバーでSigmaをSnowflakeに接続している場合、SnowflakeのPrivateLink統合は使用できません。「[独自のVPCを介してSnowflakeに接続する](#connect-to-snowflake-via-your-own-vpc)」を参照してください。
    * Snowflakeアカウント管理者である必要があります（システムロールは`ACCOUNTADMIN`）。

* **SnowflakeのPrivateLink統合を使用して接続する (Connect using Snowflake's PrivateLink integration)**
    SnowflakeのPrivateLink統合で接続するには：
    1.  Snowflakeで、`SYSTEM$GET_PRIVATELINK_CONFIG`を呼び出します。以下の値を記録してください。
        * **privatelink-vpce-id:** これはVPCエンドポイントサービス名で、`com.amazonaws.vpce.<region>.vpce-svc-xxxxxxxxxx`のような形式です。
        * **privatelink-account-url:** これはSnowflake PrivateLinkアカウントURLで、`<privatelink-account-name>.<aws-region>.privatelink.snowflakecomputing.com`のような形式です。
    2.  Sigmaアカウントエグゼクティブまたはカスタマーアカウントマネージャーに連絡して、SigmaとのPrivateLink接続をインストールし、サービス名とURLを提供してください。インストールが完了すると、Sigmaから連絡があります。
    3.  PrivateLinkを使用するように接続を更新します。
        * **既存のSnowflakeへの接続の場合：**
            a. `Home` > `Administration` > `Connections`に移動します。
            b. 既存の接続を選択し、`Edit`を選択します。
            c. `Account`フィールドに、ステップ1で記録したPrivateLinkアカウントURLを、`<privatelink-account-name>.<aws-region>.privatelink`の形式で入力します。
            d. `Save`を選択します。
            > 📘
            > 既存の接続は引き続き機能しますが、このステップが完了するまでPrivateLinkは使用されません。
        * **新しいSnowflakeへの接続の場合：**
            「[Connect to Snowflake](https://help.sigmacomputing.com/docs/connect-to-snowflake)」の手順を使用して新しい接続を作成します。`Account`フィールドを入力する際、ステップ1で記録したPrivateLinkアカウントURLを、`<privatelink-account-name>.<aws-region>.privatelink`の形式で入力します。<img width="250" height="21" alt="74e4420e5fde0485e6293a59b1293a8d9486ecc49dee93c1c50b11e474f69cd2-accountfieldprivatelink" src="https://github.com/user-attachments/assets/d4a8e0d8-1a60-42cd-b771-8f6e386c20b3" />

##### **独自のVPCを介してSnowflakeに接続する (Connect to Snowflake via your own VPC)**

SnowflakeのPrivateLinkに接続するには：
1.  VPCエンドポイントサービスを作成します。エンドポイントサービスを作成するには、AWSドキュメントの「[Create a service powered by AWS PrivateLink](https://docs.aws.amazon.com/vpc/latest/privatelink/create-endpoint-service.html)」を参照してください。
2.  新しく作成したVPCエンドポイントサービスをSigmaに検出可能にします。エンドポイントを検出可能にするには、AWSドキュメントの「[Manage permissions](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-permissions.html)」を参照してください。
    * エンドポイントサービスを構成するには、SigmaのAmazon Resource Name (ARN)が必要です。VPCエンドポイントサービスの`Allow principals`構成に、以下のARNを入力してください：`arn:aws:iam::185497759670:role/cdktf-operator`
    > 📘
    > `arn:aws:iam::185497759670:role/root`構成を持つ既存の構成は、すべてのユーザーに対して引き続き機能しますが、`role/cdktf-operator`の使用が推奨されます。
3.  Sigmaアカウントエグゼクティブまたはカスタマーアカウントマネージャーに連絡して、PrivateLink接続をインストールします。彼らは以下を必要とします。
    * あなたのエンドポイントのVPCエンドポイントサービス名（`com.amazonaws.vpce.<region>.vpce-svc-xxxx`のような形式）。
    * あなたのロードバランサーのアベイラビリティゾーンID（`use1-az1`のような形式）。
    * アカウントURL（`<account-name>.<region>.privatelink.snowflakecomputing.com`のような形式）。
4.  インストールには数日かかる場合があります。インストールが完了すると、Sigmaから連絡があり、接続用のアカウントURL名が提供されます（後の構成で必要です）。
5.  インストール後、VPCエンドポイントサービスが新しい接続を手動で受け入れる必要がある場合は、Sigmaの新しいエンドポイント接続を受け入れる必要があります。AWSドキュメントの「[Accept or reject connection requests](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-endpoint-services.html#accept-reject-connection-requests)」を参照してください。
6.  PrivateLinkを使用するように接続を更新します。
    * **既存のデータプラットフォームへの接続の場合：**
        a. `Home` > `Administration` > `Connections`に移動します。
        b. 目的の接続を選択し、`Edit`を選択します。
        c. `Account`フィールドに、Sigmaから提供されたアカウントURL名を入力します。
        d. `Save`を選択します。
        > 📘
        > 既存のデータプラットフォームへの接続は引き続き機能しますが、このステップが完了するまでPrivateLinkは使用されません。
    * **新しいデータプラットフォームへの接続の場合：**
        「[Connect to data sources](https://help.sigmacomputing.com/docs/connect-to-data-sources)」の手順を使用してデータプラットフォームに接続します。`Account`フィールドを入力する際、Sigmaから提供された新しいアカウントURLを使用します。

#### **Redshift**
PrivateLinkを介したRedshiftへの接続は、Redshiftの構成に依存します。
* RedshiftクラスターがRA3インスタンスタイプで、クラスターの再配置がオンになっている場合、SigmaはRedshift管理のVPCエンドポイントを介して接続することを推奨します。「[Redshift管理のVPCエンドポイントで接続する](#connect-with-redshift-managed-vpc-endpoints)」を参照してください。
* RedshiftクラスターがRA3インスタンスタイプでない場合、クラスターの再配置がオフになっている場合、またはRedshift管理のエンドポイントを使用したくない場合は、「[独自のVPCを介してRedshiftに接続する](https://help.sigmacomputing.com/docs/aws-privatelink-connections#connect-to-redshift-via-your-own-vpc)」を参照してください。

##### **Redshift管理のVPCエンドポイントで接続する (Connect with Redshift managed VPC endpoints)**
Redshift管理のVPCエンドポイントを使用すると、追加のインフラストラクチャを作成することなく、クラスターに追加のセキュリティを追加できます。詳細は、AWSドキュメントの「[Redshift managed VPC endpoints](https://docs.aws.amazon.com/redshift/latest/mgmt/managing-redshift-managed-vpc-endpoints.html)」を参照してください。

* **追加要件 (Additional requirements)**
    * 既存のRedshiftインスタンスを持っていること。
    * アクセスするクラスターはRA3インスタンスタイプである必要があります。
    * アクセスするクラスターは、クラスターの再配置がオンになっている必要があります。AWSドキュメントの「[Relocating a cluster](https://docs.aws.amazon.com/redshift/latest/mgmt/managing-cluster-recovery.html#relocating-a-cluster)」を参照してください。

* **Redshift管理のVPCエンドポイントでPrivateLinkを設定する (Set up PrivateLink on Redshift managed VPC endpoints)**
    Redshift管理のVPCエンドポイントを設定するには：
    1.  SigmaにRedshiftインスタンスへのアクセスを承認します。AWSドキュメントの「[Granting access to a VPC](https://docs.aws.amazon.com/redshift/latest/mgmt/managing-redshift-managed-vpc-endpoints.html#managed-vpc-endpoint-access-method-console)」を参照してください。アクセスを許可するAWSアカウントIDは`185497759670`です。Redshiftクラスターの場所に応じて、以下のVPC IDへのアクセスを許可してください。

| | |
| :--- | :--- |
| us-east-1 | vpc-03e998398a2b8d7d4 |
| us-east-2 | vpc-0eb5c451f6d93b9b0 |
| us-west-1 | vpc-0b98df9ea218bbae3 |
| us-west-2 | vpc-0ebc060057f91792c |
| ap-southeast-2 | vpc-0173a781cad403b87 |
| ap-northeast-1 | vpc-01d69d4176bf329d4 |
| eu-central-1 | vpc-03967ee832f14c234 |
| eu-west-1 | vpc-0ef690315d8c934e9 |
| eu-west-2 | vpc-0d89ee0ccf9f3eeb7 |

    もしあなたのRedshiftクラスターのリージョンが上記にリストされていない場合は、Sigmaサポートに支援を求めてください。

    2.  Sigmaに以下の情報を提供してください。
        * Redshiftクラスター識別子
        * RedshiftクラスターのAWSリージョン
        * AWSアカウント番号
        * アベイラビリティゾーンID：`use1-az1`のような形式。AWSドキュメントの「[Availability Zone IDs for your AWS resources](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/#Availability_Zone_IDs)」を参照してください。
        * [任意] 希望のDNS名：プライベートリンクアカウントURLの希望するサブドメイン名。名前は記述的で識別しやすいものであるべきです。例えば、`<name>-<env>-<region>-<index_number>`のような形式にしたいかもしれません。

    3. プライベートリンクが作成されると、Sigmaから連絡があります。

##### **独自のVPCを介してRedshiftに接続する (Connect to Redshift via your own VPC)**

1.  VPCエンドポイントサービスを作成します。エンドポイントサービスを作成するには、AWSドキュメントの「[Create a service powered by AWS PrivateLink](https://docs.aws.amazon.com/vpc/latest/privatelink/create-endpoint-service.html)」を参照してください。
2.  新しく作成したVPCエンドポイントサービスをSigmaに検出可能にします。エンドポイントを検出可能にするには、AWSドキュメントの「[Manage permissions](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-permissions.html)」を参照してください。
    * エンドポイントサービスを構成するには、SigmaのAmazon Resource Name (ARN)が必要です。VPCエンドポイントサービスの`Allow principals`構成に、以下のARNを入力してください：`arn:aws:iam::185497759670:role/cdktf-operator`
    > 📘
    > `arn:aws:iam::185497759670:role/root`構成を持つ既存の構成は、すべてのユーザーに対して引き続き機能しますが、`role/cdktf-operator`の使用が推奨されます。
3.  Sigmaアカウントエグゼクティブ、カスタマーアカウントマネージャー、またはSigmaサポートに連絡して、PrivateLink接続をインストールします。彼らは以下を必要とします。
    * あなたのエンドポイントのVPCエンドポイントサービス名（`com.amazonaws.vpce.<region>.vpce-svc-xxxx`のような形式）。
    * あなたのロードバランサーのアベイラビリティゾーンID（`use1-az1`のような形式）。
    * [任意] 希望のDNS名：プライベートリンクアカウントURLの希望するサブドメイン名。名前は記述的で識別しやすいものであるべきです。例えば、`<cdw_name>-<env>-<region>-<index_number>`のような形式にしたいかもしれません。この値を提供しない場合、Sigmaサポートがそれを選択し、あなたに提供します。
4.  インストールには数日かかる場合があります。インストールが完了すると、Sigmaから連絡があり、接続用のアカウントURL名が提供されます（後の構成で必要です）。
5.  インストール後、VPCエンドポイントサービスが新しい接続を手動で受け入れる必要がある場合は、Sigmaの新しいエンドポイント接続を受け入れる必要があります。AWSドキュメントの「[Accept or reject connection requests](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-endpoint-services.html#accept-reject-connection-requests)」を参照してください。
6.  PrivateLinkを使用するように接続を更新します。
    * **既存のデータプラットフォームへの接続の場合：**
        a. `Home` > `Administration` > `Connections`に移動します。
        b. 目的の接続を選択し、`Edit`を選択します。
        c. `Host`フィールドに、ステップ3のDNS名の後に`.privatelink.sigma.internal`を付けたものを入力します。例えば、`<cdw_name>-<env>-<region>-<index_number>.privatelink.sigma.internal`。
        d. `Save`を選択します。
        > 📘
        > 既存のデータプラットフォームへの接続は引き続き機能しますが、このステップが完了するまでPrivateLinkは使用されません。
    * **新しいデータプラットフォームへの接続の場合：**
        「[Connect to data sources](https://help.sigmac.com/docs/connect-to-data-sources)」の手順を使用してデータプラットフォームに接続します。`Host`フィールドを入力する際、ステップ3のDNS名の後に`.privatelink.sigma.internal`を付けたものを入力します。例えば、`<cdw_name>-<env>-<region>-<index_number>.privatelink.sigma.internal`。

#### **Databricks**

##### **追加要件 (Additional requirements)**
* Databricksプラットフォームは`Enterprise`ティアである必要があります。
* Databricksワークスペースは`us-west-1`リージョンにあってはなりません。
* Databricksワークスペースは、顧客管理である必要があります（Databricks管理ではない）。
    * Databricksワークスペースにアクセスしたときに`Network`サムネイルが表示されない場合、ワークスペースはDatabricks管理です。
    * Databricksワークスペースにアクセスしたときに`Network`サムネイルが表示される場合、それは顧客管理です。

##### **PrivateLinkでDatabricksに接続する (Connect to Databricks with PrivateLink)**
PrivateLinkでDatabricksに接続するには：
1.  AWSアカウントに2つのVPCエンドポイントを作成します。AWSドキュメントの「[Create a VPC endpoint](https://docs.aws.amazon.com/vpc/latest/userguide/vpce-interface.html#create-interface-endpoint)」を参照してください。リージョンでVPCエンドポイントを作成するために必要なエンドポイントサービス名については、Databricksドキュメントの「[PrivateLink VPC endpoint services](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/privatelink.html#step-2-create-aws-vpc-endpoints)」を参照してください。作成する必要があるのは：
    * 1つの`Workspace (including REST API)` VPCエンドポイント
    * 1つの`Secure cluster connectivity relay` VPCエンドポイント
2.  Databricksで、作成した2つのVPCエンドポイントを登録する必要があります。これにより、ネットワーク構成で使用できるようになります。Databricksドキュメントの「[Manage VPC endpoint registrations](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/privatelink.html#manage-vpc-endpoint-registrations)」を参照してください。
3.  Databricksで、リージョン用のSigma VPCエンドポイントを登録する必要があります。Databricksドキュメントの「[Manage VPC endpoint registrations](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/privatelink.html#manage-vpc-endpoint-registrations)」を参照してください。
    SigmaのVPCエンドポイントは以下の表にリストされています。もしあなたのリージョンがリストされていない場合は、Sigmaアカウントエグゼクティブまたはカスタマーアカウントマネージャーに連絡してください。

| Region | WORKSPACE_ACCESS Endpoint |
| :--- | :--- |
| us-east-2 | vpce-01e5bcfb542cc064b |
| us-east-1 | vpce-01e5ee810ad38e87a |
| us-west-2 | vpce-0f7f1c9eb781e5ee0 |
| ap-southeast-2 | vpce-0ea8cc8aaac99003c |
| eu-central-1 | vpce-042d25a7829e28994 |
| eu-west-1 | vpce-089a8efa3ea799d03 |
| eu-west-2 | vpce-0e2cc626d12fd41a5 |
| ap-northeast-1 | vpce-05a3ec6e4605fdd94 |

4.  Databricksで、PrivateLink接続を許可するためのプライベートアクセス設定オブジェクトを作成します。Databricksドキュメントの「[Create a private access settings object](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/privatelink.html#step-4-create-a-private-access-settings-object)」を参照してください。以下の構成が設定されていることを確認してください。
    * Public access enabled: `False`
    * Private access level: `Account`
5.  Databricksで、新しいネットワーク構成を作成します。Databricksドキュメントの「[Create a network configuration](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/customer-managed-vpc.html#step-3-create-a-network-configuration-using-the-account-console)」を参照してください。以下の構成が使用されていることを確認してください。
    * 目的のDatabricksワークスペースの`VPC`, `Subnet IDs`, `Security Group IDs`を使用します。
    * `VPC endpoint for secure cluster connectivity relay`および`VPC endpoint for REST APIs`フィールドには、AWSアカウントで作成したAWSエンドポイントを使用します。
6.  新しいネットワーク構成とプライベートアクセス設定を含むようにDatabricksワークスペースを更新します。Databricksドキュメントの「[Advanced configurations](https://docs.databricks.com/en/administration-guide/cloud-configurations/aws/customer-managed-vpc.html#advanced-configurations)」を参照してください。
7.  Sigmaアカウントエグゼクティブまたはカスタマーアカウントマネージャーに連絡して、PrivateLink接続をインストールします。彼らはあなたのDatabricksワークスペースに関する以下の情報を必要とします。
    * Deployment name
    * Workspace region
8.  インストールには数日かかる場合があります。インストールが完了すると、Sigmaから連絡があり、接続用のホストURLが提供されます。
9.  PrivateLinkを使用するように接続を更新します。
    * **既存のデータプラットフォームへの接続の場合：**
        a. `Home` > `Administration` > `Connections`に移動します。
        b. 目的の接続を選択し、`Edit`を選択します。
        c. `Host`フィールドに、ステップ7でSigmaから提供されたホストURLを入力します。
        d. `Save`を選択します。
        > 📘
        > 既存のデータプラットフォームへの接続は引き続き機能しますが、このステップが完了するまでPrivateLinkは使用されません。
    * **新しいデータプラットフォームへの接続の場合：**
        「[Connect to data sources](https://help.sigmacomputing.com/docs/connect-to-data-sources)」の手順を使用してデータプラットフォームに接続します。`Host`フィールドを入力する際、ステップ7でSigmaから提供されたホストURLを使用します。

#### **MySQL, SQL Server 2022, PostgreSQL, Starburst, またはカスタムプロキシサーバー**

MySQL, SQL Server 2022, Starburst, PostgreSQL, またはカスタムプロキシサーバー（例：secuPi）を使用する組織の場合、AWS PrivateLinkで接続するには以下の手順を使用します。

1.  VPCエンドポイントサービスを作成します。エンドポイントサービスを作成するには、AWSドキュメントの「[Create a service powered by AWS PrivateLink](https://docs.aws.amazon.com/vpc/latest/privatelink/create-endpoint-service.html)」を参照してください。
2.  新しく作成したVPCエンドポイントサービスをSigmaに検出可能にします。エンドポイントを検出可能にするには、AWSドキュメントの「[Manage permissions](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-permissions.html)」を参照してください。
    * エンドポイントサービスを構成するには、SigmaのAmazon Resource Name (ARN)が必要です。VPCエンドポイントサービスの`Allow principals`構成に、以下のARNを入力してください：`arn:aws:iam::185497759670:role/cdtraf-operator`
    > 📘
    > `arn:aws:iam::185497759670:role/root`構成を持つ既存の構成は、すべてのユーザーに対して引き続き機能しますが、`role/cdktf-operator`の使用が推奨されます。
3.  Sigmaアカウントエグゼクティブ、カスタマーアカウントマネージャー、またはSigmaサポートに連絡して、PrivateLink接続をインストールします。彼らは以下を必要とします。
    * あなたのエンドポイントのVPCエンドポイントサービス名（`com.amazonaws.vpce.<region>.vpce-svc-xxxx`のような形式）。
    * あなたのロードバランサーのアベイラビリティゾーンID（`use1-az1`のような形式）。
    * [任意] 希望のDNS名：プライベートリンクアカウントURLの希望するサブドメイン名。名前は記述的で識別しやすいものであるべきです。例えば、`<cdw_name>-<env>-<region>-<index_number>`のような形式にしたいかもしれません。この値を提供しない場合、Sigmaサポートがそれを選択し、あなたに提供します。
4.  インストールには数日かかる場合があります。インストールが完了すると、Sigmaから連絡があり、接続用のアカウントURL名が提供されます（後の構成で必要です）。
5.  インストール後、VPCエンドポイントサービスが新しい接続を手動で受け入れる必要がある場合は、Sigmaの新しいエンドポイント接続を受け入れる必要があります。AWSドキュメントの「[Accept or reject connection requests](https://docs.aws.amazon.com/vpc/latest/privatelink/manage-endpoint-services.html#accept-reject-connection-requests)」を参照してください。
6.  PrivateLinkを使用するように接続を更新します。
    * **既存のデータプラットフォームへの接続の場合：**
        a. `Home` > `Administration` > `Connections`に移動します。
        b. 目的の接続を選択し、`Edit`を選択します。
        c. `Host`フィールドに、ステップ3のDNS名の後に`.privatelink.sigma.internal`を付けたものを入力します。例えば、`<cdw_name>-<env>-<region>-<index_number>.privatelink.sigma.internal`。
        d. `Save`を選択します。
        > 📘
        > 既存のデータプラットフォームへの接続は引き続き機能しますが、このステップが完了するまでPrivateLinkは使用されません。
    * **新しいデータプラットフォームへの接続の場合：**
        「[Connect to data sources](https://help.sigmacomputing.com/docs/connect-to-data-sources)」の手順を使用してデータプラットフォームに接続します。`Host`フィールドを入力する際、ステップ3のDNS名の後に`.privatelink.sigma.internal`を付けたものを入力します。例えば、`<cdw_name>-<env>-<region>-<index_number>.privatelink.sigma.internal`。

### 2-2-5. Azure Private Link接続 (Azure Private Link Connections)

このドキュメントでは、AzureのPrivate Linkを使用して、AzureでホストされているデータウェアハウスにSigmaを接続する方法について説明します。

> 📘
> SigmaのAzure Private Linkラボに関する詳細は、「[Azure Private Link lab](https://www.sigmacomputing.com/hands-on-lab/azure-private-link)」を参照してください。

#### **要件 (Requirements)**
* Azureで実行されているSigma組織。
* Sigma組織における管理者権限。「[User account types](https://help.sigmacomputing.com/docs/user-account-types)」を参照してください。
* データウェアハウスに応じて、Snowflake, Databricks, PostgreSQLまたはMySQLの管理者。
* Azureでの管理者であること。
* Snowflakeの内部ステージにアクセスするためにAzure Private Linkを作成したい場合は、Sigmaアカウントエグゼクティブに連絡してください。

#### **概要 (Introduction)**
Azureで実行されているSigma組織は、AzureのPrivate Linkを使用してデータに安全に接続できます。これにより、Sigmaは仮想ネットワーク内のプライベートエンドポイントを介してAzureでホストされているデータウェアハウスにアクセスできます。これにより、データ転送中のセキュリティが向上するだけでなく、ネットワーク遅延を削減することでパフォーマンスも向上します。Private Linkを使用すると、SigmaはプライベートIPアドレスを使用してデータウェアハウスに接続するため、トラフィックがMicrosoftネットワークを離れることはなく、データはインターネットに公開されることなく安全に保たれます。

Private Linkを利用するには、仮想ネットワークにプライベートエンドポイントを作成し、それをデータウェアハウスにマッピングし、プライベートIPアドレスを割り当て、このアドレスを使用してウェアハウスに接続します。

Sigmaは、Azure上の以下のデータウェアハウスへの接続をサポートしています。
* Snowflake
* Databricks
* PostgreSQL
* MySQL
* Azure SQL Database, Azure SQL Managed Instance, or SQL Server 2022

#### **データウェアハウス用のPrivate Link接続を作成する (Create Private Link Connection for Your Data Warehouse)**
以下の手順に従って、AzureでホストされているデータウェアハウスへのPrivate Link接続を作成します。
> 📘
> このプロセスを開始するために、すべてのデータウェアハウスの最初のステップは、必要な情報を取得してアカウントマネージャーに送信することです。

#### **Snowflake**

##### **Snowflakeの情報をSigmaに提供する (Provide Snowflake Info to Sigma)**
以下の手順に従って、組織用のPrivate Linkを作成するために必要な情報をSigmaに提供します。
> 📘
> Private Linkを使用するには、SnowflakeアカウントがBusiness Critical Editionである必要があります。

1.  Snowflake SQLコンソールで、以下のコマンドを実行します。
    ```sql
    select system$get_privatelink_config();
    ```
<img width="1463" height="843" alt="9e7f78e-1" src="https://github.com/user-attachments/assets/5feee0c2-1473-4f43-950c-24949e5d02e7" />

2.  以下はSQLクエリからの出力です。
    ```json
    {"regionless-snowsight-privatelink-url":"app-br67048-sigma_azure_us_east_2.privatelink.snowflakecomputing.com","privatelink-account-name":"os99982.east-us-   privatelink","snowsight-privatelink-url":"app.east-us-2.privatelink.snowflakecomputing.com","privatelink-account-url":"os99982.east-us-privatelink.snowflakecomputing.com","privatelink-pls-id":"sf-pvlinksvc-azeastus2.cf82bce2-bw2d-4dw2-92ee-3dw2fb04d191.eastus2.azure.privatelinkservice","regionless-privatelink-account-url":"br67048-sigma_azure_us_east_2.snowflakecomputing.com","privatelink_ocsp-url":"ocsp.os99982.east-us-privatelink.snowflakecomputing.com","privatelink-connection-urls":"[]"}
    ```
3.  出力フィールドで、`privatelink-pls-id`と`privatelink-account-url`の値をコピーします。
    * 上記の例では、`privatelink-pls-id`は
      `sf-pvlinksvc-azeastus2.cf82bce2-bw2d-4dw2-92ee-3dw2fb04d191.eastus2.azure.privatelinkservice`
    * `privatelink-account-url`は
      `os99982.east-us-2.privatelink.snowflakecomputing.com`
      です。 これら2つの値をSigmaのアカウントマネージャーに送信します。
4.  SigmaがPrivate Linkを作成し、リンクがアクティブになったら通知します。
    > 📘
    > SigmaがPrivate Linkを作成するまで、接続を構成することはできません。

##### **Snowflake接続を構成する (Configure Snowflake Connection)**
以下の手順に従って、Private Linkを使用するようにSigmaのSnowflake接続を構成します。

1.  プライベートリンクがアクティブになった後、Sigmaで、**Admin > Connections > Snowflake**に移動します。
2.  `Create`をクリックしてSnowflake接続を作成します。
3.  `Account`フィールドに、アカウントURLの3つの部分を次の形式で入力します：`<account>.<region_id>.privatelink`
    * 例えば、アカウントURLが `test123.west-us-2.privatelink.snowflakecomputing.com` の場合、`Account`フィールドは `test123.west-us-2.privatelink` となります。
4.  `Warehouse`の下に、Snowflakeにリストされているウェアハウス名を入力します。
5.  組織でOAuthが有効になっており、接続でそれを使用したい場合は、OAuthアクセスをオンにします。「[OAuthでSnowflakeに接続する](https://help.sigmacomputing.com/docs/connect-to-snowflake#connect-to-snowflake-with-oauth)」を参照してください。
  　注意：サービスアカウントなしでOAuthを使用することを選択した場合、ステップ9〜11は適用されません。
6.  `User`の下に、Snowflakeのユーザー名を入力します。
7.  `Password`の下に、Snowflakeのパスワードを入力します。
8.  [任意] `Role`には、この接続で使用するSnowflakeロールを指定できます。<img width="658" height="457" alt="fd91793-2" src="https://github.com/user-attachments/assets/3a232a57-75f9-493f-b7c0-b658af178f9f" />
9. [任意] `Connection Features`には、接続タイムアウトを設定したり、書き込みアクセスを有効にしたりできます。
10. フォームへの入力を完了したら、`Create`をクリックします。

#### **Databricks**

##### **前提条件 (Prerequisites)**
* Azure Databricksワークスペースを作成する必要があります。
* DatabricksワークスペースはPremiumティアである必要があります。
* Private Linkをサポートするには、カスタマイズされたネットワーク構成が必要です。

##### **DatabricksのリソースIDをSigmaに提供する (Provide Databricks Resource ID to Sigma)**
以下の手順に従って、組織用のプライベートリンクを作成するために必要なリソースIDをSigmaに提供します。

1.  Azure Servicesで、**Azure Databricks**にカーソルを合わせ、**Create**をクリックします。<img width="259" height="88" alt="cd565f2-4" src="https://github.com/user-attachments/assets/8387e996-dc82-4555-9b6c-2021f47ab49d" />

2.  Azureのdatabricksワークスペースページの右上隅にある**JSON View**をクリックします。
3.  **Networking**タブで、**Deploy Azure Databricks workspace in your own Virtual Network**に**Yes**をチェックし、事前に構成された仮想ネットワークと、パブリックおよびプライベートサブネットフィールド用の仮想ネットワークCIDR範囲内の2つのサブネットを入力する必要があります。
4.  以下の値をコピーして、アカウントエグゼクティブに送信してください。
    * Resource ID
    * DatabricksウェアハウスのRegion Name（Locationの下）
    * DatabricksサービスのURL、`adb-<workspace-id>.<random-number>.azuredatabricks.net`の形式。
<img width="1118" height="662" alt="26fdb87-5" src="https://github.com/user-attachments/assets/b1feb2ec-0c9a-44b8-8128-3d978ee04829" />

##### **プライベートリンクの承認 (Private Link Approval)**
Sigmaから通知があった後、以下の手順に従ってプライベートリンクを承認します。

1.  Azureポータルで、**Azure Databricks**に移動します。
2.  選択したAzure Databricksワークスペースをクリックします。
3.  左側のパネルで**Networking**をクリックします。
4.  **Private endpoint connections**をクリックします。
5.  新しく作成されたプライベートエンドポイントを選択します。ステータスは`Pending`になります。エンドポイントを承認するには、**Approve**をチェックします。Sigmaを構成する際に必要になるため、プライベートエンドポイントの名前をコピーしてください。<img width="1722" height="380" alt="bb7b579-6" src="https://github.com/user-attachments/assets/6e2306b4-9568-42e9-be22-5ed6377cbb68" />

##### **Databricks接続を構成する (Configure Databricks Connection)**
1.  AzureのDatabricksセクションで、ウェアハウスインスタンス > **Databricks Workspace**をクリックします。
2.  **Launch Workspace**をクリックします。<img width="698" height="294" alt="870df05-7" src="https://github.com/user-attachments/assets/53cb6c90-1347-455c-80dd-5298802c23e1" />
3.  Databricksで、**Data Science & Engineering**ドロップダウンから**SQL**を選択します。<img width="277" height="151" alt="200f8d7-8" src="https://github.com/user-attachments/assets/3d2b1e37-4ebe-4a76-a452-2215513dc3a1" />
4.  **Review SQL Warehouses**をクリックします。<img width="220" height="165" alt="0138e83-9" src="https://github.com/user-attachments/assets/d7f49630-c51e-41b1-92a6-527b7d082b5f" />

5.  ウェアハウスを選択します。
6.  **Connection details**タブをクリックします。
7.  Sigma UIで必要になるため、Databricksの**HTTP path**の値をコピーします。<img width="464" height="385" alt="7d4fc7c-10" src="https://github.com/user-attachments/assets/171b3e19-9d6d-41d8-90b1-1874a99083b1" />

8.  Databricksでユーザー名をクリックして**User Settings**に移動します。<img width="127" height="145" alt="c69849a-11" src="https://github.com/user-attachments/assets/a821f92e-fcf8-4781-a53d-6ce07b363aa6" />

9.  **Personal access tokens**タブをクリックします。
10. **Generate new token**をクリックします。
11. **Lifetime**フィールドで、プライベートリンクの期間を設定します。リンクはこの値に基づいて期限切れになります。
12. **Comment**フィールドに値を入力します。<img width="554" height="233" alt="6cf7600-12" src="https://github.com/user-attachments/assets/fc29c138-12c7-436f-87ef-a9523b708353" />

13. **Generate**をクリックします。Sigma UIで必要になるため、このトークンをコピーします。
14. Sigmaで、**Admin > Connections > Databricks**に移動します。
15. **Host**フィールドに、エンドポイントを承認したときにコピーしたプライベートエンドポイントを、以下の形式で入力します。
    `<private_endpoint_name>.privatelink.azuredatabricks.net`
    例えば、プライベートエンドポイント名が`databricks-endpoint`の場合、`Host`フィールドには次のように入力します。
    `databrick-endpoint.privatelink.azuredatabricks.net`
    > 📘
    > プライベートエンドポイントの名前を見つけるには、Azureポータル > **Azure Databricks Workspace > Networking**（左パネル）に移動します。プライベートエンドポイント名は、`Private endpoint connections`の`Private Endpoint`列に表示されます。
16. Azureからコピーした**HTTP path**の値を、Sigmaの**HTTP path**フィールドに貼り付けます。
17. Azureで作成したトークンをコピーし、Sigmaの**Access token**フィールドに入力します。<img width="644" height="236" alt="e8b6e0c-14" src="https://github.com/user-attachments/assets/6bc1ed72-2bbc-40a7-a7f2-16ceaa593720" />

18. [任意] **Connection Features**の下で、接続タイムアウトを設定したり、書き込みアクセスを有効にしたりできます。
19. [任意] **Connection queue size**フィールドで、Sigmaがこの接続で同時に実行できるインタラクティブクエリの数を定義します。
20. Sigmaで**Create**をクリックします。<img width="703" height="518" alt="a8d5ed4-15" src="https://github.com/user-attachments/assets/b4707bd8-93cd-442b-a92a-10ee45bc9482" />

#### **PostgreSQL**

Private Linkは、パブリックアクセスで作成されたAzure Database for PostgreSQLフレキシブルサーバーインスタンス、またはシングルサーバーインスタンスに対して有効にできます。

##### **前提条件 (Prerequisites)**
Private Link接続を追加するには、以下の手順を完了する必要があります。
* [PostgreSQLのリソースIDをSigmaに提供する](#provide-your-postgresql-resource-id-to-sigma)
* [Azureでプライベートリンクを承認する](#approve-the-private-link-in-azure)
* [SigmaでPostgreSQL接続を構成する](#configure-the-postgresql-connection-in-sigma)

##### **PostgreSQLのリソースIDをSigmaに提供する (Provide your PostgreSQL Resource ID to Sigma)**
Sigmaは、あなたの組織用のPrivate Linkを作成するために、あなたの`Resource ID`を必要とします。Azureドキュメントの「[How to get your Azure Resource ID](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resources-portal#get-resource-id)」を参照してください。サーバーページの`JSON View`から`Resource ID`をコピーし、PostgreSQLウェアハウスの`Region Name`も同様にコピーしてください。これらをSigmaのアカウントエグゼクティブに送信します。

##### **Azureでプライベートリンクを承認する (Approve the Private Link in Azure)**
SigmaがPrivate Linkの構成を完了した後、Azureドキュメントの「[Approve private endpoint connections](https://learn.microsoft.com/en-us/azure/private-link/private-endpoint-overview#approve-a-private-endpoint-connection)」を参照してプライベートエンドポイント接続を承認する方法を確認してください。プライベートエンドポイントのステータスが`Pending`から`Accepted`に変更されていることを確認してください。

##### **SigmaでPostgreSQL接続を構成する (Configure the PostgreSQL connection in Sigma)**
Sigmaで新しいPrivate Link PostgreSQL接続を構成します。
1.  **Administration > Connections**に移動します。
2.  `Create Connection`を選択し、次に`PostgreSQL`を選択します。接続に`Name`を入力します。
3.  `Connection Credentials`の下にあるフィールドを入力します。

| フィールド | 説明 |
| :--- | :--- |
| **Host** | Sigmaのアカウントエグゼクティブから提供されたDNS名を入力します。|
| **User** | Azure PostgreSQLサーバーページにある`Admin Username`を入力します。|
| **Port** | PostgreSQLのポート番号を入力します。|
| **Password** | データウェアハウスにアクセスするために作成したパスワードを入力します。|
| **Database** | データベースの名前を入力します。|

4.  接続のTLS暗号化を有効にするには、`Enable TLS`トグルをオンにします。

#### **MySQL**

##### **前提条件 (Prerequisites)**
* Private Linkは、パブリックアクセスで作成されたAzure Database for MySQLフレキシブルサーバーインスタンスに対してのみ有効にできます。
* Private Link接続を追加するには、以下の手順を完了する必要があります。
    * [MySQLのリソースIDをSigmaに提供する](#provide-your-mysql-resource-id-to-sigma)
    * [Azureでプライベートリンクを承認する](#approve-the-private-link-in-azure-mysql)
    * [SigmaでMySQL接続を構成する](#configure-the-mysql-connection-in-sigma)

##### **MySQLのリソースIDをSigmaに提供する (Provide your MySQL Resource ID to Sigma)**
Sigmaは、あなたの組織用のPrivate Linkを作成するために、あなたの`Resource ID`を必要とします。Azureドキュメントの「[How to get your Azure Resource ID](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resources-portal#get-resource-id)」を参照してください。サーバーページの`JSON View`から`Resource ID`をコピーし、MySQLウェアハウスの`Region Name`も同様にコピーしてください。これらをSigmaのアカウントエグゼクティブに送信します。

##### **Azureでプライベートリンクを承認する (Approve the Private Link in Azure)**
SigmaがPrivate Linkの構成を完了したら、Azureドキュメントの「[Approve private endpoint connections](https://learn.microsoft.com/en-us/azure/private-link/private-endpoint-overview#approve-a-private-endpoint-connection)」を参照してプライベートエンドポイント接続を承認する方法を確認してください。プライベートエンドポイントのステータスが`Pending`から`Accepted`に変更されていることを確認してください。

##### **SigmaでMySQL接続を構成する (Configure the MySQL connection in Sigma)**
Sigmaで新しいPrivate Link MySQL接続を構成します。
1.  **Administration > Connections**に移動します。
2.  `Create Connection`を選択し、次に`MySQL`を選択します。接続に`Name`を入力します。
3.  `Connection Credentials`の下にあるフィールドを入力します。

| フィールド | 説明 |
| :--- | :--- |
| **Host** | Sigmaのアカウントエグゼクティブから提供されたDNS名を入力します。|
| **User** | MySQLサーバーページにある`Admin Username`を入力します。|
| **Port** | MySQLのポート番号を入力します。|
| **Password** | データウェアハウスにアクセスするために作成したパスワードを入力します。|
| **Database** | データベースの名前を入力します。|

4.  接続のTLS暗号化を有効にするには、`Enable TLS`トグルをオンにします。
---
#### **Azure SQL Database, Azure SQL Managed Instance, or SQL Server 2022**
Azure SQL Database, Azure SQL Managed Instance, または SQL Server 2022接続用のPrivate Linkの設定に関する詳細については、Sigmaのアカウントエグゼクティブにお問い合わせください。

### 2-2-6. 接続のトラブルシューティング (Troubleshoot your connection)

テーブルが見つからない、接続できないなどの接続に関する問題をトラブルシューティングする必要がある場合は、このページのガイダンスに従ってください。

#### **SigmaのIPを許可リストに追加する (Add Sigma IPs to the allowlist)**
場合によっては、データに正常に接続するために、SigmaのIPアドレスを許可リストに追加する必要があります。これは、ファイアウォール、セキュリティグループ、またはその他のIPベースのセキュリティポリシーによってウェアハウスが外部接続に対して閉じられている場合に、必要なステップです。

Sigmaは、すべての個々の`Connection`ページにアウトバウンドIPアドレスをリストしています。それらを表示するには、以下の手順に従います。
1.  **Administration > Connections**ページを開きます。
2.  関連する接続を選択します。
3.  データソースへの接続がない場合は、`Create Connection`をクリックします。
4.  `Connection Credentials`セクションで、`Host`フィールドの下にリストされているIPを確認します。
> 📘
> 接続概要にリストされているIPアドレスは、Private Link経由の接続には適用されません。Private Link接続用のIPアドレスが必要な場合は、Sigmaサポートにお問い合わせください。

個々のデータプラットフォームに特有のガイダンスについては：
* **PostgreSQL:** Sigmaは、ネットワークレベルまたはクライアント認証のいずれかで認証される必要があります。
* **Redshift:** 「[Amazon Redshift cluster security groups](https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-security-groups.html)」を参照してください。
* **Snowflake:** 「[Network Policies](https://docs.snowflake.com/en/user-guide/network-policies)」を参照してください。

#### **Snowflakeユーザーロールの権限 (Permissions for the Snowflake user role)**
Sigmaは、接続で指定されたSnowflakeユーザーロールを使用します。Snowflakeでそのロールに正しい権限が付与されていない限り、Sigmaでデータを表示することはできません。

接続が`OAuth`を使用している場合、接続は組織の各メンバーの権限をSnowflakeから直接継承します。個々のユーザーまたはサービスアカウントユーザーの権限をトラブルシューティングするには、以下を確認してください。
* ユーザーに付与されたプライマリロールが、Snowflakeで関連するアクセスを提供していること。
* ユーザーが、OAuthプロバイダーを通じて意図したロールを継承していること。

#### **データを同期する (Sync your data)**
Sigmaは、接続のメタデータを自動的（かつ定期的）に同期します。
クラウドデータウェアハウスでテーブルのスキーマを更新するなど、変更を加えた場合は、これらの変更がSigmaに反映されるように手動で同期を実行する必要があります。同期は、接続、データベース、スキーマ、またはテーブルレベルで実行できます。同期は選択したレベルでのみ行われるため、変更が表示されるようにするには、これら4つのレベルすべてで手動同期を実行する必要があります。

UIを使用するか、プログラムで手動同期を実行できます。Sigma REST APIを使用して手動同期を実行するガイダンスについては、「[Sync a connection by path](https://help.sigmacomputing.com/reference/syncconnectionbypath)」を参照してください。

UIで手動同期を実行するには、以下の手順に従います。
1.  **Administration > Connections**に移動します。
2.  リストから関連する接続を選択します。
3.  `Browse connection`をクリックします。
4.  接続を同期するには（その接続で利用可能なデータベースへの更新を検出します）、接続の`Sync connection metadata`()をクリックします。<img width="995" height="314" alt="64da128-1" src="https://github.com/user-attachments/assets/6ede8db2-52cb-45b8-8852-7d811e90ab6e" />

5.  個々のデータベースまたはスキーマを同期するには、接続を展開し、コンテナを見つけ、データベースまたはスキーマの名前の隣にある`More`をクリックします。あるいは、名前で検索してデータベースまたはスキーマを見つけることもできます。<img width="996" height="334" alt="7b5f8e5-2" src="https://github.com/user-attachments/assets/92603d06-52bd-4c40-b4cd-d6bf0bd1c625" />

    * ドロップダウンメニューから、`Sync now`を選択します。
6.  個々のテーブルを同期するには、接続を展開し、テーブルを含むデータベースを見つけ、そのデータベースを展開し、テーブルを見つけ、テーブルの名前の隣にある`More`をクリックします。あるいは、名前で検索してテーブルを見つけることもできます。
    * ドロップダウンメニューから、`Sync now`を選択します。<img width="996" height="447" alt="3edde1c-3" src="https://github.com/user-attachments/assets/ae259d1c-3e86-442d-bf94-380b0f97e88f" />


### 2-2-7. 入力テーブルの接続問題をトラブルシューティングする (Troubleshoot input table connection issues)

入力テーブルのエラーに遭遇した場合（一般ユーザーとして）、または失敗した入力テーブルの編集を通知するシステムメールを受け取った場合（管理者として）、それは接続またはデータプラットフォームの構成または可用性の問題が原因である可能性があります。この種の問題は、Sigma内の管理者またはデータプラットフォームで直接解決する必要があります。

このドキュメントでは、Sigmaが構成および可用性の問題から生じる入力テーブルのエラーをどのように処理するかを説明し、これらのエラーのトラブルシューティングと解決に関するガイダンスを提供します。

#### **ユーザー要件 (User requirements)**
このドキュメントで特定された入力テーブルの問題を解決する機能には、以下が必要です。
* あなたは`Admin`[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* このドキュメントで特定された解決タスクを実行するために、データプラットフォームで必要な権限を持っている必要があります。

これらの要件を満たしていない場合は、Sigmaまたはデータプラットフォームの管理者に連絡して問題を解決してください。

#### **入力テーブルのエラーハンドリング (Input table error handling)**
データの整合性を向上させ、予期しないデータ損失を防ぐために、Sigmaは入力テーブルのエラーを次のように処理します。
* 接続またはデータプラットフォームの構成または可用性の問題により入力テーブルの編集が失敗した場合、Sigmaはそれを致命的なエラーとして扱い、操作を再試行しません。基盤となる問題はSigmaでは回復不可能であるため、操作を再試行しても失敗し続けます。
* 接続またはデータプラットフォームの構成または可用性の問題から生じる入力テーブルのエラーは、特定のユーザーまたは組織全体に適用される可能性があります。Sigmaがこの種の問題を検出すると、同じエラーの影響を受けるユーザーが入力テーブルを作成および編集する能力を一時的に制限します。最初の入力テーブルエラーの後、関連するすべての既存の入力テーブル要素には「編集が制限されています」というメッセージが表示されます。
* Sigmaは、構成が誤っているか利用できない接続を特定し、エラーメッセージを表示し、このドキュメントへのリンクを含むメールアラートを管理者に送信します。

#### **トラブルシューティングの手順 (Troubleshooting steps)**
エラーをトラブルシューティングするには、以下の手順を完了してください。
1.  システムメールで特定された組織と接続を確認します。これは、複数の組織または接続を管理している場合に重要です。
2.  システムメールで特定されたエラーメッセージを確認します。
3.  `Error messages and resolutions`テーブルで該当するエラーメッセージを探します。該当するエラーメッセージが見つからない場合は、[サポートに連絡](https://help.sigmacomputing.com/hc/en-us/requests/new)してください。
4.  根本原因を確認し、接続に構成されている認証方法に対応する解決策を完了します。

#### **エラーメッセージと解決策 (Error messages and resolutions)**
このセクションでは、Databricks、Redshift、およびSnowflakeに特有の既知の構成および可用性エラーに関する詳細を提供します。以下の表に含まれていないエラーメッセージに遭遇した場合は、[サポートに連絡](https://help.sigmacomputing.com/hc/en-us/requests/new)してください。

##### **Databricksのエラー (Databricks errors)**

* **権限が不十分です (Insufficient privileges)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `execution error: failed to execute query: unexpected operation state ERROR_STATE: [INSUFFICIENT_PERMISSIONS] Insufficient privileges: User does not have <REQUIRED_PRIVILEGE> on <OBJECT_TYPE><OBJECT_NAME>. SQLSTATE: 42501` |
| **根本原因** | サービスプリンシパルが、特定された操作を実行するために必要な権限を持っていません。 |
| **解決策** | Databricksドキュメントの「[Show, grant, and revoke privileges](https://docs.databricks.com/en/data-governance/unity-catalog/manage-privileges/manage-privileges.html)」を参照して、接続に使用されるサービスプリンシパルに必要なカタログとスキーマの権限が付与されていることを確認してください。<br>必要な権限に関する情報については、「[Configure Databricks](https://help.sigmacomputing.com/docs/connect-to-databricks#configure-databricks)」を参照してください。 |

* **無効または期限切れのアクセストークン (Invalid or expired access token)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `Databricks access token is invalid or expired.`<br>または<br>`Invalid Databricks access token.` |
| **根本原因** | 接続構成で提供されたアクセストークンが認証に使用できませんでした。<br>考えられる原因：<br>・提供されたトークンに入力ミスがある。<br>・不正なトークンが提供された。<br>・トークンが削除または失効した。<br>・トークンが期限切れになった。 |
| **解決策 (非OAuth)** | Sigmaで、接続構成ページに移動し、`Connection Credentials` > `Access token`フィールドに有効なトークンを入力します。<br>アクセストークンが期限切れ、削除、または失効した場合は、Databricksドキュメントの「[Databricks personal access tokens for workspace users](https://docs.databricks.com/en/dev-tools/auth/pat.html)」を参照して新しいものを生成してください。<br>アクセストークンの要件に関する詳細は、「[Specify your connection credentials](https://help.sigmacomputing.com/docs/connect-to-databricks#specify-your-connection-credentials)」を参照してください。 |
| **解決策 (OAuth)** | Sigmaで、接続構成ページに移動し、`Service Account Configuration` > `Access token`フィールドに有効なトークンを入力します。<br>アクセストークンが期限切れ、削除、または失効した場合は、Databricksドキュメントの「[Databricks personal access tokens for service principals](https://docs.databricks.com/en/dev-tools/auth/pat-v2.html)」を参照して新しいものを生成してください。<br>アクセストークンの要件に関する詳細は、「[Configure OAuth features](https://help.sigmacomputing.com/docs/connect-to-databricks#configure-oauth-features)」を参照してください。 |

##### **Redshiftのエラー (Redshift errors)**

* **大文字と小文字の区別が有効 (Case sensitivity enabled)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `enable_case_sensitive_identifier must be off` |
| **根本原因** | Redshiftの`enable_case_sensitive_identifier`構成値が`true`に設定されているため、入力テーブルの編集が失敗します。 |
| **解決策** | Redshiftで、`enable_case_sensitive_identifier`を`false`に設定します。<br>構成値に関する詳細は、Redshiftドキュメントの「[enable_case_sensitive_identifier](https://docs.aws.amazon.com/redshift/latest/dg/r_enable_case_sensitive_identifier.html)」を参照してください。 |

---

##### **Snowflakeのエラー (Snowflake errors)**

* **ロールが見つかりません (Role not found)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `Role does not exist` |
| **根本原因** | 接続構成で提供されたロールが、Snowflake環境で見つかりません。<br>考えられる原因：<br>・提供されたロールに入力ミスや大文字小文字の問題がある。<br>・ロールがSnowflakeで削除された。 |
| **解決策 (非OAuth)** | Sigmaで、接続構成ページに移動し、`Connection Credentials` > `Role`フィールドでロール名が正しく入力されていることを確認します。<br>ロールが削除された場合は、Snowflakeドキュメントの「[Create a role](https://docs.snowflake.com/en/user-guide/security-access-control-configure#create-a-role)」を参照して再作成してください（削除されたロールは回復できません）。 |
| **解決策 (OAuth)** | Sigmaで、接続構成ページに移動し、`Service Account Configuration` > `Role`フィールドでロール名が正しく入力されていることを確認します。<br>ロールが削除された場合は、Snowflakeドキュメントの「[Create a role](https://docs.snowflake.com/en/user-guide/security-access-control-configure#create-a-role)」を参照して再作成してください。 |

* **ウェアハウスにアクセスできません (Cannot access warehouse)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `000606 (57P03): No active warehouse selected in the current session. Select an active warehouse with the 'use warehouse' command.` |
| **根本原因** | 接続がウェアハウスにアクセスできません。<br>考えられる原因：ウェアハウスが、無効な、またはユーザーに値が割り当てられていないユーザー属性を使用して設定されている。 |
| **解決策 (非OAuth/OAuth)** | Sigmaで、接続構成ページに移動し、`Connection Credentials` > `Warehouse`フィールドで使用されているユーザー属性名が正しく入力されていることを確認します。<br>提供されたユーザー属性名が有効な場合は、「[Configure user attributes on a Snowflake connection](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照して、ユーザーにウェアハウス属性が割り当てられていることを確認してください。 |

* **テーブルにアクセスできません (Cannot access tables)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `002003 (42S02): SQL compilation error: Object <OBJECT_NAME> does not exist or not authorized.` |
| **根本原因** | 接続が、入力テーブルデータと編集ログを含むテーブルにアクセスできません。<br>考えられる原因：<br>・提供されたロールに、特定されたテーブルにアクセスするために必要なSnowflake権限がない。<br>・テーブルが削除または移動された。 |
| **解決策** | 「[Restore input table access for a Snowflake connection or user](https://help.sigmacomputing.com/docs/restore-input-table-access-for-a-snowflake-connection-or-user)」を参照してください。 |

* **ロールの権限が不十分です (Insufficient role privileges)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `003001 (42501): SQL access control error: Insufficient privileges to operate on schema <SCHEMA_NAME>` |
| **根本原因** | 接続構成で提供されたロールが、特定されたスキーマで操作を実行するために必要なSnowflake権限を持っていません。 |
| **解決策** | Snowflakeドキュメントの「[Grant privileges to a role](https://docs.snowflake.com/en/user-guide/security-access-control-configure#grant-privileges-to-the-role)」を参照して、必要な権限をロールに付与してください。<br>書き込みアクセスを正しく構成するために必要なスキーマ権限に関する詳細は、「[Configure write access](https://help.sigmacomputing.com/docs/connect-to-snowflake#configure-write-access)」を参照してください。 |

* **ユーザーアクセスが無効です (User access disabled)**

| | |
| :--- | :--- |
| **エラーメッセージ** | `390101 (08004): User access disabled. Contact your local system administrator.` |
| **根本原因** | 接続構成で提供されたユーザー名とパスワードが変更されたか、無効になっています。 |
| **解決策 (非OAuth)** | Sigmaで、接続構成ページの`Connection Credentials`セクションで`User`と`Password`フィールド（またはキーペア認証を使用している場合は`User`, `Private key`, `Private key passphrase`）を更新します。<br>あるいは、Snowflakeドキュメントの「[Disabling or enabling a user](https://docs.snowflake.com/en/user-guide/admin-user-management#disabling-or-enabling-a-user)」を参照してユーザーを再有効化します。 |


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

#### 3-2-1. データモデルのナビゲーション (Navigate data models)

データモデルは、**ワークブックページ**と**概要ページ**の2つのページで構成されています。ワークブックページでは、データモデルを構築するための再利用可能な要素を作成・変換でき、一方、概要ページでは、データモデルに関するコンテキストや、組織全体での一般的な使用状況が提供されます。概要ページ内では、メタデータにアクセスして、データの構造、品質、リネージ（系譜）に関する重要なインサイトを得ることもできます。

このドキュメントでは、データモデルのナビゲーションに役立つよう、ワークブックページと概要ページの構造と内容について説明します。

**データモデルのワークブックページ (Data model workbook page)**

ワークブックページでは、単一のデータモデル内で、様々なテーブルや入力テーブルを再利用可能な要素として作成・管理することができます。このフォーマットは、Sigmaのワークブック構造の容易さと柔軟性を、データモデル開発にもたらします。ワークブック分析で行うようにデータを統合・変換し、どの要素が組織全体でデータソースとして再利用できるかを制御します。
<img width="1796" height="1191" alt="69f0d6c4cf15664222a65d94c437198d2d8bece72a5a43430ab6c1e22b851de4-image" src="https://github.com/user-attachments/assets/1685e9da-5bf7-4d42-802a-1eada0d95d94" />


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
<img width="1805" height="936" alt="f15860e040b41573d7192986baa5f0d45d687e963097e956f5e010ea7c00ba09-image" src="https://github.com/user-attachments/assets/58b08561-78c4-42a3-89c5-fabf5866c2f5" />

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
* **f. 探索 (Explore) ボタン:**
    再利用可能要素を新しい探索で開きます。

#### **データの詳細 (Data details)**
概要ページの「詳細」ビューは、データモデル内の個々の再利用可能要素のメタデータへのアクセスを提供し、データプロファイリングとリネージ追跡のための重要なインサイトを明らかにします。

##### **列 (Columns)**
`Columns`タブには、構造メタデータ（列名、データ型、フォーマット、説明）と、データ品質、分布、および変動性を評価するのに役立つシステム生成の統計が含まれています。この情報により、データをより良く理解し、潜在的な問題を特定し、データのユーザビリティを向上させることができます。
<img width="1320" height="875" alt="d7c97865495a162831dd2aa0ffec573980cc72264cce66ffb83e6afc9687d0e9-image" src="https://github.com/user-attachments/assets/6ab05599-502e-49cd-98aa-f502b8530996" />

*システム生成の統計からのインサイト例：*
* `null`の割合が高い場合は、値の欠損や不完全なデータを示唆します。
* `distinct`な値の割合が低い場合は、予期しないデータの冗長性を引き起こす重複レコードを示している可能性があります。
* 最小値と最大値はデータの範囲を表し、データ入力エラーの可能性がある外れ値を明らかにすることができます。
* 高い標準偏差は、データの不整合に寄与する異常値の証拠となり得ます。

##### **コントロール (Controls)**
`Controls`タブには、再利用可能要素に適用されたコントロールに関する情報がリストされます。このデータの透明性は、ユーザーがデータモデル内でデータがどのようにフィルタリングされ、変換されているかを理解するのに役立ちます。
<img width="1320" height="324" alt="7cb0a7e33ddc784c55d8490c419084bdc57f005861b11d9643ed61e1e990f9c1-image" src="https://github.com/user-attachments/assets/0b491ee2-1c16-485c-a2c6-00921ce402eb" />

##### **リネージ (Lineage)**
`Lineage`タブは、再利用可能要素のデータソースと参照（下流の依存関係）に関する詳細を提供し、ユーザーがデータがどこから来たのか、そして組織全体でどこで使用されているのかを特定することを可能にします。
<img width="1320" height="559" alt="f50e3f3bf4fa8aea28dd5e0d87884d13295eafd92b1e0149e49a9ce7e011efb4-image" src="https://github.com/user-attachments/assets/6873eee2-ef58-42c9-9102-03dcce8289d6" />

#### **ハイライトされたメトリクスを探索する (Explore highlighted metrics)**
データモデルにメトリクスが含まれている場合、最大6つのメトリクスが**データモデルの概要**ページに表示されます。データモデルへの編集アクセス権を持つユーザーは、[どのメトリクスをハイライトするかを選択](https://help.sigmacomputing.com/docs/about-metrics#highlight-metrics)できますが、データモデルへのアクセス権を持つ誰もがハイライトされたメトリクスを探索できます。

ハイライトされたメトリクスの詳細を確認するには、データモデルを開き、ハイライトされたメトリクスを選択します。メトリクスの詳細なプロファイルページが開きます。
<img width="1476" height="697" alt="b6c739630a20d27a194a428763b305d5aecf09f72010379abe2442240a6c09a6-dm-metric-profile" src="https://github.com/user-attachments/assets/6d7df059-d7ee-475e-81ca-14fa157d65f6" />
データモデルで定義された各メトリクスについて、以下を確認できます。
* メトリクス名と数式。
* メトリクスを含むデータモデル要素の名前。
* メトリクスの説明。
* メトリクスを使用しているトップドキュメント。ドキュメント名をクリックすると、同じブラウザタブでドキュメントが開きます。
* メトリクスでタイムラインが有効になっている場合は、メトリクスのタイムラインとKPIチャートを探索します。

`Explore in workbook`を選択すると、メトリクスをKPIチャートとして含む新しいワークブックが開きます。

#### 3-2-3. データモデルの作成と管理 (Create and manage data models)

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
2.  `Create New` をクリックし、メニューから `Data Model` を選択します。<img width="1149" height="484" alt="7136646-image" src="https://github.com/user-attachments/assets/cf305374-195c-4d72-b633-d1393e2c1a70" />

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
    `Map columns` モーダルが表示されます。
3.  影響を受けるテーブルの変更された列を確認し、任意で、公開バージョンのデータモデル内の変更された列を、公開予定のドラフト内の置換列にマッピングします。デフォルトでは、変更された列は `No match` にマッピングされ、これにより下流の要素で列がエラーとなります。
    * *例えば、`Normalized Price` という複雑な計算列を更新したい場合、更新された計算ロジックを持つ `Revised Normalized Price` という新しい列を追加し、前の列を削除します。データモデルを公開する際、`Normalized Price` 列を `Revised Normalized Price` 列にマッピングします。*<img width="787" height="447" alt="a91064fd63760e4f08980e6516c4d78fe7d830422f708dea0e2a6ba224b5483e-map-successful" src="https://github.com/user-attachments/assets/7212c963-e5f6-4728-9731-a47dc447678c" />

    * *`Normalized Price` 列を置換列にマッピングせずにデータモデルから削除するには、デフォルトの `No match` の選択のままにします。*
4.  すべての影響を受けるテーブルの関連するすべての列のマッピングが完了したら、`Save and publish` を選択します。

* **トラブルシューティング：列を選択できない (Troubleshooting: Unable to select column)**
    変更された列を別の列にマッピングしたいが、選択できない場合は、以下を実行します。
    1.  `Map columns` モーダルで、`No matches` トグルをオフにします。
    2.  新しい列を `No match` にマッピングし、その後、削除された列を新しい列にマッピングします。
        * *例えば、`Revised Normalized Price` を `No match` にマッピングし、その後、削除された列 `Normalized Price` を置換列 `Revised Normalized Price` にマッピングします。*<img width="789" height="291" alt="e2f2f80ee38232b0fe4f2722e83f64b35604cef95be801681bb4fde9f21800ca-map-success" src="https://github.com/user-attachments/assets/d93eaf68-ed00-4f45-8eeb-a9b956bcd3cc" />

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

##### **データモデルを共有する (Share the data model)**
組織のメンバーが要素をデータソースとして使用できるように、データモデルを共有します。特定のデータモデルを使用するアクセス権が付与されていないユーザーは、ワークブックや他のデータモデルでその要素をデータソースとして表示または選択できません。

1.  共有したいデータモデルを開きます。
2.  データモデルのヘッダーで、ドキュメント名を選択してドキュメントメニューを開き、`Share`を選択します。
3.  `Share Data Model`モーダルで、組織のメンバー、チーム、またはメールアドレスを検索して選択します。
4.  `Permission`フィールドで、オプションを選択します。
    * **Can view:** 選択されたユーザーがデータモデルとその再利用可能な要素を表示・使用できるようにします。
    * **Can edit:** 選択されたユーザーがデータモデルとその再利用可能な要素を表示・使用・編集できるようにします。
5.  `Share`をクリックして権限を保存します。

##### **要素をデータソースとして有効化・無効化する (Enable or disable an element as a data source)**
デフォルトでは、データモデル内の要素はワークブックや他のデータモデルでデータソースとして表示されます。いつでも要素をデータソースとして有効または無効にできます。ソースとして無効化された要素は、データモデルのページ上では利用可能ですが、データモデルの概要からは非表示になり、したがってデータモデルの閲覧者からも非表示になります。

ソースとして無効化された要素間でリレーションシップを作成することはできます。関連する列を他のデータモデルやワークブックで使用可能にするためには、リレーションシップのプライマリソース（またはリレーションシップの階層の最上位のプライマリソース）がデータソースとして有効になっている必要があります。「[Define relationships in data models](https://help.sigmacomputing.com/docs/define-relationships-in-data-models)」を参照してください。
> 🚧
> 要素をソースとして無効にすると、無効化された要素を参照する（同じデータモデル、異なるデータモデル、またはワークブック内の）全ての要素で「Source not found」というエラーメッセージが表示されます。

1.  編集したい要素を含むデータモデルを開きます。
2.  データモデルのヘッダーで、`Edit`をクリックします。
3.  `ERD`または**ワークブックページ**で要素を探して選択し、エディタパネルで`Modeling`タブを選択します。
4.  `Source visibility`セクションで、`Visible as source`トグルをオンまたはオフにします。デフォルトでは、テーブルをワークブックや他のデータモデルのデータソースとして利用可能にするために、トグルはオンになっています。

##### **要素を編集する (Edit an element)**
Sigmaワークブックで行うのと同じように、データモデル内の再利用可能または無効化された要素を編集します。
1.  編集したい要素を含むデータモデルを開きます。
2.  データモデルのヘッダーで、`Edit`をクリックして**ワークブックページ**を開きます。
3.  編集したい要素を探し、必要に応じて変更します。

##### **要素を削除する (Delete an element)**
再利用可能または無効化された要素を削除して、データモデルから永久に削除します。
1.  削除したい要素を含むデータモデルを開きます。
2.  データモデルのヘッダーで、`Edit`をクリックして**ワークブックページ**を開きます。
3.  削除したい要素の上にカーソルを合わせるか選択し、`More`をクリックしてメニューから`Delete element`を選択します。

##### **データモデルを削除する (Delete a data model)**
データモデルを削除するには、あなたがデータモデルの所有者であるか、それに対する`Can edit`アクセス権を持っているか、`Admin`アカウントタイプを持っている必要があります。
1.  データモデル名を選択してドキュメントメニューを開き、`File > Delete...`を選択します。
2.  `Confirm Deletion`モーダルで、`Delete`をクリックします。

##### **削除されたデータモデルを復元する (Recover a deleted data model)**
削除されたデータモデルを復元するには、あなたがデータモデルの所有者であるか、`Admin`アカウントタイプを持っている必要があります。
1.  **ホーム**ページに移動します。
2.  ナビゲーションメニューで、`Trash`を選択します。
3.  `Trash`ページで、削除されたドキュメントのリストを検索し、復元したいものをクリックします。`Name`, `Deleted on`, `Deleted by`の列をソートして、該当するドキュメントを特定するのに役立てることができます。
4.  `Document has been deleted`モーダルで、`Recover`をクリックします。Sigmaは復元されたドキュメントを即座に開きます。

  #### 3-2-3. データモデルでリレーションシップを定義する (Define relationships in data models)

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
5.  エディタパネルで、`Modeling` タブを選択します。`Relationships` セクションで、`+` (リレーションシップを追加) を選択します。<img width="1437" height="868" alt="d9a1ec580897e1c8f8f0518c2ed7eebd0b765bf6d58b683db1fe5f7d625d9aa3-data-model-erd" src="https://github.com/user-attachments/assets/a84690dd-bd9e-4b78-aae2-bf5f36b695f6" />
   `Add a relationship` モーダルが開きます。<img width="1192" height="576" alt="931951e7fb7aea1c01e837b794b21e1af3f738c54a15c831221a78ea7a8d6529-dm-rel-add" src="https://github.com/user-attachments/assets/556ab140-2ec8-4ec7-b3de-c967e5fb9e3e" />

6.  [任意] リレーションシップに名前を付けます。デフォルトでは、リレーションシップ名はターゲット要素のタイトルを使用します。
7.  [任意] リレーションシップに説明を追加します。
8.  `Target source` で、リレーションシップのターゲットとして追加するデータモデル内の要素を選択します。要素をターゲットとして追加すると、その列がソース要素から利用可能になります。
    > 💡
    > ターゲットソースは、ソースとして無効化された要素にすることができます。ターゲットソースが無効化されている場合、下流のユーザーがその要素の列を扱う唯一の方法は、このリレーションシップを通じてです。
9. `Join keys` で、リレーションシップの結合キーとして使用するソース要素とターゲット要素の列を選択します。
10. [任意] `+ Add another mapping` をクリックして、さらに列マッピングを追加します。
11. [任意] ソース要素とターゲット要素のキーマッチングの詳細を確認して、リレーションシップが正しいキーで設定されていることを検証します。`Result preview` を選択して、リレーションシップの出力が期待通りに見えることを確認します。
12. `Save` をクリックします。
13. リレーションシップを下流のユーザーが利用できるようにするには、データモデルを公開します。

ワークブックで関連する列を使用する方法の詳細については、「[Use related columns in a workbook](https://help.sigmacomputing.com/docs/use-related-columns-in-a-workbook)」を参照してください。

**リレーションシップの例 (Example relationship)**

例えば、SigmaサンプルデータベースのBIKESデータをワークブックでより簡単に分析したい場合、次のようにモデリングしてリレーションシップを定義できます。
1.  あなたのデータモデルで、Sigmaサンプルデータベースの `EXAMPLES.BIKES` スキーマをデータソースとして使用し、`TRIP` テーブルと `STATIONS` テーブルを2つのデータ要素として追加します。
    * `TRIP` テーブルは、レンタルバイクでのバイクトリップに関する詳細を提供します。バイクトリップごとに1行あり、各ステーションに対して多くの合計行があります。
    * `STATIONS` テーブルは、各バイクドッキングステーションの場所に関する詳細を提供します。各ステーションごとに1行あります。<img width="1437" height="868" alt="d9a1ec580897e1c8f8f0518c2ed7eebd0b765bf6d58b683db1fe5f7d625d9aa3-data-model-erd" src="https://github.com/user-attachments/assets/2bb71d12-26f4-4ac3-a6dd-4a322bc4f8e8" />

2.  2つのテーブル間にリレーションシップを作成するには、`TRIP` テーブルから始め、`STATIONS` テーブルをターゲット要素として使用します。この方向でリレーションシップを作成すると、多対一（many-to-one）結合のロジックが定義されます。<img width="1192" height="576" alt="931951e7fb7aea1c01e837b794b21e1af3f738c54a15c831221a78ea7a8d6529-dm-rel-add" src="https://github.com/user-attachments/assets/3865492e-377b-4210-85f5-f378888b65c6" />

3.  その後、データモデルを公開すると、ビジネスアナリストはデータモデルから `TRIP` テーブルを扱い、`STATIONS` テーブルから関連する列を簡単に追加できます。Sigmaはリレーションシップで定義されたロジックに基づいて結合を実行し、その結合は関連する列がワークブックに追加されたときにのみ実行されます。<img width="505" height="596" alt="f49529347bdc20fb584a935075ddf64c86fc4b3c62e586a36e59a97986a4c95d-use-related-columns" src="https://github.com/user-attachments/assets/735b74f2-c815-4c45-b9d7-2c747bd938ad" />

**データモデル要素の既存のリレーションシップを確認する (Review existing relationships for data model elements)**

データモデルのエンティティ関係図（ERD）を使用して、データモデル要素間のリレーションシップを確認できます。
* 要素を接続する矢印で方向性のあるリレーションシップを識別します。各リレーションシップには個別の矢印があります。
* 矢印を選択すると、リレーションシップと、ソースおよびターゲット要素の関連するキーがハイライトされます。
* どのリレーションシップが、再利用可能要素のどの列に対して設定されているかを識別します。

### 3-3. メトリクスについて (About metrics)

メトリクスとは、データソースに固有の、動的で再利用可能な計算のことです。そのため、メトリクスは通常、特定の列を参照します。信頼性が高く効率的な集計計算を提供するためにメトリクスを作成し、ビジネスユーザーから複雑な数式を抽象化することができます。

例えば、以下のようなメトリクスの例を計算することがあります。
* 収益データソースの年間経常収益（ARR）、純ドル維持率（NDR）、および解約率。
* 顧客データソースの総顧客数、エンゲージ顧客数、およびアクティブ顧客数。
* 製品テレメトリデータソースの月間アクティブユーザー数。
* ウェブサイト分析データソースの総ページビュー数、ユニークユーザー数、および総セッション数。

これらのいくつかは計算が反復的であり、他は複雑で異なる解釈で構築される可能性があるため、個々のビジネスユーザーが計算列として独立して計算することは望ましくありません。メトリクスは、組織全体で一貫性のある正確な計算を保証するのに役立ちます。

もし、特定のデータ型の任意の列を引数として受け取ることができる再利用可能な計算を作成したい場合は、代わりに[カスタム関数](https://help.sigmacomputing.com/docs/intro-to-custom-functions)を作成してください。カスタム関数は数式内で使用できます。

#### **メトリクスと計算列の使い分け (Choosing between metrics and calculated columns)**

メトリクスは、データソース固有であり、したがって特定のデータソース列に関連付けられた、動的で再利用可能な計算です。メトリクスは、あらゆるグルーピングレベルで集計された値を提供します。

計算列は、静的であり、それらが作成されたデータ要素に固有です。計算列は、計算を使用して、個々の（グループ化されていない）テーブル行に対する静的な非集計値を生成するか、特定の静的なグルーピングレベルで集計された値を生成します。

データ要素に計算列を追加するとき、あなたはその計算ロジックを定義します。メトリクスのロジック定義はデータソース内に存在し、そのデータモデル、データセット、またはデータベーステーブルを参照するどの要素でも再利用できます。

計算のロジックが変更された場合、該当する全ての要素で計算列を個別に編集する必要があります。代わりにメトリクスを使用する場合、データソースでメトリクスの数式を一度更新すれば、そのメトリクスを使用する全ての要素でメトリクスの結果が自動的に再計算されます。

データモデルやデータセットにメトリクスや計算列を追加できます。また、接続からデータベースやカタログテーブルにメトリクスを追加することもできます。

#### **制限事項 (Limitations)**

* メトリクスは、JoinやUnionを越えて、あるいは全てのソース列ではなくグルーピングレベルに基づいた子要素へは伝播しません。結合されたテーブルの子要素でメトリクスを利用可能にするには、結合の出力に対してメトリクスを定義してください。
* メトリクスは単一のデータソース内でのみ定義できます。同じメトリクスロジックが組織全体、または複数のデータソースにわたって適用される場合、該当する各データモデル、データセット、またはデータベーステーブルでそれぞれメトリクスを定義する必要があります。
* メトリクスの数式は、[ウィンドウ関数](https://help.sigmacomputing.com/docs/window-functions)や[結合関数](https://help.sigmacomputing.com/docs/join-functions)をサポートしていません。
* [動的テキスト](https://help.sigmacomputing.com/docs/dynamic-text)内でメトリクスを直接参照することはできません。動的テキストにメトリクスの出力を含めるには、メトリクスを参照する計算列を作成し、その列を動的テキストの数式で参照してください。

##### **データセット固有の制限事項 (Dataset-specific limitations)**
メトリクスを持つデータセットやデータベーステーブルに基づいてデータセットを作成した場合、メトリクスは継承されません。代わりに、メトリクスを再作成する必要があります。

##### **データモデル固有の制限事項 (Data model-specific limitations)**
マテリアライズされている、またはマテリアライズされた子要素を持つデータモデルでメトリクスを追加、編集、または削除した場合、新しいマテリアライゼーションジョブが実行されるまで、マテリアライズされたデータは使用されません。新しいまたは更新されたメトリクスが以下の条件を満たす場合、マテリアライズされたデータが使用されます。
* メトリクスによって使用される列が、既存のメトリクスによって使用されている。
* 更新されたメトリクスが新しい列を参照していない。例えば、メトリクスの数式を `[Column] * 0.1` から `[Column] * 100` に変更しても、新しいマテリアライゼーションの実行は必要ありません。
  
* #### 3-3.1 メトリクスの作成と管理 (Create and manage metrics)

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
        `Add a metric` モーダルが表示されます。
    5.  `Name` フィールドに、メトリクスに使用する名前を入力します。
    6.  `Description` フィールドに、メトリクスが何をするかの説明を入力します。この説明は、ユーザーがメトリクスにカーソルを合わせたときに表示されます。
    7.  `Formula` フィールドで、メトリクスのロジックを定義します。Sigmaの関数を使用したり、データモデルのテーブル内の任意の列を参照したり、別のメトリクスを参照したりできます。<img width="932" height="645" alt="4c93e56a2b6bb36f40629cceef2f4a5ffefdaa0c5b9c19cc1358f7b8d5905e2c-dm-add-metric" src="https://github.com/user-attachments/assets/5793ad02-7e1a-4c48-95e9-2ab40b2c9bd1" />

    8.  [任意] `Timeline` スイッチをオンにすると、**データモデルの概要**ページにメトリクスのタイムラインが表示されます。
        * `Date` で、タイムラインに使用するデータ内の日付列を選択します。
        * `Truncation` で、日付をどのように切り捨てるかを選択するか、日付の切り捨てを削除して日付列の既存の粒度を使用するかを選択します。
        *  [任意] `Compare period` で、メトリクスの比較期間を選択するか、`None` を選択します。
        *  [任意] `Direction` で、比較トレンドの方向を選択するか、`None` を選択します。
    9. メトリクスの `Preview` を確認し、任意でメトリクスの出力フォーマットを定義します。
        * 例えば、数式の結果を通貨やパーセンテージとして指定したり、小数点以下の桁数を設定したり、数値フォーマットメニュー()をクリックして完全なフォーマットメニューからオプションを選択したりできます。
        > 📘
        > メトリクスは集計計算を定義します。プレビューがnull値を表示する場合、あなたの数式には `Sum()`, `Avg()`, `Count()` などの集計関数が欠けている可能性があります。
    10. データモデルを公開して、変更を下流で利用可能にします。

* **データモデルの概要でメトリクスをハイライトする (Highlight a metric in the data model overview)**
    デフォルトでは、データモデルで作成した最大6つのメトリクスが**データモデルの概要**ページに表示されます。どのメトリクスを表示するかを変更するには、概要ページで特定のメトリクスをハイライトして、それらだけを表示するように選択できます。
    1.  編集のためにデータモデルを開きます。
    2.  メトリクスを追加したいデータモデル要素を選択します。
    3.  エディタパネルで、`Modeling` タブを選択します。
    4.  エディタパネルの `Modeling` タブの `Metrics` セクションで、メトリクスを探します。
    5.  そのメトリクスについて、`More` () をクリックし、`Highlight in overview` を選択します。
    6.  データモデルを公開して、変更を利用可能にします。<img width="829" height="289" alt="f529d9f2d1ea4e921516e8c5a2cfc2356960b8b79ec51f34a6c47e9d16a6ef97-highlighted-metrics" src="https://github.com/user-attachments/assets/09b23160-fa64-4380-b150-7f4f8ade1950" />

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
    8.  ヘッダーで `Publish` をクリックしてメトリクスを保存します。<img width="1149" height="557" alt="a400f0d-3" src="https://github.com/user-attachments/assets/3ca95081-836f-47ba-976d-5280d19aa0cb" />


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
    5.  そのメトリクスについて、`More` () をクリックし、`Delete` を選択します。<img width="1149" height="279" alt="cb0d1c0-8" src="https://github.com/user-attachments/assets/aae68572-9973-4df4-8736-b6e0e6834445" />

        あるいは、メトリクスを選択してメトリクスビルダーを開き、サイドパネルでメトリクスを探します。メトリクスの名前の隣にある `Delete metric` () をクリックします。<img width="1149" height="354" alt="13798f1-9" src="https://github.com/user-attachments/assets/d312a874-ab89-4efc-a78b-a04e89447c00" />

 
   #### 3-4. データカタログのレビューと管理 (Review and manage your data catalog)

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
<img width="1719" height="925" alt="563a7477ed80e266ea5e279dd44c75a7901a1106c90c80eb74734bdeb270f6bf-view-data-catalog" src="https://github.com/user-attachments/assets/7d4a5a33-aa78-4abd-8b80-5cf8e0bb5bc2" />

* **テーブルの説明を追加する (Add table descriptions)**
    データカタログでテーブルを見つけたら、説明を追加します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  右上の `Edit` を選択します。
    4.  テーブル名の隣にある `More info` () を選択します。
    5.  表示されるポップオーバーで、`Description` フィールドに説明を入力します。<img width="649" height="373" alt="9427d4eb8011689db736f8f38af96a6abbdb7879c19a948db8c7182c9ea74769-edit-table-descr-db-table" src="https://github.com/user-attachments/assets/9fee68fa-e4a9-475d-99c2-d49604f52eec" />

    6.  変更を保存するには、`Publish` を選択します。

* **バッジを追加または更新する (Add or update a badge)**
    データのステータス、品質、信頼性を示すために、認定バッジを追加または更新します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  テーブル名の隣にある `More info` () を選択します。
    4.  ポップオーバーで、`Badge` ドロップダウンからオプションを選択します。<img width="1336" height="457" alt="78287f84edecad3e43dfabc88333e7bd32f9c6cbb4c9ce786d540c74d33b48b2-2025-02-13_23-12-13" src="https://github.com/user-attachments/assets/f4aa575c-02c5-46e7-acee-d26c5f151138" />

    5.  [任意] バッジを選択すると、ポップオーバーに `Badge note` フィールドが表示されます。バッジに関するコンテキストを提供するためにメモを追加します。

    バッジは自動的に保存され、左パネルのテーブルアイコンに即座に反映されます。<img width="1336" height="520" alt="1f561bb406350a33516423ea091c28754a95019249c2f0705029bab7e324d188-2025-02-13_23-40-41" src="https://github.com/user-attachments/assets/31a8401a-362e-4ca4-b02d-2d49a16210d5" />


* **列の説明を追加する (Add column descriptions)**
    データソースのユーザーに追加のメタデータとガイダンスを提供するために、列に説明を追加します。
    1.  データカタログでテーブルに移動します。
    2.  テーブル名を選択してテーブルを開きます。
    3.  右上の `Edit` を選択します。
    4.  `Columns` タブを選択します。
    5.  `Description` 列で、テーブル内の任意の列に説明を追加します。<img width="1377" height="670" alt="cb0b2139d79fbdf4299ff32ddec3e859ac7e12c2be26834f4ebbb2c2837eb53c-update-columns-db-table" src="https://github.com/user-attachments/assets/2bad08e6-6fcf-4364-8b3d-10157935b24f" />

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

#### 3-5-1. データセットの作成と管理 (Create and manage datasets)

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
4.  テーブル名を選択してテーブルを開きます。<img width="1719" height="925" alt="563a7477ed80e266ea5e279dd44c75a7901a1106c90c80eb74734bdeb270f6bf-view-data-catalog" src="https://github.com/user-attachments/assets/1f53b9f6-568c-46a3-8abb-e11b17604c89" />
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
    3.  ポップオーバーで、`Badge` ドロップダウンからオプションを選択します。<img width="1336" height="591" alt="cd187ccbc76e4fecde9d0f17612432daf3ba0914f9c0f0e934d2dc34511a83b8-2025-02-13_23-25-54" src="https://github.com/user-attachments/assets/82cf8bed-4128-44fc-96ef-ef7264ad5490" />

    4.  [任意] バッジを選択すると、ポップオーバーに `Badge note` フィールドが表示されます。バッジに関するコンテキストを提供するためにメモを追加します。<img width="1336" height="696" alt="5aac68f70f462ac91619f31e45d2721631771954fddde7e459a7261799826075-2025-02-13_23-33-20" src="https://github.com/user-attachments/assets/aa6dc357-5e9f-4b5d-8547-c0c66d7b3720" />
    バッジは自動的に保存され、データセットのヘッダーに即座に反映されます。<img width="805" height="101" alt="f58ae3ac97e5a41634693591d4c86aee2f3ff6f2c16ffe8707a15accda535b95-2025-02-13_23-28-42" src="https://github.com/user-attachments/assets/05dd8850-86de-495e-a435-773d84760476" />

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

5.  #### 3-5-2. データセットのベストプラクティス (Dataset best practices)

* **レベルを最小限にする (Minimize Levels)**
    データセットのワークシートタブにあるすべてのレベルは、そのデータセットを基に作成されたワークシートではフラット化されます。混乱を防ぐため、主要な計算に必要なレベルのみを作成してください。

* **フィルターを考慮する (Consider Your Filters)**
    最も関連性の高いデータを表示するためにフィルターを適用すると、インサイト発見のプロセスがはるかに速くなります。マテリアライゼーションと組み合わせると、クエリの実行も速くなります。最良のフィルターとは、制限しすぎることなく、無関係なデータを削減するものです。

* **データセットを説明する (Describe the Dataset)**
    もしデータセットが特定のユースケースの基盤として構築された場合、良いタイトルと説明は、人々にそのユースケースが何であるかを知らせます。データセットがいつ使用されるべきで、いつ使用されるべきでないかを明確にすることが重要です。

* **マテリアライズする (Materialize)**
    データセットのマテリアライゼーションを設定している場合は、使用しているデータがデータベースでいつ更新されるかを確認してください。データベースの更新後に更新スケジュールが発生するように設定したいはずです。

#### 3-5-3. チュートリアル：データセットを使用したデータモデリング (Tutorial: Data modeling with datasets)

データチームは、ビジネスユーザーによるデータ探索を可能にするためにデータセットを作成することが多いですが、データセットは多くの理由で作成されます。例えば以下のような理由です。
* ディメンショナルモデルの結合とフラット化
* 機密データのマスキング
* パフォーマンス向上のためのデータのマテリアライズ
* 共通の計算や重要業績評価指標（KPI）の一貫性を確保する

このステップバイステップガイドでは、ディメンショナルモデルをフラット化するデータセットの作成手順を説明します。

**要件 (Requirements)**

* あなたはCreatorアカウントタイプ、またはモデリング権限を含むカスタムアカウントタイプを割り当てられている必要があります。

**データセットを作成する (Create Datasets)**
1.  ホームページの上部で、`Create New` をクリックし、`Dataset` を選択します。<img width="1280" height="720" alt="4216dec-1" src="https://github.com/user-attachments/assets/8e338631-bbe2-4402-9fd9-722ff8607806" />
2.  `Select a Data Source` ページで、`Table` オプションを選択します。<img width="1280" height="720" alt="a870abb-2" src="https://github.com/user-attachments/assets/3f0a601f-6ec5-487c-9bd0-75d77e257ed2" />
3.  左パネルのConnectionsセクションを見つけ、`Sigma Sample Database` を選択します。
4.  `Examples` データベースと `PLUGS_ELECTRONICS` スキーマを探します。
5.  `F_POINT_OF_SALE` テーブルをクリックして、データのプレビューを表示します。<img width="1280" height="720" alt="664e345-3" src="https://github.com/user-attachments/assets/ba6dddb0-124a-43ce-80c8-2e11e59a4f5a" />
6.  ページヘッダーの右上隅にある `Get Started` をクリックします。

**データをモデリングする (Modeling Data)**

* **計算を作成する (Create Calculations)**
    データセットを構築するためのテーブルを見つけたので、次に追加の列に計算を追加します。データセットに計算列を追加することで、組織によるメトリクスやKPIの計算方法の一貫性が保証されます。計算列は、アナリストが毎回共通の計算をワークブックに追加する必要がなくなるため、貴重な時間節約になります。
    1.  画面上部の `Worksheet` タブをクリックします。<img width="1280" height="720" alt="625b47d-4" src="https://github.com/user-attachments/assets/8e1c23aa-2ab0-4ce5-9f60-80c9be905062" />

    2.  `Sales Amount` 列のキャレットアイコン()をクリックします。
    3.  `Add New Column` をクリックします。<img width="1280" height="720" alt="cb3609d-5" src="https://github.com/user-attachments/assets/3f2d53ec-665c-4112-a76e-68e8b09e8579" />

    4.  数式バーに `[Sales Amount] * [Sales Quantity]` と入力します。<img width="1280" height="720" alt="05b82ff-6" src="https://github.com/user-attachments/assets/c2d9c4a6-b7ce-43be-9dd7-dad6e6ba98fa" />

    5.  キーボードの `Enter` をクリックします。
    6.  新しい列の名前をダブルクリックし、`Revenue` に変更します。
    7.  `Revenue` 列のキャレットアイコン()をクリックします。
    8.  `Format` を選択します。
    9.  `Currency` を選択します。<img width="1280" height="720" alt="8cd0b4f-7" src="https://github.com/user-attachments/assets/ada28772-bd97-4aa7-9139-3bdec36c73c9" />

    10. ステップ1-5を繰り返し、`COGS` (Cost of Goods Sold) という名前の別の列を追加します。
        * 数式バーに `[Cost Amount] * [Sales Quantity]` と入力します。
    11. キーボードの `Enter` をクリックします。
    12. `COGS` 列のキャレットアイコン()をクリックし、`Format` を選択します。
    13. `Currency` を選択します。

* **追加のテーブルを結合する (Joining additional tables)**
    このデータセットに追加のテーブルを結合して、上記で作成したデータセットにさらなるコンテキストを追加しましょう。
    Sigmaはleft, right, full, inner joinタイプ、およびlookupをサポートしています。複数の列を結合したり、結合内で任意の関数（例：日付の切り捨て）を定義したりすることもできます。詳細は「[Join types](https://help.sigmacomputing.com/docs/join-data#join-types)」を参照してください。
    1.  データセットが編集モードの状態で、データベースアイコンをクリックしてそのタブを開きます。これは右側のパネルにあります。<img width="1280" height="720" alt="9eb7f07-8" src="https://github.com/user-attachments/assets/3ff2bb2b-60eb-4282-be4a-21999f866a59" />
    2.  データベースアイコンの下にあるプラスアイコン()をクリックします。これにより `Add Source` ページが開きます。<img width="1280" height="720" alt="73683cd-9" src="https://github.com/user-attachments/assets/b80e3a1c-e1b5-4e0d-be55-216b8b3b2822" />
    3.  データソースタイプとして `Table` を選択します。<img width="1280" height="720" alt="7062633-10" src="https://github.com/user-attachments/assets/166feee8-e3db-4b30-848d-d72ed26f9adc" />
    4.  ページの左側、`Connections` の下で、`Sigma Sample Database` を選択します。
    5.  `Examples` データベースと `PLUGS_ELECTRONICS` スキーマを探します。
    6.  `F_SALES` テーブルをクリックしてデータのプレビューを表示します。
    7.  ページヘッダーの右上隅にある `Next` をクリックします。
    8.  `Join Type` で、デフォルトの `Left Join` を使用します。
    9.  左の結合キーセレクタを `ORDER_NUMBER` 列に設定します。
    10. 右の結合キーセレクタを `ORDER_NUMBER` 列に設定します。<img width="1280" height="720" alt="97e1703-11" src="https://github.com/user-attachments/assets/d8c231f4-6b1b-42fd-8af0-ab1bed8f4a72" />

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
          <img width="1280" height="720" alt="52a6e07-12" src="https://github.com/user-attachments/assets/b34e0365-a0e3-4ea6-a8d7-b0f0ed1e34ba" />

        * *注：結合を介して追加されたすべての列には、括弧内にテーブル名が付加されます。列名をダブルクリックして名前を変更します。列をワークシートの新しい位置にドラッグして移動します。*

* **JSONを抽出する (Extracting JSON)**
    SigmaではJSONを抽出する機能があります。
    1.  `Cust Json Field (D_CUSTOMER)` 列のキャレットアイコン()をクリックします。
    2.  `Extract Columns` を選択します。<img width="1280" height="720" alt="a53e61c-13" src="https://github.com/user-attachments/assets/9eeafc18-ba84-465c-b3d1-50162bccfd7b" />
    3.  `Extract Fields` モーダルで、`AGE_GROUP` と `LOYALTY_PROGRAM` フィールドを選択します。<img width="846" height="666" alt="87b764a-14" src="https://github.com/user-attachments/assets/2f7da950-91d3-4995-af6f-47dad5efe693" />
    4.  `LOYALTY_PROGRAM` のキャレットアイコン()をクリックします。
    5.  `Logical` を選択します。<img width="1764" height="1314" alt="38b9a34-15" src="https://github.com/user-attachments/assets/8d970e26-6ff9-414d-8499-d596afc5cd83" />
    6.  `Confirm` ボタンをクリックします。

* **データをフィルタリングする (Filter Your Data)**
    データセットをフィルタリングすると、データ探索中にアナリストが利用できるデータの量が制限されます。
    * **相対日付フィルターを追加する**
        1.  `[Date (F_SALES)]` のキャレットアイコン()をクリックします。
        2.  `Add Filter` を選択します。
        3.  フィルタータイプとして `Date Range` を選択します。
        4.  `Select Date Range` フィールドをクリックして、日付選択メニューを表示します。<img width="1280" height="882" alt="2e7869e-16" src="https://github.com/user-attachments/assets/92957832-1681-45d5-9c05-53c97a3af867" />

        5.  モーダルの左側で `Relative` を選択します。
        6.  テキスト入力フィールドに `1` と入力します。
        7.  `...` メニューで `Weeks` を選択します。
            * *注：このフィルターにより、データは常に最新の週にフィルタリングされます。*
        <img width="1280" height="720" alt="8ab028c-17" src="https://github.com/user-attachments/assets/67e26eef-16f4-4bd5-8f6e-1c34d18b20f3" />
        8.  `Save` をクリックします。
           
    * **テキストフィルターを追加する**
        1.  `Store State` 列のドロップダウン矢印をクリックし、`Add Filter` を選択します。
        2.  `Filter Values` ドロップダウンメニューをクリックします。<img width="1280" height="720" alt="0b9a2da-18" src="https://github.com/user-attachments/assets/70fbbc7f-3849-4a7b-b21e-d15eaaf8cedd" />
        3.  `California`, `Texas`, `Michigan` のチェックボックスをオンにします。<img width="1280" height="931" alt="c22c926-19" src="https://github.com/user-attachments/assets/5ea71c4e-77ce-4fc5-84fc-38089e1897de" />
        4.  `Save` をクリックします。

* **テーブルをリンクする (Link Tables)**
    データセットでリンクを定義することにより、ユーザーは結合されたデータをワークブックに追加するオプションを得ます。さらに、SigmaはSnowflakeでリレーショナルメタデータ（外部キー）が定義されているテーブルを自動的にリンクします。
    1.  画面上部の `Links` タブをクリックします。<img width="1280" height="720" alt="8fe0b5b-20" src="https://github.com/user-attachments/assets/c9d22d70-9f3f-4524-bc5b-9bbfc09d9257" />
    2.  `Add links to other source` をクリックします。<img width="1280" height="720" alt="01dd00e-21" src="https://github.com/user-attachments/assets/c4c7afc5-5ae4-48bf-b441-ebd8b53ba1f3" />
    3.  左パネルの下部にある `Connections` をクリックします。<img width="1280" height="931" alt="5dfc6e6-22" src="https://github.com/user-attachments/assets/5a182533-8299-4bb9-89e5-b80d00d81a88" />
    4.  `Sigma Sample Database` を選択します。
    5.  `Examples` と `PLUGS_ELECTRONICS` フォルダを探します。
    6.  `D_PRODUCT` テーブルをクリックしてデータのプレビューを表示します。<img width="1280" height="931" alt="496b49d-23" src="https://github.com/user-attachments/assets/ca93aafa-ba17-46b0-b163-97a8561e81d4" />
    7.  `Next` をクリックします。
    8.  `Join Type` の選択を見つけ、`Left Join` を選択します。
    9.  左の結合キーセレクタを `PRODUCT KEY Link (F_POINT_OF_SALE)` に設定します。
    10. 右の結合キーセレクタを `PRODUCT KEY` に設定します。<img width="1280" height="931" alt="3222b66-24" src="https://github.com/user-attachments/assets/a9c0e90d-e868-4a84-a039-a3128104d654" />

    11. `Save` をクリックします。
    12. 画面上部の `Publish` ボタンをクリックして、すべてのデータセットの変更を保存します。

* **データセットにバッジを付ける (Badging Datasets)**
    データセットにバッジを追加して、コンテンツが `Endorsed`（推奨）、`Warning`（警告）、または `Deprecated`（非推奨）であることを示します。任意のバッジノートを使用して、すべての組織メンバーに追加のコンテキストを提供できます。
    * **バッジを追加または更新する**
        1.  ページヘッダーの情報アイコン()をクリックします。これにより、ページのポップアップが開きます。
        2.  ドロップダウンリストから `Endorsed` バッジタイプを選択します。<img width="1280" height="720" alt="15aebdc-25" src="https://github.com/user-attachments/assets/1b8a319d-2164-4f53-8bbe-f30585156509" />

* **権限設定とデータセットの共有 (Setting Permissions & Sharing Datasets)**
    モデリングが完了したら、データセットを共有できます。ユーザーのチームや個人に[直接共有](https://help.sigmacomputing.com/docs/share-a-dataset#direct-share)するか、より広範に[ワークスペース](https://help.sigmacomputing.com/docs/share-a-dataset#move-to-workspace)に共有することができます。権限が付与されると、人々はデータセットを分析の基礎として使用できます。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
    * **直接共有 (Direct Share)**
        1.  画面上部の `Permissions` タブをクリックします。
        2.  `Add Permission` をクリックします。<img width="1280" height="720" alt="cad52ef-26" src="https://github.com/user-attachments/assets/9a1fc4e7-0caf-40f7-b45c-56e0ee628ae5" />
        3.  メンバーのメールアドレスまたはチーム名を検索します。<img width="1280" height="720" alt="4e2b5a3-27" src="https://github.com/user-attachments/assets/d0b0a57e-aa58-49f4-8f1a-5861d8f7e042" />

        4.  選択したメンバーまたはチームに付与したい権限の種類を選択します。<img width="1280" height="720" alt="d975497-28" src="https://github.com/user-attachments/assets/63ae7d88-68e0-4a0e-8cfb-35cdfb68bdc7" />

            * *注：ユーザーはホームページの「Shared with Me」タブからデータセットにアクセスできるようになります。*
    * **ワークスペースへ移動 (Move to Workspace)**
        1.  データセットヘッダーの `More` をクリックします。
        2.  `Move` をクリックします。<img width="1280" height="720" alt="32e6e40-29" src="https://github.com/user-attachments/assets/94d2e7fe-4285-4944-a042-5c762f45f9ac" />

        3.  `Workspaces` タブをクリックします。<img width="1280" height="931" alt="1384d2a-30" src="https://github.com/user-attachments/assets/bccc9553-f3c4-4af5-873e-ca0326b1c8de" />

        4.  データセットを移動したいワークスペースを選択します。<img width="1280" height="931" alt="4b85bae-31" src="https://github.com/user-attachments/assets/802b8979-55f7-4e0d-9ccc-197514906a85" />

        5.  `Move` をクリックします。

* **マテリアライゼーション (Materialization)**
    マテリアライゼーションにより、データセットをテーブルとしてウェアハウスに書き戻すことができます。これらのテーブルは、Sigmaで構築する複雑なSQLクエリの簡略化版として機能し、下流のレポートの速度とパフォーマンスを向上させることができます。各テーブルは、設定したスケジュールでウェアハウスに書き込まれ、再書き込みされます。Sigmaはテーブルの上にビューを作成するため、Sigma外の他のアプリがSigmaの作成した準備済み/変換済みデータにアクセスできます。
    * **要件 (Requirements)**
        * データセットの接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。
        * あなたは組織のAdminである必要があります。
    * **データセットにマテリアライゼーションを追加する**
        1.  画面上部の `Materialization` タブをクリックします。<img width="1280" height="720" alt="b619d7a-32" src="https://github.com/user-attachments/assets/c3e820f0-541b-4f74-ad41-fe6ad9b93813" />
        2.  `Create Schedule` をクリックします。<img width="1280" height="720" alt="f06593a-33" src="https://github.com/user-attachments/assets/a90ebbb3-2c12-46e9-a8aa-3d2a12113e6e" />
        3.  データをマテリアライズする頻度を選択します。<img width="1280" height="720" alt="0bb4ee1-34" src="https://github.com/user-attachments/assets/ea225629-b222-4e36-92cc-9efc14e896db" />
        4.  `Save` をクリックします。
        マテリアライゼーションのスケジュールを保存すると、Sigmaは最初のマテリアライゼーションを実行します。
        スケジュールされた全てのマテリアライゼーションは、データセットの `Materialization` タブで表示できます。

#### 3-5-4. データセットワークシート入門 (Introduction to the Dataset Worksheet)

データセットのワークシートを使用すると、そのデータを構造化し、操作することができます。計算の作成、データのグループ化、フィルターやフォーマットの適用、パラメータの追加などが可能です。データセットのワークシートには、少なくとも一つのデータソースが含まれている必要があります。データソースの例としては、あなたの組織のデータウェアハウスのテーブル、アップロードされたCSV、さらには他のデータセットも含まれます。


**ワークシートタブの構成 (Worksheet Tab Anatomy)**
<img width="3584" height="1968" alt="65ea8e1-dataset-worksheet" src="https://github.com/user-attachments/assets/b217f5d3-14b5-401f-8123-aa0ad606396b" />

* **数式バー (The Formula Bar)**
    各ワークシートには、ページの上部近くに数式バーが配置されています。<img width="3584" height="324" alt="fbb79de-20-dataset-worksheet-formula-bar" src="https://github.com/user-attachments/assets/c2e9b486-d3c6-4508-8180-73c28baf795c" />

    数式はセルではなく、列に適用されます。数式が列に適用されると、その列のすべての行に適用されます。
    データソースから直接データを参照している列を含め、すべての列には数式があります。列の数式を表示するには、その列を選択すると、数式バーに自動的にその数式が表示されます。
    ワークシートで新しい計算を作成するには、まず新しい列を追加し、その列に数式を追加する必要があります。Sigmaの最も[人気のある関数](https://help.sigmacomputing.com/docs/function-index)から始めてみましょう。

* **右側パネル (The Right Side Panel)**
    どのワークシートの右側にあるパネルにも、列ビューとデータソースリストの2つのコンポーネントがあります。
    * **列ビューパネル (The Column View Panel)**
        列ビューパネルには、ワークシート内の全列の完全なリストが含まれています。非表示に設定されていない限り、これらの列はすべてワークシートのスプレッドシートに表示されます。<img width="504" height="1626" alt="9c74941-21-dataset-worksheet-right-bar" src="https://github.com/user-attachments/assets/1f09111f-a8c9-406f-9fcc-c74b857be333" />

        ここから、ワークシートの列を整理し、レベルにグループ化することができます。前述のスプレッドシートセクションで述べたように、レベル化されたグループを作成することで、選択した列の共通の特性に基づいてデータの行をまとめることができます。列ビューパネルからデータをグループ化すると、それらのグループは自動的にワークシートのスプレッドシートに反映されます。
        この列ビューパネルには、ワークシートの合計のためのセクションも含まれています。合計は、ワークシートの最上位レベルに存在する単一値の列集計です。
    * **データソースパネル (The Data Source Panel)**
        ワークシートの右側パネルにある2番目のタブをクリックすると、データソースパネルが開きます。このパネルには、ワークシートのデータソースが表示されます。ここから、データソースを編集したり、結合したりすることができます。
        各データソースにはその列のリストが含まれているため、ソースのドロップダウン列リストから、ワークシートに欠けているデータソースの列を追加することもできます。
<img width="510" height="1471" alt="9bc5ad9-22-dataset-right-datasource-tab" src="https://github.com/user-attachments/assets/4ab0a15f-063e-438c-b30b-afe5d37b22c1" />

* **コントロールパネル (The Control Panel)**
    ワークシートには、画面の左側に展開可能なコントロールパネルがあります。これには、ワークシートのフィルターとパラメータが含まれています。また、合計値が存在する場合は、それも含まれます。<img width="1644" height="1101" alt="bef05d1-23_-_dataset-worksheet-left-bar" src="https://github.com/user-attachments/assets/487a5b1a-ad1a-4f50-8d4c-d6c8cd1d9074" />

  #### 3-5-4-1. データセットワークシートのコントロール (Dataset worksheet controls)

**ユーザー要件 (User requirements)**

データセットワークシートのコントロールを利用するには、以下が必要です。
* `Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。
* あなたはデータセットの所有者であるか、`Can edit` のデータセット権限を付与されている必要があります。

**コントロールパネルの開閉とサイズ変更 (Opening, closing, and resizing the control panel)**

Sigmaのワークシートコントロールは、ワークシートのテーブルおよびチャートエリアの真左に配置された、ワークシートコントロールパネル内にあります。この配置により、コントロールの値を作成・修正しながら、同時にデータがリアルタイムで応答するのを見ることができます。

コントロールパネルを開くには、ワークシートの左側にある `CONTROLS` バー、またはツールバーの `Show Controls` ボタンをクリックします。
<img width="1280" height="853" alt="06d6c4a-37_-_hide-controls" src="https://github.com/user-attachments/assets/afbbe2b1-8f40-4d00-b5bb-806df88673d4" />

コントロールパネルは、その右側にある青いホバーバーをドラッグすることで、サイズ変更したり閉じたりすることができます。

**合計 (Totals)**

合計は、ワークシートの最上位レベルに存在する単一値の列集計です。計算されたワークシートの合計は、コントロールパネルの `TOTALS` セクションで表示および選択できます。`TOTALS` セクションは、ワークシートに一つ以上の合計が存在する場合にのみ表示されます。「[Dataset totals](https://help.sigmacomputing.com/docs/dataset-totals)」を参照してください。

**フィルター (Filters)**

フィルターを使用すると、特定の条件を満たす行のみを表示するようにデータを制限できます。ワークシートのフィルターは、コントロールパネルの `FILTERS` セクションで作成および管理できます。「[Dataset filters](https://help.sigmacomputing.com/docs/dataset-filters)」を参照してください。

**パラメータ (Parameters)**

パラメータは、ワークシートに追加し、数式で参照できるカスタマイズ可能なフィールドです。パラメータは、What-If分析やユーザー入力分析にとって非常に大きな資産となり得ます。ワークシートのパラメータは、コントロールパネルの `PARAMETERS` セクションで作成および管理できます。「[Dataset parameters](https://help.sigmacomputing.com/docs/dataset-parameters)」を参照してください。

#### 3-5-4-2. データセットワークシートの列 (Dataset Worksheet Columns)

列はSigmaで作業する上で中心的な役割を果たします。データセットワークシートを作成する際、既存の列を構造化・フォーマットしたり、列の計算を作成したり、データをソート・フィルタリングしたりすることができます。

**データセットワークシートで列を表示する (View columns in dataset worksheets)**

データセットのワークシートで作業する際、下のスクリーンショットのように見えます。このビューは、列の操作をすぐに始めるための2つの方法を提供します：ワークシートのスプレッドシートと列ビューパネルです。これら2つのコンポーネントのいずれかから変更が加えられると、あなたの列はもう一方でも自動的に更新されます。
<img width="3584" height="1968" alt="3b0459e-dataset-worksheet" src="https://github.com/user-attachments/assets/3e47194b-2015-4185-865e-5d337ef38ea4" />

* **スプレッドシートインターフェース (The spreadsheet interface)**
    ワークシートのスプレッドシートインターフェースは中央に配置され、インタラクティブなスプレッドシートのようなインターフェースを提供します。全ての列アクションは、このテーブルから列メニューを使用して開始できます。<img width="982" height="505" alt="image" src="https://github.com/user-attachments/assets/718a6ecc-50e2-4f38-aa06-b11c44ee3528" />

* **列ビューパネル (The column view panel)**
    列ビューパネルはワークシートの右側にあります。これはワークシートの列のハイレベルな編集可能ビューを表示します。このパネルを使用して列を検索し、データをレベルにグループ化します。スプレッドシートと同様に、各列には[列メニュー](#column-menus)もあります。<img width="973" height="476" alt="image" src="https://github.com/user-attachments/assets/034ba59d-d432-4de1-92d5-dc73f2f6ee94" />

**列の詳細 (Column details)**

Jsonを除く全てのワークシート列タイプで、列の詳細が利用可能です。個々の列の詳細と統計情報を表示するには、列メニューを開き、`Column Details...` を選択します。

モーダルの内容は列のタイプによって異なりますが、全体的な構造は一貫しています。<img width="819" height="490" alt="3a0aedc-26-column-details" src="https://github.com/user-attachments/assets/2f715091-7100-4b07-885c-91f9ab0af204" />

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
<img width="772" height="427" alt="image" src="https://github.com/user-attachments/assets/d222c4d6-fed9-440d-a0f2-aa38dbab01ee" />

* **列の名前変更 (Renaming columns)**
    列の名前を変更するには、列名をダブルクリックするか、列メニューから `Rename Column` を選択します。
    * Sigmaで列の名前を変更しても、データベースでの名前は変更されません。

* **列の説明の追加 (Adding column descriptions)**
    * **列メニューから説明を追加または編集するには：**
        1.  列メニューを開きます。
        2.  `Add Description` をクリックします。<img width="1255" height="833" alt="ac38dfe-28-column-description" src="https://github.com/user-attachments/assets/f3570534-5490-4573-b088-d7ba052dde57" />

        3.  テキスト入力ボックスに説明を入力します。
        4.  `Save` をクリックします。
    * **ワークシートツールバーから説明を追加または編集するには：**
        1.  列を選択します。
        2.  ワークシートツールバーの `description icon` をクリックします。
        3.  テキスト入力ボックスに説明を入力します。
        4.  `Save` をクリックします。

* **列の説明の表示 (Viewing column descriptions)**
    説明付きの列は、列ヘッダーの左上隅にある黄色いマーカーで識別できます。説明を表示するには、列ヘッダーにカーソルを合わせます。
<img width="257" height="280" alt="03cce34-29-view-column-description" src="https://github.com/user-attachments/assets/b484ee93-57b4-4a08-af64-01a5ab49528c" />

* **列の非表示と再表示 (Hide or unhide columns)**
    列は、列メニューの 'Hide Column' アクションを使用して非表示にできます。非表示の列はスプレッドシートには表示されません。しかし、列ビューパネルからは引き続き表示され、操作可能です。列ビューパネルでは、非表示の列は表示されている隣の列と比較して「グレーアウト」して表示されます。<img width="493" height="1257" alt="3c13e66-30-worksheet-column-menu" src="https://github.com/user-attachments/assets/053b2843-ad96-4c48-bf8b-b1413ee9bc3e" />

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
<img width="756" height="423" alt="image" src="https://github.com/user-attachments/assets/348e3607-3e71-4c7e-8705-6261130e1517" />

**列の作成と計算 (Creating and calculating columns)**

* **新しい列の追加 (Adding a New Column)**
    テーブルの中間に新しい列を挿入するには、新しい列を配置したい場所の直前にある列のメニューから `Add New Column` を選択します。
    テーブルの最後またはグルーピングレベルの最後の列として新しい列を追加するには、列ビューパネルの関連する `Add New Column` ボタンをクリックします。
<img width="598" height="1148" alt="d3ca22a-32-add-new-column" src="https://github.com/user-attachments/assets/eb1bd1b8-1868-447a-b3b6-bd8b22bdd9f1" />

* **数式バーを使用する (Use the formula bar)**
    数式バーは、ワークシートでのデータ計算の中心です。これはワークシートの上部、スプレッドシートの上、ツールバーの下にあります。
    数式バーの数式は、常にワークシートで選択されている列に属します。列が選択されていないか、複数の列が選択されている場合、数式は表示されません。
    新しい数式を計算するには、まず新しい列を追加します。次に、数式バーに数式を入力します。入力中に、オートコンプリートされた関数名や列名が提案されます。数式を完成させたら、Enterキーを押すか、数式バーの右にある緑色のチェックマークをクリックします。
    Sigmaの関数インデックスをご覧ください。

**レベルのグルーピングを操作する (Working with level groupings)**

* **データをグループ化する (Group your data):**
  1.  画面の右側で、グループ化したい列の名前を見つけます。その列を `Select Grouping Key` と書かれたボックスまでドラッグします。
  2. ワークシートの上部または側部にある列名の右側の矢印をクリックしてアクセスする列メニューを使用して、集計列を簡単に作成できます。集計列を作成すると、それは自動的に次のレベルのグループの下にネストされます。
    * *Holidayでグループ化し、売上データを合計する集計列を作成すると、新しい列はHolidayごとの総売上を表示します。*
  3．画面右側の列名リストからグループ化したい列の名前を探し、その列名を `Base Columns` リストの上にドラッグすると、新しいレベルを追加するオプションが表示されます。ワークシートには2つのレベルのデータグルーピングが表示されます。全てのグループレベルの下にデータの集計列を作成できます。

* **レベルを折りたたむ (Collapsing levels)**
    レベルを折りたたむと、必要なデータのみを表示するのに役立ちます。`Base Columns` ラベルの左にある二重矢印をクリックすることで、レベルを折りたたんだり展開したりできます。
<img width="758" height="434" alt="image" src="https://github.com/user-attachments/assets/ad4e686f-dea3-4c53-a168-01cc638363f3" />

**半構造化データを抽出する (Extract semi-structured data)**

SigmaがJSONまたはVariant列タイプを検出すると、列メニューのオプションに「Extract Columns」が表示されます。データが半構造化されており、「Extract Columns」オプションが表示されない場合は、型関数 `JSON` または `Variant` を使用して、Sigmaがデータの列をどのように解釈するかを変更できます。<img width="3584" height="1968" alt="2f108c1-39_-_json-data" src="https://github.com/user-attachments/assets/b21497f0-9df6-4eaa-80bb-cdb271e98674" /><img width="1639" height="1274" alt="2f67593-40_-_json-field-extract-modal" src="https://github.com/user-attachments/assets/f2b536a1-265c-4e29-836a-2636f6df22f7" />


#### 3-5-4-3. データセットの合計 (Dataset Totals)

合計（Totals）は、ワークシートの最上位レベルに存在する、単一値の列集計です。合計は、ワークシートの右側パネルにある列ビュータブの下で作成できます。計算された合計値は、その後ワークシートの[コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls)に表示されます。

**合計を作成する (Create a Total)**

1.  ワークシートの右側パネルにある**列ビュータブ**を開きます。<img width="487" height="1027" alt="49e2dbc-45-totals-right-inspector" src="https://github.com/user-attachments/assets/6cb39147-1e88-48b0-b811-477500215a58" />

2.  `TOTALS` セクションの下にある `New Total...` をクリックします。
3.  リストから列を選択して、推奨される集計合計を自動的に作成します。または、`Add Empty Column` を選択して、独自の数式を記述します。
    * この例では、`[Sales Amount]` 列を選択します。これにより、`Sum([Sales Amount])` という数式を計算する新しい列 `[Sales Amount - Sum]` が自動的に作成されます。
    その列は右側の `TOTALS` リストに表示され、その数式は数式バーでアクセス可能になり、計算された値はコントロールパネルの `TOTALS` リストの下に表示されます。<img width="3584" height="1968" alt="966e943-46_-_new_total" src="https://github.com/user-attachments/assets/1d95b341-4853-4d6e-8444-1570c95fdec6" />

#### 3-5-4-4. データセットのフィルター (Dataset filters)

フィルターを使用すると、特定の条件を満たす行のみを表示するようにデータを制限できます。Sigmaのワークシートフィルターは、データセットワークシートの左側パネルに直接配置されているコントロールパネル内にあります。この配置により、フィルターの値を変更しながら、同時にデータがリアルタイムで応答するのを見ることができます。

**ユーザー要件 (User requirements)**

データセットでフィルターを使用するには、`Create, edit, and publish datasets` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。

**フィルターの構成要素 (Anatomy of a filter)**

* **コントロールパネル (Control panel)**
    フィルターは、データセットワークシートタブの左側にあるワークシートコントロールパネル内にあります。このパネルには、ワークシートの合計（Totals）とパラメータも含まれます。<img width="1274" height="710" alt="15ae7b2-47_-_filters-left-inspector" src="https://github.com/user-attachments/assets/7db8610e-83a1-4ff4-ab0b-a228c8a34740" />

* **フィルターリスト (Filter list)**
    既存のすべてのフィルターは、コントロールパネルの `FILTERS` ヘッダーの下で利用できます。無効化されたフィルターはグレーアウトされます。
<img width="407" height="323" alt="584aef8-48_-_disabled-filter" src="https://github.com/user-attachments/assets/db5e3d7d-a9f8-4d1f-b535-d31a75b77302" />

* **フィルター (Filter)**
    すべてのフィルタータイプは、フィルターリストに表示される際に同じ基本構造を持っています。
    以下は「Include」フィルターと「Range」フィルターの構成要素です。
<img width="197" height="84" alt="4df978b-50_-_filter-56" src="https://github.com/user-attachments/assets/f44ca67d-8054-4395-a5b6-fea3ab2ad1c4" />

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
<img width="197" height="92" alt="8fd531d-51_-_filter7" src="https://github.com/user-attachments/assets/504e176d-c0c2-4f2b-b437-4d3e9815e07c" />

**フィルターモーダル (The Filter Modal)**

フィルターモーダルを使用すると、SigmaのCreatorはフィルターを作成および編集できます。モーダルのフィールドオプションは、選択した列タイプとフィルタータイプによって異なります。
コントロールパネルのフィルターで直接値を選択する場合とは異なり、フィルターモーダルでの値の選択は、`Save` をクリックした後にのみワークシートデータに適用されます。
<img width="426" height="366" alt="344c926-52_-_filter-modal" src="https://github.com/user-attachments/assets/862c1f25-c8da-46e6-88e9-e1d5a8e904cf" />

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
    1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)がまだ開いていない場合は、折りたたまれたCONTROLSバーまたはワークシートツールバーの `Show Controls` ボタンをクリックして開きます。<img width="1449" height="545" alt="c2bbe1f-53_-_show-controls" src="https://github.com/user-attachments/assets/9c91b6ad-3095-49d8-9c40-6b242e44045e" />

    2.  パネルの `FILTERS` セクションの右側にある `+` アイコンをクリックします。<img width="1248" height="614" alt="1c7d692-54_-_add_new_filter" src="https://github.com/user-attachments/assets/ffd0e9fa-f58e-4e05-ad51-61e9cb85f724" />

    3.  `Add Filter` モーダルが画面に表示され、ワークシートからフィルターする列を選択するように求められます。
        ドロップダウンリストから `Column` を選択します。
        * *注：選択する列のタイプによって、続くステップが決まります。これは、フィルタータイプとフィルター値が列タイプに依存するためです。この例では、Text (abc) 列を選択します。*<img width="417" height="280" alt="f017774-55_-_new_filter_type_popup" src="https://github.com/user-attachments/assets/2b4b2661-a57f-4fcf-9aea-1d83e3f3f6c4" />

    4.  次に、ドロップダウンメニューから `Filter Type` を選択します。
        * *この例では、デフォルトの ‘Include Values’ フィルタータイプを使用します。*<img width="419" height="336" alt="aa1f101-56_-_filter_type_select" src="https://github.com/user-attachments/assets/9679425f-d2f0-432e-9e9a-ffffca6597c5" />

    5.  `Filter value` の下で、フィルターする値を選択します。
        * *IncludeとExcludeの両方のフィルタータイプは、カウントでランク付けされた値のリストを提供します。順序付けられたリストをスクロールするか、検索を使用して値を見つけて選択します。*<img width="420" height="357" alt="15fb580-57_-_include_values" src="https://github.com/user-attachments/assets/9275ada3-dc4c-45f6-b61b-c3ded2ad62fa" />

    6.  `Save` をクリックして新しいフィルターを保存します。
        * *新しいフィルターはワークシートコントロールパネルに表示され、ワークシートのスプレッドシートインターフェースと並行して選択した値を変更できます。*<img width="1252" height="704" alt="4d4aaa2-58_-_completed_filter_add" src="https://github.com/user-attachments/assets/e416c18f-fad7-4cf6-89f6-3543af01b165" />


* **列メニューからフィルターを作成する**
    1.  フィルターしたい列の[列メニュー](https://help.sigmacomputing.com/docs/dataset-worksheet-columns#column-menus)を開きます。
    2.  メニューから `Add Filter...` を選択します。
    3.  `Add Filter` モーダルが画面に表示され、列が選択され、デフォルトの `Filter Type` が設定されています。
        * *注：選択した列のタイプによって、続くステップが決まります。この例では、Numeric (123) 列を選択しました。*<img width="416" height="361" alt="0cb4258-59_-_range-filter" src="https://github.com/user-attachments/assets/b7fc56ac-3802-4574-be19-00e8665228ca" />

    4.  [任意] `filter type` を変更します。
        * *この例では、デフォルトの ‘Range’ フィルタータイプを使用します。*
    5.  `Filter value` の下で、フィルターしたい範囲を選択します。最小値と最大値の両方を指定するか、範囲の一端を開いたままにすることができます。<img width="417" height="365" alt="390bcfa-60_-_numeric_range_filter" src="https://github.com/user-attachments/assets/f3ce9d0a-9c98-4183-b85f-2b1a11ea21ca" />

    6.  値を選択した後、フィルターにnull値を含めるかどうかを選択できます。デフォルトではnullが含まれます。
    7.  `Save` をクリックして新しいフィルターを保存します。
        * *新しいフィルターはワークシートコントロールパネルに表示され、そこで選択した値を変更できます。*<img width="1059" height="757" alt="7cd9e6c-61_-_numeric_filter_complete" src="https://github.com/user-attachments/assets/b195855d-7e89-414c-bc89-7ca0e2556fb0" />


* **セルメニューからフィルターする**
    テーブルセルのコンテキストメニューを使用して、新しいinclude/excludeタイプのフィルターを作成したり、既存のものを変更したりすることが可能です。選択したセルの値でフィルターするには：
    1.  フィルターしたいセルを右クリックします。`cell menu` が開きます。
    2.  メニューから `Include` または `Exclude` を選択します。
        * *あなたの選択はワークシートに適用され、コントロールパネルの `Filters` リストに反映されます。*<img width="344" height="217" alt="c772da8-62_-_filter_from_cell" src="https://github.com/user-attachments/assets/aaa3a875-c69d-4e0f-a868-8526d98e5ff2" />


**フィルターの値の選択を変更する (Modify a filter’s value selection)**
コントロールパネルからフィルターの値の選択に加えられた変更は、自動的にワークシートのデータに適用されます。値選択の入力フィールドは、フィルタータイプに依存します。
![e1d3ec9-63-change-filter-value](https://github.com/user-attachments/assets/8e72314c-e0a2-4dcf-89b1-ae0ae4fcacd6)

**フィルターを編集する (Edit a filter)**
以下の手順は、「Edit Filter」モーダルを開く方法を示します。ここから、フィルターの構造的な詳細を編集できます。
変更は `Save` を押すまで行われません。
* **コントロールパネルからフィルターを編集する**
    1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
    2.  FILTERSリストで、編集したいコントロールにカーソルを合わせ、キャレットアイコンをクリックしてドロップダウンメニューを開きます。
    3.  `Edit Filter` をクリックします。
        * *「Edit Filter」モーダルが開きます。目的の変更を加えて `Save` をクリックします。*<img width="321" height="346" alt="413a412-64_-_edit_filter" src="https://github.com/user-attachments/assets/7ed4cca8-d030-426f-8426-0590eb1a791a" />


**フィルターを削除する (Delete a filter)**
以下の手順は、フィルターを永久に削除します。代わりに、[フィルターを一時的に無効にする](https://help.sigmacomputing.com/docs/dataset-filters#temporarily-disabling-a-filter)こともできます。
1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
2.  FILTERSリストで、削除したいフィルターにカーソルを合わせ、キャレットアイコンをクリックしてドロップダウンメニューを開きます。
3.  `Delete Filter` をクリックします。

**フィルターを一時的に無効にする (Temporarily disabling a filter)**
1.  [コントロールパネル](https://help.sigmacomputing.com/docs/dataset-worksheet-controls#opening-and-closing-the-control-panel)を開きます。
2.  `FILTERS` リストで、無効にしたいコントロールにカーソルを合わせます。
3.  青いトグルスイッチをクリックしてフィルターを無効にします。<img width="260" height="356" alt="5a50ce4-65_-_disable_filter" src="https://github.com/user-attachments/assets/988da6c9-9224-4831-a73f-2fa423f06e18" />

**フィルターの権限 (Filter permissions)**
SigmaのCreatorまたはAdminであれば、アクセス権のあるデータセットワークシートでフィルターを表示、作成、編集、削除できます。ただし、他のワークシートの変更と同様に、作業を公開するにはワークシートに対する編集権限が必要です。閲覧専用のアクセス権しかない場合は、ワークシートの変更を新しいワークシートとして保存できます。「[Data permissions](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。

#### 3-5-4-5. データセットのパラメータの作成と管理 (Create and manage dataset parameters)

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

Sigmaホームから、既存のデータセットを選択するか、新しいものを作成します。「[Create Datasets](https://help.sigmacomputing.com/docs/create-and-manage-datasets)」を参照してください。

データセットを表示する際、データセットの `Worksheet` タブを表示しているときに、左パネルでデータセットパラメータにアクセスします。
<img width="827" height="410" alt="b696725abe4e295e9794d875546667de5ce83e253c80c940d0998e3aa13d1bf6-dataset-parameters-sidebar" src="https://github.com/user-attachments/assets/9f02cbc1-f267-4f75-8b7b-5f04add675cd" />

左パネルでは、既存のすべてのデータセットパラメータが `Parameters` の下に表示されます。各パラメータについて、以下を確認できます。
* **Data type:** パラメータの値のタイプを表します。テキスト(abc)、数値(123)、日付(カレンダー)など。詳細は「[Supported data types and formats](https://help.sigmacomputing.com/docs/data-types)」を参照してください。
* **Parameter name:** パラメータの名前。
* **Parameter value:** パラメータの現在の値。データセットを編集する際、新しいパラメータ値を入力できます。パラメータの設定に応じて、リストから値を選択したり、テキストを入力したり、数値を入力したり、日付を選択したりできます。
* **Parameter menu:** パラメータを編集、複製、または削除するためのメニュー。メニューを開くには を選択します。このメニューはデータセットを編集中にのみ利用可能です。

**データセットパラメータを作成する (Create a dataset parameter)**

1.  データセットを開き、そのデータセットの `Worksheet` タブを開きます。
2.  `Edit` をクリックします。
3.  左のコントロールパネルがまだ開いていない場合は、ツールバーの `Show Controls` をクリックするか、`Controls` バーを選択して展開します。
4.  `Parameters` セクションで、`Add Parameter` をクリックします。<img width="295" height="107" alt="f361738-3" src="https://github.com/user-attachments/assets/a4de45fa-1dfe-4469-a2b0-2930f9ee5e9d" />
    Add Parameter` モーダルが開きます。<img width="759" height="550" alt="f6c91d6-4" src="https://github.com/user-attachments/assets/94c11c2c-b6bb-4481-af10-69db0b40e930" />
5.  `Parameter Name` に、パラメータの名前を入力します。
6.  (任意) 説明を追加します。
7.  パラメータの `Data Type` (Text, Number, Date) を選択します。
8.  `Suggested Values` オプションが、パラメータの入力タイプを決定します。以下のいずれかを選択します。
    * **All:** データ型に応じて、テキスト、数値、または日付の値にすることができます。
    * **List:** カスタムの値オプションのセット。ユーザーはリスト内の任意の値を選択できます。「[Use a list of values in a dataset parameter](#use-a-list-of-values-in-a-dataset-parameter)」を参照してください。
9. (任意) パラメータの `Default Value` を指定します。
10. (任意) 日付または数値のデータ型の場合、パラメータ値の `Format` を指定します。
11. `Save` をクリックします。

パラメータを作成した後、以下のいずれかの方法で使用できます。
* データセットワークシートの左の `Controls` パネルで、値を変更する。
* 新しいデータセット列など、数式でパラメータを参照する。「[Reference a dataset parameter in a formula in a dataset worksheet](#reference-a-dataset-parameter-in-a-formula-in-a-dataset-worksheet)」を参照してください。
* ワークブックコントロールの選択に基づいてパラメータの値を更新する。「[Parameters in Workbooks](https://help.sigmacomputing.com/docs/parameters-in-workbooks)」を参照してください。

**データセットパラメータで値のリストを使用する (Use a list of values in a dataset parameter)**

1.  [データセットパラメータを作成する](https://help.sigmacomputing.com/docs/create-and-manage-dataset-parameters#create-a-dataset-parameter)手順に従い、`Suggested Values` で `List` を選択します。
2.  (任意) 日付または数値のデータ型の場合、パラメータ値の `Format` を指定します。例えば、数値を通貨としてフォーマットします。
3.  `Values List` に、各値を追加します。表示フォーマットを定義した場合、`Display Value` はそのフォーマットを反映します。<img width="665" height="765" alt="3902776-6" src="https://github.com/user-attachments/assets/c146474a-449b-418b-b3a9-488b87ca8e0d" />

4.  (任意) `Default Value` ドロップダウンメニューで、リストから値の1つを選択します。
5.  `Save` をクリックします。

**データセットワークシートの数式でデータセットパラメータを参照する (Reference a dataset parameter in a formula in a dataset worksheet)**

ワークシートの列の数式で、データセットパラメータを名前で参照できます。数式はパラメータの値を使用し、パラメータの値が変更されると自動的に更新されます。

例えば、`Revenue` 列を持つデータセットに対して、`Min Sales Amount` パラメータを作成し、売上収益が最小販売額より大きいかどうかを評価する数式を計算することができます。
1.  データセットに新しい列を追加します。
2.  新しい列の数式バーに、角括弧で囲んだデータセットパラメータの名前を入力します。例： `[Min Sales Amount]`<img width="524" height="404" alt="f5c940b-7" src="https://github.com/user-attachments/assets/b43e88c1-9441-4415-ab69-99bfbdb7f775" />

3.  数式を反映するように列の名前を変更します。例： `Min Sales Param`
4.  パラメータリストで、パラメータの値を更新し、列の変更を観察します。<img width="550" height="554" alt="1d042f2-8" src="https://github.com/user-attachments/assets/43c1379e-7356-4178-8781-a72c66ab1004" />

5.  列の数式を変更して、計算でパラメータを使用します。例えば、列の各行の `Revenue` が `Min Sales Amount` パラメータ値より大きいかどうかを、数式 `[Revenue] > [Min Sales Amount]` を使用して評価します。
    * Sigmaは自動的に列のブール値（論理値）を計算します。
6.  パラメータリストで、パラメータの値を変更し、列のtrue/false値の変更を観察します。
    * 新しいパラメータ値を入力すると、計算列は自動的に更新されます。

**データセットパラメータでデータセットワークシートをフィルタリングする (Filter a dataset worksheet with a dataset parameter)**

データセットパラメータに基づいてデータセットワークシートをフィルタリングするには：
1.  パラメータを作成します。「[Create a dataset parameter](https://help.sigmacomputing.com/docs/create-and-manage-dataset-parameters#create-a-dataset-parameter)」を参照してください。
2.  列の数式でパラメータを参照します。「[Reference a dataset parameter in a formula in a dataset worksheet](#reference-a-dataset-parameter-in-a-formula-in-a-dataset-worksheet)」を参照してください。
3.  その列のフィルターを作成します。
    a.  列メニューから、`Add Filter` を選択します。
    b.  `Add Filter` モーダルで、フィルタータイプと、データセットでフィルターするフィルター値を選択します。例えば、True値のみを表示するように選択します。<img width="448" height="365" alt="3576ba4-10" src="https://github.com/user-attachments/assets/a7ca69e7-f396-493e-9aee-aa4071a23b4d" />

    c.  `Save` をクリックします。
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

#### 3-5-5-1. データセットでCSVを使用する (Using CSVs in Datasets)

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
2.  ドロップダウンメニューで `Dataset` を選択します。<img width="789" height="774" alt="3a17db6-1" src="https://github.com/user-attachments/assets/dee5e23e-ccff-480e-aa08-71ae20447061" />

3.  データソース選択ページが開きます。<img width="3584" height="1968" alt="ebb9e06-2" src="https://github.com/user-attachments/assets/65b130a3-fbe7-4740-8c80-18cb7ce4e5d0" />

4.  データソースとして `CSV` を選択し、アップロードページに移動します。<img width="3584" height="1968" alt="a3c07db-3" src="https://github.com/user-attachments/assets/38f5d11a-68b4-4c1d-95bf-6c1d9153a25e" />

5.  提供されたリストから `Connection` を選択します。選択した接続が、あなたのファイルがアップロードされるウェアハウスです。書き込みアクセスが有効なデータウェアハウスが一つしかない場合、それはデフォルトで選択されます。
6.  `File Upload` セクションで、ページにドラッグ＆ドロップするか、`Browse` をクリックしてCSVファイルをアップロードします。<img width="3584" height="1968" alt="2261f3c-4" src="https://github.com/user-attachments/assets/b459fa53-6327-44a7-af69-837b1ef173b0" />

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

#### 3-5-6. データセットのリネージ (Dataset Lineage)

ウェアハウステーブルとデータセットの「Lineage」タブでは、あなたのデータセットやウェアハウステーブルがSigma内のどこで使用されているか、そしてあなたのデータセットが依存している全てのソースを確認できます。これにより、特定のデータセットやウェアハウステーブルに変更を加えた場合に何が影響を受けるかを確認できます。

**データソース (Data sources)**

データソースはデータセットに表示されます。これは、あなたのデータセットによってデータのソースとして直接使用されているウェアハウステーブルとデータセットをリストアップしたものです。

**参照 (References)**

参照はテーブルとデータセットの両方に表示されます。これは、現在のテーブルまたはデータセットを下流でソースとして使用している全てのワークブックとデータセットをリストアップしたものです。

リネージを見ることで、以下のような疑問に答えることができます。
* この列はどこから来たのか？
* このデータはどのように計算されたのか？
* このデータセットを変更した場合、どのワークブックが影響を受けるか？
<img width="1791" height="381" alt="88f8d37-Screen_Shot_2021-10-19_at_2 14 00_PM" src="https://github.com/user-attachments/assets/596548a8-9eef-439e-819f-760559bfe52a" />

* #### 3-5-7. データセットの共有 (Share datasets)
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
2.  Sigmaが `Share Dataset` モーダルと共に開かれ、現在のアクセスリクエストを表示できます。任意で、権限ドロップダウンメニューをクリックして、ユーザーが持つべきアクセスレベルを選択します。<img width="797" height="550" alt="29cd3be-1" src="https://github.com/user-attachments/assets/3846581d-c51d-44d0-84b7-f9de124e6265" />

    * *注：ユーザーには、そのアカウントタイプが許可するよりも高いアクセス権を付与することはできません。*
3.  必要に応じて `Approve` をクリックします。`Approve` が選択されると、リクエストは `Share Dataset` モーダルから削除され、ユーザーは `Who Has Access` タブにリストされます。<img width="797" height="550" alt="29cd3be-1" src="https://github.com/user-attachments/assets/5b407c05-fc1e-4c12-ac1b-30c36bc9bb82" />

   または、`Deny` をクリックします。`Deny` が選択されると、リクエストは `Share dataset` モーダルから削除されます。<img width="797" height="550" alt="e5ef7ea-3" src="https://github.com/user-attachments/assets/7aaf4e6f-0c88-4ad9-9f5f-d34ccc417fec" />

4.  `Save` をクリックするか、`Share Dataset` モーダルを閉じます。コンテンツへのアクセスリクエストに関するあなたの決定は、どちらの方法でも保存されます。
<img width="797" height="550" alt="a77a964-4" src="https://github.com/user-attachments/assets/cb6e2222-a7d8-45ec-acc0-90ccee9bf441" />

  #### 3-5-8. データセットの列を構成する (Configure Dataset Columns)

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

5.  #### 3-5-8. データセットのリンク (Dataset Links)

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

#### 3-5-9. SQLからデータセットを作成する (Create a dataset from SQL)

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
4.  `Custom SQL` について、`More` > `Edit Source` を選択します。<img width="237" height="314" alt="c7f2e313d5fa0904b4898e4eef2e9b9896bb168a71b8074b3a1b1cc504b8fa8a-dataset-sql-edit" src="https://github.com/user-attachments/assets/429203f6-be29-44b2-9d8a-941673769749" />

5.  開いたクエリエディタで、カスタムSQLを修正します。`Run` をクリックして、クエリが期待通りの結果を返すことを検証します。
6.  `Done` をクリックしてクエリを保存します。
7.  `Publish` をクリックしてデータセットを更新します。

**既存のSigmaデータセットを参照する (Reference existing Sigma datasets)**

データプラットフォームに作成された[ウェアハウスビュー](https://help.sigmacomputing.com/docs/dataset-warehouse-views)の完全修飾名を使用して、既存のSigmaデータセットをSQLで参照できます。もしデータセットにロケーションまたはデータセットウェアハウスビューが利用できない場合は、作成してください。

完全修飾名は、データプラットフォーム内のデータセットのロケーションとウェアハウスビューの名前の組み合わせです。
`SELECT * FROM <location>.<dataset_warehouse_view_name>`

データセットの完全修飾名を特定するには、データセットを表示しているときに `More info` を選択します。
<img width="1194" height="522" alt="52cf6e5-Screenshot_2024-05-20_at_11 58 22_AM" src="https://github.com/user-attachments/assets/916f3743-d03c-48ed-961c-58a01bdce361" />

`Location` フィールドは、データセットを含むデータプラットフォーム内のデータベースまたはカタログとスキーマを提供し、`Dataset` フィールドは参照できるビュー名を提供します。

> 💡
> 完全修飾名をクリップボードにコピーするには、`More` () をクリックし、`Copy path` を選択します。

SQLステートメントでSigmaデータセットから個々の列を参照するには、列名を二重引用符で囲みます。例：
```sql SELECT "Customer Id" FROM DATABASE.SCHEMA.DATASET_WAREHOUSE_VIEW_NAME```


#### 3-5-10. データセットのウェアハウスビューの作成と管理 (Create and manage dataset warehouse views)

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

#### 3-6-1. サポートされるデータ型とフォーマット (Supported data types and formats)

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


#### 3-6-2. CSVデータのアップロード (Upload CSV data)

接続されたデータプラットフォームに保存されていないデータを分析するために、CSVデータをアップロードします。

**システムとユーザー要件 (System and user requirements)**

CSVデータをアップロードする機能には、以下が必要です。
* CSVデータをアップロードするために使用したい接続で、[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。
* [CSVアップロード機能](https://help.sigmacomputing.com/docs/enable-csv-uploads)があなたの組織で有効になっている必要があります。
* `Upload CSV` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/user-account-types)を割り当てられている必要があります。

**制限事項 (Limitations)**

CSV形式のファイルをアップロードするための最大ファイルサイズは200MBです。

**データはどこに保存されますか？ (Where's my data stored?)**

CSVファイルがSigmaにアップロードされると、ファイル内のデータは自動的に、書き戻しに使用されるスキーマ内に新しいテーブルとしてあなたのデータプラットフォームに書き込まれ、先頭に `sigma_df_csv` が付きます。あなたの組織に書き込みアクセスが有効な接続が複数ある場合、データを書き込む接続を選択するオプションが与えられます。

ワークブックにCSVファイルをアップロードした場合、あなたのファイル内のデータは、そのCSVファイルを使用するSigmaワークブックからのみアクセス可能です。接続のデータカタログでテーブルを閲覧する際に、CSVアップロードから作成されたテーブルは表示されません。そのワークブックを削除すると、CSVファイルのデータはもはやアクセスできなくなります。

> 💡
> CSVファイルを他のワークブックで再利用するには、代わりに[データモデルを作成](https://help.sigmacomputing.com/docs/get-started-with-data-modeling)してください。既にファイルをワークブックにアップロードしている場合は、[ワークブックのテーブル要素からデータモデルを作成する](https://help.sigmacomputing.com/docs/create-and-manage-data-models#create-a-data-model-from-a-workbook-table)こともできます。

**CSVファイルからワークブックを作成する (Create a workbook from a CSV file)**

1.  左のナビゲーションパネルで `+ Create New` をクリックし、`Upload CSV` を選択します。
2.  `Upload CSV` ページが開きます。<img width="329" height="447" alt="3a33d42-upload-csv" src="https://github.com/user-attachments/assets/4890dfbe-958c-4fc3-aa5d-e6ef26f347db" />

3.  ドロップダウンメニューから `Connection` を選択し、ファイルをアップロードするクラウドデータウェアハウスを指定します。
    * 書き込みアクセスが有効なデータウェアハウスが一つしかない場合、それはデフォルトで選択されます。
4.  `Upload CSV` セクションにファイルをドラッグ＆ドロップするか、`Browse` をクリックしてCSVファイルをアップロードします。<img width="1793" height="400" alt="cd185e9-3" src="https://github.com/user-attachments/assets/fa8118a0-556e-4c51-ab2a-f03df2373077" />

5.  データのプレビューが表示されます。
6.  データをプレビュー中に、警告やエラーに対処したり、その他の調整を行ったりできます。
    * [任意] ページの左側で、アップロードから除外したい列のチェックボックスをオフにします。
    * [任意] `Parsing Options` の下で解析オプションをカスタマイズします。
7.  ページの右上隅にある `Explore` をクリックして、データをワークブックで開きます。

**既存のワークブックにCSVファイルを追加する (Add a CSV file to an existing workbook)**

既存のワークブックがある場合、CSVファイルをデータ要素としてワークブックに追加できます。

* **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ページの右上隅にある `Edit` をクリックします。「[Workbook lifecycle](https://help.sigmacomputing.com/docs/workbook-lifecycle)」を参照してください。

1.  ワークブック内から、 を選択してワークブックの `Add new element` パネルを開きます。
2.  `Data elements` の下で、追加したい要素のタイプ（`Table`, `Visualization`, `Pivot table`）を選択します。
3.  要素のデータソースとして、`CSV` を選択してCSV形式のファイルをアップロードします。
4.  ドロップダウンメニューから `Connection` を選択し、ファイルをアップロードするクラウドデータウェアハウスを指定します。
    * 書き込みアクセスが有効なデータウェアハウスが一つしかない場合、それはデフォルトで選択されます。<img width="329" height="447" alt="3a33d42-upload-csv" src="https://github.com/user-attachments/assets/5b193a5d-ae15-4ce4-80b1-828fa56c7233" />

5.  `File Upload` セクションにファイルをドラッグ＆ドロップするか、`Browse` をクリックしてCSVファイルをアップロードします。
6.  データのプレビューが表示されます。<img width="1793" height="400" alt="cd185e9-3" src="https://github.com/user-attachments/assets/7d31a4ae-bae0-41ab-9d49-44610adc78d0" />

7.  データをプレビュー中に、警告やエラーに対処したり、任意で `Parsing Options` セクションで解析オプションをカスタマイズしたりできます。
8.  `Done` をクリックします。
    * 新しい要素がページに表示され、エディタパネルが特定の要素の構成ビューで開きます。

  #### 3-7-1. Joinタイプ (Join types)

**システム要件 (System requirements)**

ワークブックとデータセットにおけるJoin（結合）とLookup（ルックアップ）は、同じ接続からのソースを使用しなければなりません。

**SigmaにおけるJoinタイプ (Join types in Sigma)**

* **ルックアップ (Lookup)**
    ルックアップは、現在のデータのすべての行と、結合されたデータの一致する行からのすべてのデータを返します。現在のデータの一つの行に対して複数の一致が存在する場合、ルックアップはアスタリスク（*）を返し、現在のデータの行数を維持します。
    ルックアップは、ExcelのVLOOKUP関数のように機能します。詳細は、「[Lookup join](https://help.sigmacomputing.com/docs/join-data#lookup-join)」を参照してください。
<img width="477" height="362" alt="e738471-Lookup" src="https://github.com/user-attachments/assets/964f5e4e-5d04-472b-a48d-724bea0b0f70" />

* **内部結合 (Inner join)**
    内部結合は、現在のデータと結合されたデータの両方に一致するデータを含む行を返します。一致するデータを含まない行は省略します。
    詳細は、「[Inner join](https://help.sigmacomputing.com/docs/join-data#inner-join)」を参照してください。
<img width="477" height="362" alt="024edc4-Inner_Join" src="https://github.com/user-attachments/assets/c47c5773-d7f6-4757-a3be-5699232ee282" />

* **左外部結合 (Left outer join)**
    左外部結合は、現在のデータのすべての行と、結合されたデータの一致する行からのすべてのデータを返します。現在のデータの一つの行に対して複数の一致が存在する場合、結合は結合されたデータの各一致ごとに行を追加するため、行数が増加する可能性があります。
    詳細は、「[Left outer join](https://help.sigmacomputing.com/docs/join-data#left-outer-join)」を参照してください。
<img width="477" height="362" alt="4b3adca-Left_Outer_Join" src="https://github.com/user-attachments/assets/ffe13776-746f-4406-b349-063ea41d4ab8" />

* **右外部結合 (Right outer join)**
    右外部結合は、結合されたデータのすべての行と、現在のデータの一致する行からのすべてのデータを返します。結合されたデータの一つの行に対して複数の一致が存在する場合、結合は現在のデータ内のすべての一致する行を保持します。
    詳細は、「[Right outer join](https://help.sigmacomputing.com/docs/join-data#right-outer-join)」を参照してください。
<img width="477" height="362" alt="b835b2b-Right_Outer_Join" src="https://github.com/user-attachments/assets/89d3e86d-cb6b-4da2-a51d-fe3a480acb4f" />

* **完全外部結合 (Full outer join)**
    完全外部結合は、現在のデータのすべての行と、結合されたデータのすべての行を返し、該当する場合には一致する行を統合します。
    詳細は、「[Full outer join](https://help.sigmacomputing.com/docs/join-data#full-outer-join)」を参照してください。
<img width="477" height="362" alt="b355faf-Full_Outer_Join" src="https://github.com/user-attachments/assets/ca4e2687-1e18-47d4-a308-8d792ae4bc6e" />

#### 3-7-1-1. ルックアップ結合 (Lookup join)

このドキュメントはSigmaデータセットに関するものです。Sigmaワークブックについては、[`Lookup`関数](https://help.sigmacomputing.com/docs/lookup)および「[Add Columns through Lookup](https://help.sigmacomputing.com/docs/add-columns-through-lookup)」を参照してください。

> **重要:** すべての要素は、同じデータ接続上にある必要があります。
<img width="477" height="317" alt="945826b-Lookup" src="https://github.com/user-attachments/assets/b983e510-89b5-498d-bfc8-800504494895" />

ルックアップは、現在のデータのすべての行と、結合されたデータの一致する行からのすべてのデータを、現在のデータに行を追加することなく返します。複数の一致が存在する場合、Sigmaはアスタリスク（*）を表示して、結合されたデータに一致するデータを持つ行が複数あることを示します。ルックアップ結合は、ExcelのVLOOKUP数式と同様に機能します。

以下の例では、ルックアップを使用して顧客情報テーブルと注文情報テーブルを結合しています。結合キーとして、列CUST IDに示されている顧客IDを使用しています。注文テーブルには顧客ID 1からの注文が複数あるため、Sigmaは何らかの情報を引き出す代わりにアスタリスク（*）を表示します。これにより、顧客情報テーブルの行数が維持されます。

![Lookup Joinの例を示す図](https://help.sigmacomputing.com/hc/article_attachments/11266025219731)
<img width="707" height="439" alt="f0a7425-Lookup_table" src="https://github.com/user-attachments/assets/c397957b-98f3-4481-a5bd-b6337fdb216a" />

異なるJoinは、複数の一致する値を異なる方法で処理します。

| 一致数 | ルックアップ (Lookup) | 内部結合 (Inner join) | 左外部結合 (Left outer join) |
| :--- | :--- | :--- | :--- |
| 0 | NULL | 行を削除 | NULL |
| 1 | (値) | (値) | (値) |
| 2+ | * | 行を追加 | 行を追加 |


#### 3-7-1-2. 内部結合 (Inner Join)
<img width="719" height="323" alt="image" src="https://github.com/user-attachments/assets/9ab8a6dd-bf8e-483f-8de8-6d820ed00166" />

内部結合（Inner Join）は、現在のデータと結合されるデータの両方に存在する行を返します。現在のデータと結合されるデータの両方にデータがないすべての行を削除します。

以下の例では、内部結合を使用して顧客情報テーブルと注文情報テーブルを結合しています。結合キーとして、列CUST IDに示されている顧客IDを使用しています。両方のテーブルにデータがある行のみが保持されます。顧客ID 2、4、および6からのデータを持つ行は、元のテーブルのいずれか一方にしか存在しないため、結果のテーブルから削除されます。

![Inner Joinの例を示す図](https://help.sigmacomputing.com/hc/article_attachments/11266025340691)

異なるJoinは、複数の一致する値を異なる方法で処理します。

| 一致数 | ルックアップ (Lookup) | 内部結合 (Inner join) | 左外部結合 (Left outer join) |
| :--- | :--- | :--- | :--- |
| 0 | NULL | 行を削除 | NULL |
| 1 | (値) | (値) | (値) |
| 2+ | * | 行を追加 | 行を追加 |

#### 3-7-1-3. 左外部結合 (Left Outer Join)
<img width="477" height="362" alt="c89c21a-Left_Outer_Join" src="https://github.com/user-attachments/assets/d821ffbb-2252-49da-bcf7-3c3edf0572d6" />

左外部結合（Left Outer Join）は、現在のデータのすべての行と、結合されるデータの一致する行からのすべてのデータを返し、複数の一致がある場合には行を追加します。これにより、行数が増加する可能性があります。

以下の例では、左結合を使用して顧客情報テーブルと注文情報テーブルを結合しています。結合キーとして、列CUST IDに示されている顧客IDを使用しています。注文テーブルには顧客ID 1からの注文が複数あるため、その情報に対応するためにテーブルに追加の行が加えられます。テーブルには今、顧客1のデータを保持する行が2つあります。

![Left Outer Joinの例を示す図](https://help.sigmacomputing.com/hc/article_attachments/11266025430803)

異なるJoinは、複数の一致する値を異なる方法で処理します。
<img width="691" height="394" alt="8c7d132-LOJ_table" src="https://github.com/user-attachments/assets/88989d33-fc6e-4eba-a8fd-b236cbc3b52f" />

| 一致数 | ルックアップ (Lookup) | 内部結合 (Inner join) | 左外部結合 (Left outer join) |
| :--- | :--- | :--- | :--- |
| 0 | NULL | 行を削除 | NULL |
| 1 | (値) | (値) | (値) |
| 2+ | * | 行を追加 | 行を追加 |

#### 3-7-1-4. 右外部結合 (Right Outer Join)
<img width="477" height="311" alt="ec2f9e1-Right_Outer_Join" src="https://github.com/user-attachments/assets/f72ed949-1a13-4817-bc25-0740626d862c" />
右外部結合（Right Outer Join）は、結合されるデータのすべての行と、現在のデータの一致する行からのデータを返し、複数の一致がある場合には行を追加します。現在のデータに、結合されるデータに一致する行が複数ある場合、一致するすべての行が保持されます。

以下の例では、右結合を使用して顧客情報テーブルと注文情報テーブルを結合しています。結合キーとして、列CUST IDに示されている顧客IDを使用しています。結合される注文テーブルのすべてのデータが保持されます。注文テーブルに結合できない顧客情報テーブルのすべてのデータは削除されます。

顧客ID 2と4の顧客情報を示す行は、注文情報テーブルに対応するデータがないため削除されます。顧客ID 6の注文情報は、顧客情報テーブルには存在しなくても注文テーブルに存在するため、テーブルに追加されます。

![Right Outer Joinの例を示す図](https://help.sigmacomputing.com/hc/article_attachments/11266025514643)

#### 3-7-1-5. 完全外部結合 (Full Outer Join)
<img width="477" height="311" alt="ec2f9e1-Right_Outer_Join" src="https://github.com/user-attachments/assets/f80c78bb-3f81-45b6-9e1a-cb47fb8c87dc" />

完全外部結合（Full Outer Join）は、現在のデータのすべての行と、結合されるデータのすべての行を返し、可能な場合には一致させます。

以下の例では、外部結合を使用して顧客情報テーブルと注文情報テーブルを結合しています。結合キーとして、列 `[CUST ID]` に示されている `[Cust ID]` を使用しています。両方のテーブルのすべての行が、結合されたテーブルに追加されます。可能な場合は行が結合されます。それが不可能な場合は、行にnull値が追加されます。

結合された注文テーブルの複数の注文に対応するために、顧客1のデータの行が追加されます。顧客2と顧客4は、注文テーブルに彼らのデータがなかったため、注文データの値がNULLになります。顧客6は、元のデータに顧客6の情報がなかったため、First（名）とLast（姓）の値がNULLになります。

![Full Outer Joinの例を示す図](https://help.sigmacomputing.com/hc/article_attachments/11266050516115)
<img width="645" height="376" alt="0bcef43-ROJ_table" src="https://github.com/user-attachments/assets/8284ed2f-3ae1-4faf-a76d-dfeca5cdd6a8" />

#### 3-7-2-1. データセットでデータを結合する (Join data in datasets)

ウェアハウステーブルやデータセット間でJoin（結合）を作成する際、Joinを機能させるために入力列のデータを変更する必要がある場合があります。そのような場合、Joinを作成しながら入力列に数式を追加することができます。

Sigmaで利用可能な任意の関数を使用して、スカラー数式で結合キーを定義できます。数式は、単純な[型変更](https://help.sigmacomputing.com/docs/type-functions)関数から、複雑な[If](https://help.sigmacomputing.com/docs/if)ステートメントまで様々です。
<img width="445" height="430" alt="f61d09a-join_calc_col" src="https://github.com/user-attachments/assets/f43204f8-8087-4d02-9f0b-3821e37e8700" />

**Joinの入力列に数式を追加する (Add a formula to a join input column)**

1.  ワークシートの右側で、`Data Sources` タブに移動します。
2.  `+` をクリックして、新しいJoinを追加します。
3.  データソースを選択します。
4.  Joinタイプを選択します。
5.  結合キーの下にあるドロップダウンメニューを開き、修正したい結合キーに対して `+ Add Formula` をクリックします。
6.  数式を入力します。
7.  プレビューがロードされるのを待って、選択した結合キーが期待通りにデータを結合していることを確認します。
8.  `Done` をクリックして、Joinの作成を完了します。

#### 3-7-2-2. ワークブックでデータを結合する (Join data in workbooks)

Join（結合）は、一致する列に基づいて複数のソースからのデータを組み合わせます。

この記事では、例えば単一のデータ要素内で複数のソースからのデータを組み合わせることができるように、ワークブックでJoinを作成する方法について説明します。

Joinの詳細と、データを組み合わせるために使用したいJoinタイプの選択に関するガイダンスについては、「[Join types](https://help.sigmacomputing.com/docs/join-types)」を参照してください。

**データソースを結合する (Join data sources)**

* **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ページの右上隅にある `Edit` をクリックします。

1.  を選択して、ワークブックの `ADD NEW ELEMENT` パネルを開きます。
2.  `DATA ELEMENTS` の下で、追加したい要素のタイプ（`TABLE`, `VIZ`, `PIVOT TABLE`）を選択します。
3.  `Join` または `Union` を選択して、データソースを組み合わせます。
4.  表示された `Select source` ダイアログで、データソースまたは現在のワークブック要素を検索するか、ワークブック要素、テーブル、またはデータセットを参照します。
    データソースを選択してプレビューし、選択する列を選んでから `Select` をクリックします。
5.  `Create Join` ページが開きます。
    * Joinには2つ以上のソースが必要です。
<img width="1536" height="825" alt="c0a772e-5" src="https://github.com/user-attachments/assets/0be8f885-31f0-4ec1-87a4-0761cd3491ab" />
6.  2番目のソースを追加するには、`SOURCES` の隣にある `+` をクリックします。<img width="1536" height="825" alt="c0a772e-5" src="https://github.com/user-attachments/assets/97422541-ffd0-44a3-adb4-6e4c550d866c" />

7.  ステップ4と5を繰り返します。<img width="1536" height="827" alt="8b2acdd-6" src="https://github.com/user-attachments/assets/cd25f975-5fee-423e-8254-ebc6fa75bfca" />

8.  `Join type` を選択します。<img width="1536" height="827" alt="8b2acdd-6" src="https://github.com/user-attachments/assets/9bf18a48-304e-4371-97ff-82178da2da48" />

9. 使用する `Join keys` を選択します。ページの右側には、選択した結合キーの一致率が表示されます。<img width="1536" height="824" alt="2b9c70e-7" src="https://github.com/user-attachments/assets/58d24fdd-7026-45ea-9b5a-687a4de66648" />
    > 📘
    > 場合によっては、[完全外部結合](https://help.sigmacomputing.com/docs/full-outer-join)のように、複数の結合キーのペアを定義したいことがあります。
10. [任意] 別のソースを結合するには、ステップ6〜9を繰り返します。
11. `Preview output` を選択します。
12. 結合されたデータソースのプレビューを確認し、含まれる列に必要な変更を加えます。
    <img width="1536" height="824" alt="b7462c7-9" src="https://github.com/user-attachments/assets/80b9afba-7f6f-4452-80cd-21ecdb3fd0b4" />
13. `Done` を選択します。
    * 新しい要素がワークブックに表示されます。
   
#### 3-8-1. カスタム日時フォーマットを定義する (Define custom datetime formats)

Sigmaでは、カスタム日時フォーマットを定義して、ワークブック内で[日付データ](https://help.sigmacomputing.com/docs/supported-data-types-and-formats#date)がどのように表示されるかを制御できます。

このドキュメントでは、カスタムフォーマット文字列の概要と、それらを使用してカスタム日付フォーマットを表示する方法について説明します。

> 📘
> このドキュメントは、Sigma UIでのカスタム日時フォーマットに特化しています。関数でサポートされている日時フォーマットについては、「[DateFormat](https://help.sigmacomputing.com/docs/dateformat)」および「[DateParse](https://help.sigmacomputing.com/docs/dateparse)」を参照してください。

**ユーザー要件 (User requirements)**

カスタム日時フォーマットを定義するには、あなたがワークブックの所有者であるか、`Can explore` のワークブック権限を付与されている必要があります。

**カスタムフォーマット文字列 (Custom format strings)**

カスタムフォーマット文字列は、個々の[フォーマット指定子](https://help.sigmacomputing.com/docs/define-custom-date-formats#common-format-specifiers)と、文字、数字、記号を含む複数の指定子や文字の組み合わせをサポートします。

例えば、以下の表は、値 `2018-07-08 00:34:59` に適用された3つの異なるカスタムフォーマット文字列の出力を示しています。

| カスタムフォーマット文字列 | 出力 |
| :--- | :--- |
| `%a, %b %d, %Y` | Sun, Jul 08, 2018 |
| `%Y-Q%q` | 2018-Q3 |
| `%I:%M:%S %p` | 12:34:59 AM |

**一般的なフォーマット指定子 (Common format specifiers)**

以下の表は、一般的に使用されるフォーマット指定子を定義しています。サポートされている指定子の完全なセットについては、[`d3-time-format`モジュール](https://github.com/d3/d3-time-format)を参照してください。

| フォーマット | 説明 | 出力例<br>(`2018-07-08 00:34:59`の場合) |
| :--- | :--- | :--- |
| `%Y` | 4桁の年 | 2018 |
| `%y` | 2桁の年 | 18 |
| `%q` | 四半期 (1–4) | 3 |
| `%m` | 2桁の月 | 07 |
| `%B` | 完全な月名 | July |
| `%b` | 短縮形の月名 | Jul |
| `%A` | 完全な曜日名 | Sunday |
| `%a` | 短縮形の曜日名 | Sun |
| `%d` | 2桁の日 (01-31) | 08 |
| `%H` | 24時間制の2桁の時 (00–23) | 00 |
| `%I` | 12時間制の2桁の時 (01–12) | 12 |
| `%M` | 2桁の分 (00–59) | 34 |
| `%S` | 2桁の秒 (00–59) | 59 |
| `%p` | AM または PM | AM |
| `%L` | 3桁のミリ秒 (000–999) | 000 |
| `%f` | 6桁のマイクロ秒 (000000–999999) | 000000 |
| `%Z` | タイムゾーンオフセット | -07:00 |
| `%%` | パーセント記号 | % |

**カスタム日時フォーマットを定義する (Define a custom datetime format)**

1. 以下のいずれかの方法を使用して、`Custom Format` モーダルにアクセスします。
* **列メニュー:** フォーマットしたい列のヘッダーで、キャレット()をクリックして列メニューを開き、`Format` > `Custom` を選択します。<img width="1152" height="823" alt="aad14f9-image" src="https://github.com/user-attachments/assets/fc1f7d69-2819-4529-a6d8-9d0d32d054b6" />

* **ツールバー:** フォーマットしたい列を選択し、ワークブックツールバーの `Format` オプションをクリックして `Custom date` を選択します。
<img width="1152" height="699" alt="5420bd8-image" src="https://github.com/user-attachments/assets/4159eea2-1318-4899-80da-02bf2a864d0b" />

2. `Custom Format` モーダルで、フォーマット文字列を入力し、`Example` フィールドが表示したい日時フォーマットを反映していることを確認します。

必要に応じてフォーマット文字列を調整し、`Apply` をクリックします。列は即座にカスタム日時フォーマットを反映します。

#### 3-8-2. 構造化オブジェクトの生成とアクセス (Generate and access structured objects)

レコード数式は、ワークブックやデータモデルで直接、構造化オブジェクト（JSONなど）を生成することを可能にし、データ処理とインタラクションを改善します。

Sigmaが構造化オブジェクトを処理する際、個々のフィールドのデータ型を保持し、型の制約を強制します。この慣行はデータの整合性と正確性を保証すると同時に、型変換を行うことなくオブジェクトの値を簡単にアクセス・操作することを可能にします。

このドキュメントでは、レコード数式を紹介し、構造化オブジェクトを生成・アクセスする方法を説明します。

> 📘
> レコード数式は、BigQuery, Databricks, MySQL, PostgreSQL, Redshift, および Snowflakeでサポートされています。

**ユーザー要件 (User requirements)**

ワークブックやデータモデルで構造化オブジェクトを生成・アクセスするには、あなたがドキュメントの所有者であるか、`Can explore`（ワークブックにのみ適用）または `Can edit` のドキュメント権限を付与されている必要があります。

**レコード数式を使用して構造化オブジェクトを生成する (Use record formulas to generate structured objects)**

レコード数式は、テーブル、ピボットテーブル、入力テーブル、およびビジュアライゼーションに追加された計算列で構造化オブジェクトを生成できます。以下のサブセクションで詳述する数式構文を適用して、構造化オブジェクト内のデータ型を正確に定義してください。

* **レコード数式の構文 (Record formula syntax)**
    数式バーで、以下の構文を使用してレコード数式を構築します。
    `{ key1: value1, key2: value2, key3: value3, ... }`
    キー/値のペアはいくつでも指定できます。ここで、キーコンポーネントはオブジェクトフィールドを識別する定数であり、値コンポーネントは、サポートされているデータ型を表す[定数](https://help.sigmacomputing.com/docs/generate-and-access-structured-objects#value-format-for-constants)または列、コントロール要素、関数を参照する[他の式](https://help.sigmacomputing.com/docs/generate-and-access-structured-objects#value-format-for-other-expressions)です。

* **定数の値フォーマット (Value format for constants)**
    定数値を割り当てると、Sigmaは[型推論](https://en.wikipedia.org/wiki/Type_inference)を使用してテキスト、数値、論理データ型を認識し、日付とバリアントのデータ型を識別するためには明示的な関数呼び出しに依存します。
    以下の表は、特定のデータ型を定義するために定数値をどのようにフォーマットするかを説明しています。

| データ型 | 値フォーマット | 例 |
| :--- | :--- | :--- |
| Text | 二重引用符で囲まれたテキスト文字列 | `{ name: “Jane Doe” }` |
| Number | 数値（整数または浮動小数点） | `{ employeeId: 2865 }` |
| Logical | キーワード `true` または `false` | `{ isActive: true }` |
| Date | 二重引用符で囲まれ、`Date`関数の引数として渡される日付文字列 | `{ startDate: Date(“2024-04-15”) }` |
| Variant | 二重引用符で囲まれ、`Json`関数の引数として渡されるJSON文字列<br>(この表で詳述されている値フォーマット要件はJSON文字列内の値にも適用されます) | `{ location: Json({ city: "San Francisco", state: “CA”, zip: 94105}) }` |

* **他の式の値フォーマット (Value format for other expressions)**
    列、コントロール要素、または関数を参照する値を割り当てると、Sigmaは式のコンテキスト（例えば、関数の事前定義された戻り値の型）に基づいてデータ型を定義するために型推論を使用します。
    以下の表は、列、コントロール要素、および関数を参照する値をどのようにフォーマットするかを説明しています。

| 参照 | 参照フォーマット | 例 |
| :--- | :--- | :--- |
| Column | 角括弧で囲まれた列名 | `{ jobTitle: [Title] }` |
| Control element | 角括弧で囲まれたコントロールID | `{ lastReview: [Review-date] }` |
| Function | 必須の関数構文<br>（該当する関数ドキュメントを参照） | `{ daysEmployed: DateDiff("day", [Hire Date], Today()) }` |

**構造化オブジェクトの値にアクセスし、操作する (Access and manipulate structured object values)**

構造化オブジェクト内の特定のフィールドの値にアクセスし、操作するには、以下のドット記法を使用してパスアクセスを設定します。
`[Column Name].field`

Sigmaは構造化オブジェクト内のデータ型を保持するため、データにアクセスしたり、関数に値を渡したりする際に型変換を行う必要はありません。これは、[バリアントデータ](https://help.sigmacomputing.com/docs/supported-data-types-and-formats#variant)として処理され、同じ出力を得るために型変換が必要になる場合がある半構造化オブジェクトとは対照的です。

* **例：構造化 vs. 半構造化のパスアクセス**
* <img width="668" height="123" alt="ccdfc62-image" src="https://github.com/user-attachments/assets/a60a9aef-22cf-4bea-8e5f-66d9ab299d92" />

    * **シナリオ1：列Aに構造化オブジェクトが含まれる場合**
        例のテーブルでは、列Aに**テキストデータ**を格納する構造化オブジェクトが含まれています。列Bで "street"、"city"、"state" の値を単一のテキスト文字列に結合するには、型変換なしで以下の数式を使用できます。
        `Concat([Column A].street, ", ", [Column A].city, ", ", [Column A].state)`

    * **シナリオ2：列Aに半構造化オブジェクトが含まれる場合**
        もし列Aが代わりに半構造化オブジェクトを含んでいる場合、Sigmaはオブジェクトの値をバリアントデータとして処理します。値を列Bで単一のテキスト文字列に結合するには、値をテキストデータに変換してから `Concat` 関数に渡すために `Text` 関数を必要とする、以下の数式を使用する必要があります。
        `Concat(Text([Column A].street), ", ", Text([Column A].city), ", ", Text([Column A].state))`

#### 3-9-1. 行レベルのセキュリティを設定する (Set up row-level security)

行レベルのセキュリティ（RLS）は、データを閲覧している人の特性に基づいてデータへのアクセスを制限します。

Sigmaは、機密データを保護するために、RLSと[列レベルのセキュリティ（CLS）](https://help.sigmacomputing.com/docs/column-level-security)の両方をサポートしています。CLSが列内のすべての値をアクセス権のないユーザーから保護するのに対し、RLSは値に基づいて特定のデータ行を保護するために使用できます。

データモデルまたはデータセット内のテーブルに対してRLSを設定できます。

> 💡
> あなたの組織が接続にOAuthを使用している場合、データプラットフォーム内の既存のRLSルールはSigmaによって尊重されます。

Sigmaでは、以下に基づいてRLSを設定できます。
* ユーザー属性値（推奨）
* Sigma内のチームメンバーシップ
* ユーザーのメールアドレス

RLSを構成する際、2つのステップを実行します。
1.  RLSルールを持つ列を定義する。
2.  データを一致するようにフィルタリングする。

このアプローチはフィルターに依存しており、そのフィルターは適用先のテーブルを閲覧できる誰でも変更できる可能性があります。結果として、子要素と下流のデータソースのみが完全に保護されていると見なすことができます。データセットまたはデータモデルでRLSを構成すると、そのデータに依存するすべてのワークブックが保護されます。

**要件 (Requirements)**

RLSを設定したいドキュメントに対して、`Can Edit` または `Can Explore` の[アクセス権](https://help.sigmacomputing.com/docs/folder-and-document-permissions)を持っている必要があります。

**ユーザー属性で行レベルのセキュリティを構成する (Configure row-level security with user attributes)**

ユーザー属性を使用したRLSの設定が推奨されます。なぜなら、ユーザーとチームへのユーザー属性の割り当ては、RLSを制御する列の数式とは別に処理されるため、更新が容易だからです。ユーザー属性は、埋め込みのユースケースやカスタムSQLクエリでのRLSにも使用できます。

ユーザー属性でRLSを構成する前に、Sigmaでユーザー属性を作成し、関連するユーザーに割り当ててください。「[Configure user attributes](https://help.sigmacomputing.com/docs/user-attributes-snowflake)」を参照してください。

1.  保護したいデータモデルのテーブル、ワークブックのデータ要素、またはデータセットに、新しい列を追加します。
2.  新しい列の数式を以下の数式に設定します。`<attribute-name>` をRLSに使用するユーザー属性に、`[<column-name>]` を一致する値を含む列名に置き換えます。
    `CurrentUserAttributeText("<attribute-name>") = [<column-name>]`
    > 🚩
    > 属性値は列名と同じデータ型でなければなりません。例えば、テキストです。
    この数式は、属性値が行の値と一致する場合は `True` を、一致しない場合は `False` を評価します。
3.  新しい列にフィルターを追加して、`True` の値のみを表示するようにします。
4.  下流のユーザーにデフォルトで表示されないように、列を非表示にします。

詳細は、「[CurrentUserAttributeText](https://help.sigmacomputing.com/docs/currentuserattributetext)」を参照してください。

* **データモデルでのRLS (RLS in a data model)**
    データモデル内で、店舗地域別の売上データの `plugs_electronics` テーブルにRLSを設定したい場合：
    1.  `Region` という名前のユーザー属性を作成し、利用可能な様々な地域の値を異なる営業チームに割り当てます。
        * Sales US-West には値 West を割り当て
        * Sales US-East には値 East を割り当て
    2.  データモデルで、`plugs_electronics` テーブルを追加し、次に `Region RLS` という新しい列を追加します。
    3.  `Region RLS` 列の数式を以下のように設定します。
        `CurrentUserAttributeText("Region") = [Store Region]`
        あなたはSales US-Westチームのメンバーであるため、`Region RLS` 列は `Store Region` が `West` である行に対して `True` 値を表示します。<img width="1035" height="530" alt="226323e2b44bb82c5ceb714d467e6f4936828e7cf44fc1a445ae103b2f9cc970-rls-formula" src="https://github.com/user-attachments/assets/4e4a385a-3329-4a5c-8aaf-4820d26c1b63" />

    4.  `Region RLS` 列にフィルターを追加し、`True` の値のみを表示します。<img width="355" height="266" alt="0d66893348deae35468f8ed4aded7c90770b7e0ed01a5b613032983605e171a6-rls-filter" src="https://github.com/user-attachments/assets/7017c83b-c680-4a6f-a489-c9aa1db220bf" />

    5.  [任意] 下流のユーザーにデフォルトで表示されないように、`Region RLS` 列を非表示にします。

* **埋め込み分析でのRLS (RLS with embedded analytics)**
    Sigmaを埋め込む場合、埋め込みURLのパラメータまたはJWTクレームでRLSを強制できます。
    * [Embed URL parameters](https://help.sigmacomputing.com/docs/embed-url-parameters)
    * [Create an embed API with JSON Web Tokens](https://help.sigmacomputing.com/docs/example-embed-api-and-url#create-an-embed-api-with-json-web-tokens)

* **カスタムSQLでのRLS (RLS with custom SQL)**
    ユーザー属性を正常に構成した後、SQLを実行しているユーザーのユーザー属性に基づいてSQLクエリの結果をフィルタリングできます。
    例：
    ```sql
    SELECT
      *
    FROM
      EXAMPLES.PLUGS_ELECTRONICS.PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA
    WHERE 
      {{system::CurrentUserAttributeText::store_region}} = STORE_REGION
    ```
    このクエリは `CurrentUserAttributeText` 関数を使用して、クエリを実行しているユーザーのユーザー属性の割り当て値を取得します。この関数は、ユーザー属性名を参照するパラメータを必要とします。
    > 📘
    > ユーザー属性名にスペースが含まれている場合は、二重引用符を使用してください。例：
    > `{{system::CurrentUserAttributeText::"Store Region"}} = STORE_REGION`
    詳細は、「[Write custom SQL](https://help.sigmacomputing.com/docs/write-custom-sql)」を参照してください。

**チームで行レベルのセキュリティを構成する (Configure row-level security by team)**

`CurrentUserInTeam` 関数を使用して、チームメンバーシップによってRLSを構成できます。
1.  保護したいデータモデルのテーブル、ワークブックのデータ要素、またはデータセットに、新しい列を2つ追加します。
2.  一つの新しい列の数式を、`Switch` または `If` 関数を使用して、データ内の値をSigmaチーム名に関連付ける数式に設定します。
3.  もう一方の新しい列の数式を、RLSルールを設定するために以下の数式に設定します。
    `CurrentUserInTeam([Team Assignment])`
    この数式は、現在のユーザーが `Team Assignment` 列で指定されたチームの一つ以上のメンバーである場合に `True` を評価します。
4.  新しい列にフィルターを追加して、`True` の値のみを表示するようにします。
5.  下流のユーザーにデフォルトで表示されないように、列を非表示にします。
詳細は、「[RLS by team example](#rls-by-team-example)」を参照してください。

* **チームによるRLSの例 (RLS by team example)**
    チームによってRLSを設定するには、データを関連するSigmaチームに関連付ける `Team Region` という列をデータに作成します。例えば、データに `Store Region` 列があり、Sales US-WestとSales US-Eastという2つのSigmaチームがある場合、`Switch` 関数を使用して数式を記述します。
    `Switch([Store Region], "West", "Sales US-West", "East", "Sales US-East")`
    このロジックをテストしたい全てのチームを含むように拡張し、次に、現在のユーザーが `Team Region` 列の対応する行に示されているチームに属しているかどうかを評価するRLSルールを持つ `Team RLS` 列を作成します。
    `CurrentUserInTeam([Team Region])`
    その後、`Team RLS` 列にフィルターを追加して `True` の値のみを表示し、`Team RLS` と `Team Region` の列を非表示にすることができます。

**ユーザーで行レベルのセキュリティを構成する (Configure row-level security by user)**

`CurrentUserEmail` 関数を使用して、ユーザーによってRLSを設定できます。
1.  保護したいデータモデルのテーブル、ワークブックのデータ要素、またはデータセットに、新しい列を追加します。
2.  RLSに使用する一人以上のユーザーを含む、新しい列の数式を以下の数式に設定します。
    `[<column-name>] = CurrentUserEmail()`
    この数式は、現在のユーザーが指定されたチームの一つ以上のメンバーである場合に `True` を評価します。
3.  新しい列にフィルターを追加して、`True` の値のみを表示するようにします。
4.  下流のユーザーにデフォルトで表示されないように、列を非表示にします。

* **ユーザーによるRLSの例 (RLS by user example)**
    売上結果のテーブルがあり、各営業担当者に自分の結果のみを表示させたい場合は、ユーザーによって行レベルのセキュリティを設定します。このアプローチを使用するには、Sigmaユーザーのメールアドレスを含む列をデータに作成または特定する必要があります。列を作成する必要がある場合は、サンプル構文のマッピングデータ値について「[RLS by team example](#rls-by-team-example)」を参照してください。
    この例では、データにSigmaユーザーが使用するメールアドレスと一致する `Salesperson Email` という列が含まれていると仮定します。
    RLSルールを評価するために、以下の数式で `Salesperson RLS` という新しい列を追加します。
    `[Salesperson Email] = CurrentUserEmail()`
    この数式は、`[Salesperson Email]` 列のメールを評価し、現在データを閲覧しているユーザーのメールと一致するかどうかを確認します。この数式は、現在のユーザーのメールが営業担当者のメールと一致するすべての行に対して `True` を返します。
    その後、`Salesperson RLS` 列にフィルターを追加して `True` の値のみを表示し、`Salesperson RLS` 列を非表示にすることができます。

* **チームとユーザーによるRLSの例 (RLS by team and user example)**
    複数の条件をテストするためにフィルターを設定することもできます。例えば、営業担当者には彼らが所有するリードからのデータのみを表示し、営業マネージャーにはすべてのデータを表示するようにデータをフィルタリングする列を追加します。
    `( [Salesperson Email] = CurrentUserEmail() ) or ( CurrentUserInTeam(“Sales Manager”) )`
    この数式は、閲覧者が "Sales Manager" チームにいる場合はすべての行に対して `True` を返し、他のすべての閲覧者に対しては、閲覧者のメールが営業担当者のメールと一致する行に対してのみ `True` を返します。

  #### 3-9-2. 列レベルのセキュリティを構成する (Configure column-level security)

データモデルまたはデータセット内の列レベルのデータへのアクセスを制限またはマスキングするために、列レベルのセキュリティを構成します。CLSを使用することで、あなたの組織はデータへのアクセスを管理し、機密情報が安全で、承認されたユーザーのみがアクセスできるように保証できます。

データのモデリング方法に応じて、異なる方法で列レベルのセキュリティを強制できます。
* データモデルの場合、[チームとユーザーでCLSを強制します](https://help.sigmacomputing.com/docs/column-level-security#configure-column-level-security-in-a-data-model)。
* データセットの場合、[ユーザー属性でCLSを強制します](https://help.sigmacomputing.com/docs/column-level-security#configure-column-level-security-in-a-dataset)。

**ユーザー要件 (User requirements)**

* ユーザー属性を作成し、チームを管理するには、`Admin` アカウントタイプを割り当てられている必要があります。
* データモデルで列レベルのセキュリティを構成するには、そのデータモデルに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-data-model)を付与されている必要があります。
* データセットで既存のユーザー属性を参照するには、そのデータセットに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-dataset)を付与されている必要があります。

**列レベルのセキュリティを理解する (Understanding column-level security)**

Sigmaでは、列レベルのセキュリティはチームの割り当て、ユーザー属性、およびドキュメントの構成を通じて管理されます。データセットを使用する場合、列レベルのセキュリティを使用して、テーブル内の個々の列へのアクセスを異なる埋め込みクライアントに対して許可することができます。

列レベルのセキュリティの追加の利点には、以下が含まれます。
* **データプライバシー:** 社会保障番号、財務データ、医療記録などの個人識別子を含む機密情報を保護します。
* **データ共有とコラボレーション:** 制御されたデータ共有とコラボレーションを可能にします。組織は、データセット全体を公開することなく、選択した列を外部の関係者やパートナーと共有できます。
* **マルチテナント環境でのデータ機密性:** 複数のクライアントや組織が同じインフラを共有するマルチテナントシステムやクラウドベースの環境では、列レベルのセキュリティにより、各テナントのデータが他のテナントから隔離され、保護されることが保証されます。
* **データマスキングと匿名化:** データマスキングおよび匿名化技術と組み合わせることで、特定の承認されたユーザーが疑似または難読化された値で作業できる状態を保ちつつ、機密データを保護します。

**データモデルで列レベルのセキュリティを構成する (Configure column-level security in a data model)**

データモデルテーブルを下流で使用する一人以上のユーザーまたはチームに対して、列へのアクセスが制限されているかどうかを指定することにより、データモデルの列レベルのセキュリティを構成します。列レベルのセキュリティをより簡単に管理するために、Sigmaは列へのアクセスを制限したいユーザーのグループごとにチームを作成することを推奨します。

ユーザーが保護された列へのアクセスを許可されていない場合、データモデルをデータソースとして使用する際に、その列は表示も選択もできません。下流のユーザーが利用できるが、デフォルトでは追加（インクルード）されないように列を作成するには、データモデルテーブルでその列を非表示にします。

1.  編集のためにデータモデルを開きます。
    > 💡
    > `Modeling` タブから、またはテーブルの列メニューから列レベルのセキュリティルールを追加できます。列メニューから追加するには、テーブルまたは`Properties`タブで列を探し、キャレット()を選択して `Column security...` を選択します。
2.  列レベルのセキュリティルールを適用したいテーブルを選択します。
3.  エディタパネルで、`Modeling` タブを選択します。<img width="262" height="295" alt="fb00b50ef05201d905b7fcc5fff3221f32abab3aca016be6ef7a864e77a7e85d-dm-cls-modeling" src="https://github.com/user-attachments/assets/f5bf09c2-1474-4364-99ea-51243fb8e325" />

4.  `Column security` セクションで、`+` (Add column level security...) を選択して、列レベルのセキュリティルールを追加します。
5.  新しいルールが表示され、`Add new column security` のポップオーバーが開きます。
6.  `Restricted columns` で、アクセスを制限する一つ以上の列を選択します。
    > 📘
    > グループ化された列には列レベルのセキュリティルールを設定できません。
7.  `Criteria` で、`No one can view`（全員のアクセスを制限）と `Specific users and teams`（許可リストを作成し、指定したユーザーとチームにのみアクセスを許可）のいずれかを選択します。<img width="384" height="331" alt="1e647b6f4835c9e8422b379715dbf7d6cbd1e3c3cf4ed5f880a66b01623f349a-dm-cls-add" src="https://github.com/user-attachments/assets/26b71b5e-6ae5-40cb-9fbd-e80e4d358e9d" />

8.  `Specific users and teams` を選択した場合、列へのアクセスを許可したいユーザーとチームを検索します。デフォルトでは5つのユーザーとチームしかドロップダウンに表示されません。ユーザーまたはチームを選択すると、リストに表示されます。
9.  ルールが作成されます。`X` をクリックしてポップオーバーを閉じます。
10. `Publish` をクリックしてデータモデルを更新し、列のセキュリティルールを即座に強制します。
    > 📘
    > 一人のユーザーと一つの列に複数のアクセス制限が適用される場合、制限はルールの和集合として適用されます。例えば、あるチームが列の閲覧を許可され、別のルールがその列へのアクセスを誰にも許可しない（誰も閲覧できない）場合、チームメンバーはその列を閲覧できます。

* **データモデルでのCLS構成例 (Example CLS configuration with a data model)**
    この例では、`Business Forecast` データモデルの収益データへのアクセスを、金融リーダーシップチームのSigmaユーザーのみに制限したいとします。この例では列メニューから列セキュリティルールを設定しますが、データモデルのERDから列レベルのセキュリティを設定することもできます。
    1.  まず、収益データへのアクセスを許可したいユーザーのためのチームを作成します。この例では、`Financial leadership` チームを作成します。財務リーダーをチームのメンバーとして追加します。
    2.  `Business Forecast` データモデルを編集用に開きます。
    3.  `Modeling` タブの `Column security` セクションで、`+` を選択して `Revenue` 列のルールを追加します。
    4.  `Restricted columns` で、`Revenue` を選択します。
    5.  `Criteria` で、`Specific users and teams` を選択し、`Financial leadership` チームを選択します。<img width="1359" height="569" alt="832873cf43f7469437262c3fb94c1e84dab36d34fc9c2164d6cee381f608b235-Screenshot_2025-03-26_at_11 09 58_AM" src="https://github.com/user-attachments/assets/46cd3a89-52fc-488f-b81c-f5b1274923c1" />

    6.  `Publish` をクリックしてデータモデルを更新します。
    金融リーダーシップチームの誰かは、データモデルをデータソースとして使用し、`Revenue` 列のデータを使ってワークブックを構築できます。<img width="1331" height="639" alt="fcba970d107814c6244f4bdcfefb224f41d56413ac59e6ca27bcfb8791869e08-Screenshot_2025-03-26_at_11 11 21_AM" src="https://github.com/user-attachments/assets/caba33b5-19c3-418c-9e8f-75dd87366d84" />
もしあなたが金融リーダーシップチームの一員でない場合、`Revenue` 列のデータにアクセスできないため、彼らのためにワークブックを作成することはできません。
    `Revenue` 列へのアクセス権がないあなたや他の誰かがそのデータを含むワークブックを閲覧しようとすると、列名が `Restricted` と表示され、その列の値は `No access` となります。
<img width="1187" height="536" alt="2ebe03e5ae6776f5f925fd78a7c0d747cf0d124744f7defce58c5e1f50c533dc-Screenshot_2025-03-26_at_11 12 16_AM" src="https://github.com/user-attachments/assets/6b0c358b-8d98-4689-959a-6a775a3dad6a" />

* **子要素は列レベルのセキュリティルールを継承する (Child elements inherit column-level security rules)**
    子要素は親要素から列レベルのセキュリティルールを継承します。フィルターのように、列レベルのセキュリティルールは列に適用されますが、子要素上で表示、修正、または管理することはできません。
    データモデル内で、他のデータモデル要素で制限された列を参照する場合、その列はCLSルールを継承し、制限されます。例えば、データモデル内で一つのテーブルから別のテーブルへのルックアップを作成し、ルックアップする列がCLSルールによって制限されている場合、ルックアップを介して追加された列も同じルールによって制限されます。

* **CLSで制限された列を数式で使用する (Using CLS-restricted columns in formulas)**
    列レベルのセキュリティルールで制限された列を使用して、メトリクスや計算列を作成できます。メトリクスと計算列は、参照された制限付き列からCLSルールを継承します。
    例えば、データモデルテーブルに制限された列 `Email` があり、メトリクスが各ドメインのメールアドレス数を計算する場合、制限されたユーザーはメトリクス名と定義（列名を含む）を表示できますが、ワークブックで使用するとメトリクスは制限されます（アクセス不可）。
    別の例として、データモデルテーブルに制限された列 `Name` があり、別の列 `Formatted Name` が数式 `Proper([Name])` を使用している場合、`Formatted Name` 列はCLSルールを継承し、同様に制限されます。

**データセットで列レベルのセキュリティを構成する (Configure column-level security in a dataset)**

データセットで列レベルのセキュリティを構成するには、以下を実行します。
1.  管理者ポータルで、[ユーザー属性を作成する](https://help.sigmacomputing.com/docs/user-attributes-snowflake#configure-user-attributes)か、既存のものを編集用に開きます。
    > 💡
    > 列レベルのセキュリティ用にユーザー属性を作成する場合、デフォルト値を定義してください。デフォルト値を指定しないと、Sigmaは自動的に属性値「2」をデフォルトとして割り当て、該当ユーザーの列データを制限します。
2.  列レベルのセキュリティ用に意図された以下の既存の割り当て値を使用して、[チームに属性値を割り当てます](https://help.sigmacomputing.com/docs/user-attributes-snowflake#assign-user-attributes)。

| 割り当て値 | 列レベルのセキュリティ結果 |
| :--- | :--- |
| 0 | 列データはデフォルトでワークブックに含まれる |
| 1 | 列データは利用可能だが、デフォルトではワークブックに追加されない |
| 2 | 列データはワークブックで利用不可（制限付き）|

3.  該当するデータセットを開くか[作成し](https://help.sigmacomputing.com/docs/create-and-manage-datasets)、チームにデータセットの[権限](https://help.sigmacomputing.com/docs/share-a-dataset)を付与します。割り当てられた権限タイプは、列レベルのセキュリティ設定に影響しません。
    > 🚧
    > 意図しない結果やエラーを防ぐため、マテリアライズされたデータセットでユーザー属性を使用することは避けてください。
4.  `Columns` タブを選択し、データセットヘッダーの `Edit` をクリックします。
5.  列レベルのセキュリティを構成したい列を探し、`Visibility` ドロップダウンをクリックして、該当するユーザー属性を選択します。<img width="1149" height="520" alt="5b88446-image" src="https://github.com/user-attachments/assets/73fbb32b-9608-449d-863e-baa19aabcbad" />

6.  列レベルのセキュリティが必要なすべての列に対してステップ5を繰り返し、データセットヘッダーの `Publish` をクリックして編集を保存します。

これで、列レベルのセキュリティを持つデータセットをデータソースとして使用する[ワークブックを作成](https://help.sigmacomputing.com/docs/workbook-fundamentals)できます。該当するチームとワークブックを共有すると、各ユーザーのチーム割り当て、ユーザー属性、および対応するデータセットの可視性構成に基づいて、データが含まれたり制限されたりします。

* **データセットでのCLS構成例 (Example CLS configuration with a dataset)**
    この例は、ユーザー属性とチームを使用して、データセットで列レベルのセキュリティを実装する方法を示します。
    あるSigma組織にはTeam AとTeam Bの2つのチームがあります。Team Aのメンバーは `Customer` という既存のデータセットの `Domain` 列へのアクセスが必要ですが、Team Bのメンバーはその同じデータの閲覧を制限される必要があります。
    1.  まず、データセキュリティを管理するためのユーザー属性を作成します。この例では、`Domain CLS` ユーザー属性を作成します。
    2.  Team Aに属性値 `0`（データにアクセスするため）を、Team Bに属性値 `2`（データを制限するため）を割り当てます。<img width="1149" height="575" alt="40c6111-image" src="https://github.com/user-attachments/assets/ca5842fd-1390-481b-9ade-b4c769cf0bb3" />

    3.  次に、Team AとTeam Bの両方のメンバーがデータセットにアクセスできることを確認します。`Customer` データセットを開き、`Permissions` タブを選択します。
    4.  次に、データセットの列の可視性を更新します。データセットの編集を開始するには、`Columns` タブを選択し、`Edit` をクリックします。
    5.  `Columns` タブで `Domain` 列を探し、対応する `Visibility` ドロップダウンフィールドをクリックして、`Domain CLS` ユーザー属性を選択します。<img width="1149" height="473" alt="8794788-image" src="https://github.com/user-attachments/assets/6c373d68-0ec7-42c9-a5b6-5bd7924fa4b9" />

        Team AとTeam Bに割り当てられた `Domain CLS` ユーザー属性の値が `Domain` 列に適用されます。<img width="1149" 

    6.  データセットへの変更を `Publish` して保存します。
    7.  データセットからワークブックを作成し、全てのデータセット列を持つテーブルを追加し、そのワークブックをTeam AとTeam Bの両方と共有します。
    Team Aのメンバーがワークブックを開くと、Sigmaは `Domain` 列の全てのデータを表示します。<img width="1198" height="210" alt="0497622-image" src="https://github.com/user-attachments/assets/c830a60b-3efa-4f8d-a1fd-86b0e0cd7b1e" />

    Team Bのメンバーがワークブックを開くと、Sigmaは `Domain` 列の名前を難読化し、代わりに `Restricted` と表示します。列の各行について、データが制限されているため、ユーザーは「No access」と表示されます。


##### 第4章：データ分析 (Analyze)

#### 4-1-1. ワークブックの概要 (Workbooks overview)

あなたがスプレッドシートに精通したアナリストであれ、ビジネスインテリジェンス（BI）ツールに慣れている方であれ、SigmaはスプレッドシートとBIツールの長所を一つの場所、つまり**ワークブック**に統合します。
* スプレッドシートのように、ワークブックはページを持ち、テーブルやピボットテーブルでデータを表示できます。![Uploading 0497622-image.png…]()

* BIツールのように、ワークブックはチャート、グラフ、インタラクティブなフィルターやコントロール、テーブル、テキスト、画像を含むダッシュボードのようなレイアウトを提供します。

ワークブックでは、データ探索や分析、複雑なビジュアライゼーションの構築、エクスポート用の詳細なレポートの準備などが可能です。ワークブックはまた、あなたの製品や組織のために[データアプリを構築](https://help.sigmacomputing.com/docs/intro-to-app-like-functionality)したり、[埋め込み分析を設計](https://help.sigmacomputing.com/docs/intro-to-embedded-analytics)したりするためのインターフェースも提供します。

このドキュメントでは、ワークブックの概念的な概要と、さらなるリソースへのリンクを提供します。

**ワークブックについて (About workbooks)**

ワークブックを作成することで、探索的分析を開始したり、エンタープライズグレードの分析を構築したり、データアプリを開発したりできます。Sigmaのほとんどすべてのことは、ワークブック内で行われます。
* [テーブルやピボットテーブル](https://help.sigmacomputing.com/docs/intro-to-tables)でデータを分析する。
* [チャートやマップ](https://help.sigmacomputing.com/docs/intro-to-charts)でデータを可視化する。
* 様々な宛先に[レポートをフォーマットしてエクスポート](https://help.sigmacomputing.com/docs/send-and-schedule-exports)する。
* 分析や開発について[同僚と共同作業](https://help.sigmacomputing.com/docs/collaborate-with-live-edit-in-workbooks)する。
* アクションでインタラクティビティを構築する。
* [テーマ](https://help.sigmacomputing.com/docs/custom-themes)、[コンテナ](https://help.sigmacomputing.com/docs/design-workbook-layouts)、[モーダル](https://help.sigmacomputing.com/docs/create-and-manage-modals)、その他の要素で[レイアウトやデザインをカスタマイズ](https://help.sigmacomputing.com/docs/design-workbook-layouts)する。
* その他多数…

**ワークブックの中身 (What's in a workbook)**

ワークブックには一つ以上のページが含まれます。モーダルやその他のアプリのような機能も、ワークブックのページのように表示されます。
各ワークブックのページやモーダルには、要素を配置できるキャンバスがあります。ページキャンバス上に要素を配置できます。要素のタイプには以下が含まれます。
* **データ要素 (Data elements):** テーブル、チャート、ピボットテーブルなど。「[Create a data element](https://help.sigmacomputing.com/docs/create-a-data-element)」を参照。
* **入力要素 (Input elements):** 空の、またはリンクされた入力テーブルなど。「[Intro to input tables](https://help.sigmacomputing.com/docs/input-tables-overview)」を参照。
* **コントロール要素 (Control elements):** フィルターや入力など。「[Intro to control elements](https://help.sigmacomputing.com/docs/intro-to-control-elements)」を参照。
* **UI要素 (UI elements):** テキスト、画像、ボタン、埋め込み、区切り線など。「[Intro to UI elements](https://help.sigmacomputing.com/docs/intro-to-ui-elements)」を参照。
* **レイアウト要素 (Layout elements):** コンテナ、タブ付きコンテナ、モーダルなど。「[Design workbook layouts](https://help.sigmacomputing.com/docs/design-workbook-layouts)」を参照。

ワークブックの使用とナビゲーションに関する詳細は、「[Navigate a workbook](https://help.sigmacomputing.com/docs/navigate-a-workbook)」を参照してください。

**ワークブックのライフサイクル (The lifecycle of a workbook)**

最初にワークブックを作成すると、「探索（exploration）」が開きます。探索とは、保存されていないワークブックのことで、現時点を超えて必要ないかもしれないアドホックなデータ探索や探索的データ分析（EDA）のワークフローをサポートします。探索を使用することで、一度きりのドキュメントでフォルダやワークスペースが散らかるのを避けるのに役立ちます。探索には `Recents` ページの `Explorations` タブからアクセスできます。詳細は、「[Ad hoc data explorations](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations)」を参照してください。

分析や実験を続けるには、探索をワークブックとして保存します。ワークブックを保存すると、ドラフトで編集や変更を行ったり、ダッシュボードやレポートのように公開されたバージョンのワークブックを閲覧したりできます。詳細は、「[Create a workbook](https://help.sigmacomputing.com/docs/create-a-workbook)」および「[Workbook lifecycle: explore, draft, and publish](https://help.sigmacomputing.com/docs/workbook-lifecycle)」を参照してください。

保存後、他の人がアクセスできるフォルダやワークスペースに保存しない限り、あなただけがワークブックにアクセスできます。ワークブックの共有に関する詳細は、「[Share a workbook](https://help.sigmacomputing.com/docs/share-a-workbook)」を参照してください。

ワークブックが作成された後、異なるユーザーが異なる方法でそれと対話できます。
* 埋め込み分析ソリューションのユーザーには、最新の公開バージョンに依存するのではなく、タグ付けされた安定版のワークブックへのアクセスを許可したい場合があります。「[Add version tags to workbooks and data models](https://help.sigmacomputing.com/docs/add-version-tags)」を参照してください。
* ワークブックを作成する権限がないユーザーでも、ビューを作成することで既存のワークブックをカスタマイズできる場合があります。「[Create and interact with custom views](https://help.sigmacomputing.com/docs/create-and-interact-with-custom-views)」を参照してください。ワークブックの特定の設定を保存するには、ビューを保存して他の人と共有できます。「[Create and share saved views](https://help.sigmacomputing.com/docs/create-and-share-saved-views)」を参照してください。
* アクセス権が少ないユーザーは、あなたが構築したダッシュボードやレポートを閲覧またはフィルタリングすることしかできないか、[データアプリ](https://help.sigmacomputing.com/docs/intro-to-app-like-functionality)のフォームにデータを入力することしかできない場合があります。
詳細は、「[Workbook modes: view, explore, and edit](https://help.sigmacomputing.com/docs/workbook-modes-overview)」を参照してください。

**ワークブックで使用されるデータ (Data used in workbooks)**

ワークブックは、Sigmaに接続された[サポートされているデータプラットフォーム](https://help.sigmacomputing.com/docs/connect-to-data-sources)のテーブル、Sigmaで作成されたデータモデルのテーブル、または[CSV形式のファイル](https://help.sigmacomputing.com/docs/upload-csv-data)や[入力テーブル](https://help.sigmacomputing.com/docs/input-tables-overview)に追加された情報など、Sigmaに追加されてデータプラットフォームに保存されたデータといった、複数のソースからのデータを使用できます。データプラットフォームへの接続に関する詳細は、「[Connect to data sources](https://help.sigmacomputing.com/docs/connect-to-data-sources)」を参照してください。

あなたのデータは常にライブであり、大規模にアクセス可能で、削除されたり破損したりすることはありません。

Sigmaがあなたのデータプラットフォームに接続された後、データベースやデータカタログのテーブルから直接ワークブックを作成したり、Sigmaでデータをモデリングしたりできます。ワークブックのソースとしてデータモデルやデータセットを使用することは、一貫性を確保するのに役立ちます。詳細は、「[Get started with data modeling](https://help.sigmacomputing.com/docs/get-started-with-data-modeling)」および「[Data modeling tutorial](https://help.sigmacomputing.com/docs/tutorial-data-modeling-with-datasets)」を参照してください。

ユーザーが共有されたデータセット、データモデル、またはワークブックにアクセスすると、ドキュメント所有者のソースデータへのアクセス権がSigma内で評価され、接続設定で指定された資格情報を使用してデータプラットフォームへのクエリが実行されます。
OAuthをサポートする接続の場合、クエリは代わりに異なる方法で実行されることがあります。
* 接続がサービスアカウントなしでOAuthを使用するように構成されている場合、ドキュメントからのクエリは、データプラットフォーム用に構成されたユーザー個人のOAuth資格情報で実行されます。
* 接続がサービスアカウントありでOAuthを使用するように構成されている場合、管理者は個々のワークブックを代わりにサービスアカウントの資格情報を使用するように構成できます。「[Run a workbook with service account credentials](https://help.sigmacomputing.com/docs/run-a-workbook-with-service-account-credentials)」を参照してください。

ワークブックやデータモデルでどのクエリが実行されているかの詳細については、「[Examine workbook and data model queries](https://help.sigmacomputing.com/docs/examine-workbook-queries)」を参照してください。データセットについては、「[Examine dataset queries](https://help.sigmacomputing.com/docs/examine-dataset-queries)」を参照してください。

**レガシーワークシートユーザー向けの情報 (Information for legacy worksheet users)**

以前にSigmaのワークシートやダッシュボードを使用していた場合、単一のダッシュボードのビジュアライゼーションをソースとするために複数のワークシートを作成するプロセスに慣れているかもしれません。ワークブックは、あなたのレポート消費者に表示される場所で直接分析を構築できるようにすることで、このワークフローを緩和します。

#### 4-1-2. ワークブックのモード概要 (Workbook modes overview)

Sigmaは、ワークブック内での異なるレベルのインタラクション、カスタマイズ、および分析を提供する3つのワークブックモード（**表示**、**探索**、**編集**）を備えています。各モードは、あなたの目的と権限に応じて特定のタスクを実行するのに役立つように設計されています。

---

### ワークブックモードの目的

| | 表示モード (View mode) | 探索モード (Explore mode) | 編集モード (Edit mode) |
| :--- | :--- | :--- | :--- |
| **目的** | ワークブックの公開バージョン（「Published」とラベル付けされたバージョンおよび全てのタグ付きバージョン）を閲覧できます。 | 保存または共有されたワークブックのバージョンに影響を与えることなく、公開されたワークブックのコンテンツをカスタマイズし、あなた自身のカスタムビューでアドホック分析を実行するための隔離された環境を提供します。 | 個人または共同での分析を編集・保存できる、フルスコープの分析機能を備えたドラフト環境を提供します。 |
| **ユースケース** | 追加の分析を行わずに、準備されたデータやインサイトを閲覧する必要がある場合に推奨されます。 | 特定のビジネス上の質問に対する迅速な回答が必要だが、変更が公開バージョンに影響を与えたくない場合に推奨されます。 | 将来の使用や共有のためにレポートを構築し、公開する必要がある場合に推奨されます。 |
| **必要なアカウントタイプの権限** | `View workbooks` または `Basic explore` | `Full explore` | `Create, edit, and publish workbooks` |
| **必要なワークブックのアクセス権** | `Can view`, `Can explore`, `Can edit`, または `Owner` | `Can explore`, `Can edit`, または `Owner` | `Can edit` または `Owner` |

---

### ワークブックのアクセシビリティ比較

以下の表は、あなたに付与された、またはワークスペースやフォルダのアクセスから継承されたワークブックのアクセス権に基づいて、各モードで何ができるかを比較したものです。

| アクション | 表示モード<br>(Can view) | 表示モード<br>(Can explore / Can edit) | 探索モード<br>(Can explore / Can edit) | 編集モード<br>(Can edit) |
| :--- | :---: | :---: | :---: | :---: |
| コントロールの値を更新する | ✅ | ✅ | ✅ | ✅ |
| 既存のフィルターを修正する | ✅ | ✅ | ✅ | ✅ |
| 列データをソートする | ✅ | ✅ | ✅ | ✅ |
| 列の詳細を表示する | ✅ | ✅ | ✅ | ✅ |
| グループ化された行を展開/折りたたむ | ✅ | ✅ | ✅ | ✅ |
| **集計済み**の基盤データを表示する | ✅ | ✅ | ✅ | ✅ |
| データをリフレッシュする | | ✅ | ✅ | ✅ |
| 保存済みビューを作成する | | ✅ | ✅ | ✅ |
| コメントを表示・追加する¹ | | ✅ | ✅ | ✅ |
| 新しいフィルターを作成する | | | ✅ | ✅ |
| **非集計**の基盤データを表示・ドリルする | | | ✅ | ✅ |
| ドリルパスを使用する（"Drill anywhere"）| | | ✅ | ✅ |
| 列のフォーマット、並べ替え、名前変更、非表示、固定、削除 | | | ✅ | ✅ |
| 入力テーブルの値を入力する² | | | ✅ | ✅ |
| 個々の要素をPNGにダウンロードする | | | ✅ | ✅ |
| 個々の要素をCSV, Excel, JSON, Google Sheets, PDFにダウンロードする³ | | | ✅ | ✅ |
| エクスポートを送信またはスケジュールする⁴ | | | ✅ | ✅ |
| データポイントの値をコピーする | | | ✅ | ✅ |
| ページを作成、編集、削除する | | | | ✅ |
| 要素を作成、編集、削除する<br>(編集にはプロパティ、フォーマット、アクション、列等を含む) | | | | ✅ |
| 既存の要素を複製、移動する | | | | ✅ |
| 要素をコピー/ペーストする | | | | ✅ |
| 要素のデータソースを表示・変更する | | | | ✅ |
| 列を追加・修正する | | | | ✅ |
| カスタムSQLロジックを表示する | | | | ✅ |
| レイアウトとワークブック設定を編集する | | | | ✅ |
| リネージ（系譜）を表示する | | | | ✅ |
| 非表示のページを表示する | | | | ✅ |
| ワークブックの編集を公開する | | | | ✅ |

¹ `Can comment on workbooks` 権限が有効になっているアカウントタイプが必要です。
² 入力テーブル要素の `data entry permission` がワークブックの公開バージョンに設定されている必要があります。
³ CSV, Excel, JSON, PDFへのダウンロードには `Download or Send Now` 権限が有効なアカウントタイプが必要です。Google Sheetsへのダウンロードには `Export to Google Sheet` 権限も必要です。
⁴ エクスポートの送信（`Send now`機能を使用）には `Download or Send Now` 権限が有効なアカウントタイプが必要です。エクスポートのスケジュール設定には `Schedule export` 権限が必要です。

##### 4-1-3. ワークブックの操作 (Navigate a workbook)

このドキュメントでは、ワークブックを操作し、使用する方法について説明します。ワークブックの構成とライフサイクル管理の詳細については、「ワークブックの概要」を参照してください。

#### **ユーザー要件 (User requirements)**

`Can view`、`Can explore`、または `Can edit` の権限を持つユーザーは、公開された状態のワークブックを閲覧および操作できますが、個々の権限によって異なるオプションが表示されます。

ワークブックを編集するには `Can edit` 権限が必要です。

ワークブックの権限によっては、以下のオプションの一部が利用できない場合があります。個々のユーザー権限の詳細については、「ワークブックのモード概要」を参照してください。

---

#### **公開済みバージョンのワークブックを操作する (Navigate the published version of a workbook)**

公開済みのワークブックを操作することで、既存のデータとインサイトを閲覧できます。個々のユーザー権限によっては、新しいフィルターの変更または追加、データの更新、独自のカスタムビューおよび保存済みビューの作成も可能です。

公開済みのワークブックでは、以下のオプションが利用可能です。権限によっては一部利用できない場合があります。
<img width="1803" height="1068" alt="21e909698b4fbd7722baa409a162a0837eca48b4fc4c95f05ceeeb3772cb0e96-publishedlayour" src="https://github.com/user-attachments/assets/69cf7502-0a1a-4f4d-830d-7aa8f056c4c9" />

* **a. ホーム (Home):** 「ホーム」に移動して、組織内の他のドキュメントの表示、管理ポータルへのアクセス、ユーザープロファイルなどを確認します。ホームページの操作の詳細については、「Sigmaの基本操作」を参照してください。

* **b. ドキュメントメニュー (Document menu):** 保存済みビューの作成または管理、バージョンタグの追加、ワークブックの共有、コメントの追加、エクスポートのスケジュール設定など、主要なワークブックアクションを実行するための一元化されたメニューです。

* **c. 編集ボタン (Edit button):** (「Can edit」アクセス権を持つユーザーのみに表示) ワークブックに変更を加える場合に選択します。

* **d. このビューをカスタマイズ (Customize this view) ボタン:** (「Full explore」権限および/または「Can edit」アクセス権を持つユーザーのみに表示) ワークブックの公開バージョンに影響を与えることなく、要素を操作して変更を加えることで、ワークブックの独自のビューを作成します。「カスタムビューの作成と操作」を参照してください。

* **e. 共有 (Share) ボタン:** (「Can edit」アクセス権を持つユーザーのみに表示) ワークブックを他のメンバーまたはチームと共有します。「ワークブックを共有する」を参照してください。

* **f. データ更新 (Refresh data) ボタン:** ワークブック内のすべてのデータソースを更新します。より高度なオプションについては、「ワークブックの更新オプションの管理」を参照してください。

* **g. その他のオプション (More options) ボタン:** クエリの一時停止、クエリ履歴へのアクセス、データ更新設定の変更などのオプションを表示するために選択します。「ワークブックのクエリの調査」および「ワークブックの更新オプションの管理」を参照してください。

* **h. ページタブ (Page tabs):** ワークブック内のすべてのページ間を移動します。各ページタブのキャレットから、コピーおよびエクスポートオプションにアクセスします。「ワークブックのページをコピーする」を参照してください。

* **i. ヘルプ (Help) メニュー:** サポートライブチャット、ドキュメント、コミュニティ投稿、クイックスタート、関数インデックスなどのヘルプリソースにアクセスします。

---

#### **編集中にワークブックを操作する (Navigate a workbook while editing)**

新しいワークブックを作成したり、既存のワークブックを変更したり、変更を公開したりするには、ワークブックを編集する必要があります。ワークブックを編集するには `Can edit` 権限が必要です。

ワークブックの編集中は、公開済みバージョンで利用可能なすべてのオプションに加えて、以下の追加オプションが利用可能です。
<img width="1803" alt="21e909698b4fbd7722baa409a162a0837eca48b4fc4c95f05ceeeb3772cb0e96-publishedlayour" src="https://github.com/user-attachments/assets/204ff0de-5e5c-4f2c-8952-8f5f90cc8c7a" />

* **a. ツールバー (Toolbar):** 数値およびテキストの書式設定オプションにアクセスします。選択した要素に応じて、異なるオプションが表示されます。

* **b. 公開 (Publish) ボタン:** 変更を公開します。

* **c. 公開メニュー (Publish menu):** 異なるアクセスレベルでワークブックをプレビューしたり、ワークブックのモバイルプレビューとデスクトッププレビューを切り替えたりします。

* **d. 数式バー (Formula bar):** 列に必要な計算を実行するための数式を入力します。サポートされている関数については、関数インデックスを参照してください。

* **e. パネルの表示/非表示 (Show/Hide panels) ボタン:** ワークブックをより明確に表示するために、エディターやバージョン履歴パネルなどのサイドパネルを表示または非表示にします。

* **f. サイドパネル (Side panels):** ワークブックページで行っている操作に応じて、異なるタブが利用可能です。
    * **要素を選択した場合:** 要素のタイプに応じて、異なるタブが表示されます。たとえば、データ要素を選択すると、「プロパティ」、「フォーマット」、「アクション」タブが表示されます。テキスト要素を選択すると、「フォーマット」タブが表示されます。
    * **ワークブックの背景を選択した場合:** 「設定」および「アクション」タブが表示されます。
    * **バージョン履歴を表示している場合:** 「バージョン履歴」パネルが表示されます。

* **g. ページ概要 (Page overview) ボタン:** ワークブック内のすべてのページを表示し、その名前を選択することで特定のワークブック要素に移動します。

* **h. ページの追加 (Add page) ボタン:** ワークブックに新しいページを追加するために選択します。

* **i. 要素の追加バー (Add element bar):** ワークブック要素を追加および表示します。利用可能なデータ要素、UI要素、およびコントロール要素の詳細については、「要素の種類の概要」を参照してください。

* **j. リネージ (Lineage) ボタン:** ワークブック内のすべてのデータ要素間の関連性と系統を表示するために選択します。詳細については、「ワークブックのデータリネージの表示」を参照してください。

##### 4-1-4. ワークブックでのライブ編集による共同作業 (Collaborate with Live Edit in workbooks)

あなたのチームは、すべての編集者が一つのライブドラフトを共有し、リアルタイムでワークブックのドラフトで共同作業できます。「ライブ編集」機能を使用すると、他の人がドラフトした変更が公開される前に、それらを表示し、貢献することができます。

#### **要件 (Requirements)**

ワークブックへの `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)を持つユーザーのみが貢献できます。

#### **ワークブックを編集する (Edit a workbook)**

ワークブックを編集するには、「[ワークブックの編集、ドラフト、公開](https://help.sigmacomputing.com/docs/workbook-lifecycle)」を参照してください。

#### **他の共同作業者を表示する (View other collaborators)**

ヘッダーには、現在編集モードにいるすべてのユーザーのリストが表示されます。

> 💡
> ユーザーのアイコンをクリックすると、彼らが選択している要素（もし選択していれば）に移動します。
![5017da6-multipleeditors](https://github.com/user-attachments/assets/eccbff54-a1a1-4177-b3bb-2e744f62fd9d)

Sigmaは、要素を選択したユーザーの名前を、選択された要素のバウンディングボックスの左上隅に自動的に表示します。

#### **共同作業中に公開する (Publish while collaborating)**

Sigmaは、ドラフトに加えたすべての変更を自動的に保存し、他のすべての同時編集者にその変更を表示します。

編集者が `Publish` をクリックすると、Sigmaは他のすべての編集者によってドラフトされた変更を含む、すべてのドラフトされた変更を公開します。

#### 4-1-5. 要素タイプの概要 (Intro to Element Types)

ワークブックは通常、単一ページおよび/または複数ページに分散された要素のコレクションを含みます。

要素には3つのタイプがあります：**データ要素**、**UI要素**、および**コントロール要素**です。それぞれが独自の機能を持ち、それらが集合的に、あなたのデータを表示し、操作し、追加のコンテキストを提供することを可能にします。

ワークブックの編集者は要素を定義し、閲覧者のインタラクションのために個別に構成することができます。

**データ要素 (Data Elements)**

データ要素には、データソースから直接構築されたテーブル、ピボットテーブル、およびビジュアライゼーションが含まれます。ワークブックは、複数のデータソースから派生した様々なデータ要素を含むことができます。詳細は、「データ要素の概要」を参照してください。
![741f849-1](https://github.com/user-attachments/assets/c254ec04-96cf-467c-a15b-528f633377cb)!<img width="1410" height="921" alt="741f849-1" src="https://github.com/user-attachments/assets/efe3387b-f7c0-4431-972c-09622e03cd60" />

**UI要素 (UI Elements)**

UI要素には、コンテキストおよび/またはワークブックのスタイリングを追加するために使用されるボタン、区切り線、画像、スペーサー、埋め込み、およびテキストが含まれます。詳細は、「UI要素の概要」を参照してください。
![4a6bb19-2](https://github.com/user-attachments/assets/062134de-6d3e-4cfb-8f11-ae9f08309573)
<img width="1407" height="566" alt="4a6bb19-2" src="https://github.com/user-attachments/assets/de0e363b-0134-4297-ad3a-8499b18d2093" />

**コントロール要素 (Control Elements)**

コントロール要素には、ワークブック内のデータ要素を操作するために使用されるデータフィルターとパラメータが含まれます。詳細は、「コントロール要素の概要」を参照してください。
<img width="1007" alt="e773c5b-3" src="https://github.com/user-attachments/assets/42a09fda-9b55-4972-9a24-ca4e71b41128" />


#### 4-2-1. ワークブックを作成する (Create a workbook)

ワークブックは、アドホックなデータ探索と複雑な長期レポーティングの両方をサポートするように設計されたSigmaドキュメントタイプです。ワークブックを作成すると、[データ、UI、コントロール要素の追加](https://help.sigmacomputing.com/docs/intro-to-element-types)、[ワークブックレイアウトのカスタマイズ](https://help.sigmacomputing.com/docs/design-workbook-layouts)、[チャートの追加](https://help.sigmacomputing.com/docs/build-a-chart)、[データアプリの構築](https://help.sigmacomputing.com/docs/intro-to-app-like-functionality)、[埋め込み分析の追加](https://help.sigmacomputing.com/docs/intro-to-embedded-analytics)などが可能になります。

公開されていないワークブックは「探索（explorations）」と呼ばれます。

このドキュメントでは、新しいワークブックまたは探索を作成する方法について説明します。ワークブックの概念的な概要については、「[Workbooks overview](https://help.sigmacomputing.com/docs/workbooks-overview)」を参照してください。ワークブックの使用とナビゲーションに関する詳細は、「[Navigate a workbook](https://help.sigmacomputing.com/docs/navigate-a-workbook)」を参照してください。

#### **ユーザー要件 (User requirements)**

ワークブックまたは探索を作成するには、`Create, edit, and publish workbooks` 権限が必要です。「[Account type and license overview](https://help.sigmacomputing.com/docs/account-type-and-license-overview)」を参照してください。

#### **ワークブックまたは探索を作成する (Create a workbook or exploration)**

いくつかの場所からワークブックまたは探索を作成できます。

> 📘
> 探索は、作成後30日間、Sigmaのホームページからアクセスできます。「[Recent](https://help.sigmacomputing.com/docs/get-around-in-sigma#recents)」 > 「[Explorations](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations)」を参照してください。

* **Sigmaホームページから作成する**
    1.  `+ Create New` を選択し、`Workbook` を選択します。新しい探索が表示されます。
    2.  変更を加えた後、`Publish` を選択して探索をワークブックとして保存します。

* **データソースから作成する**
    データソース（データプラットフォームのテーブルなど）からワークブックを作成できます。
    1.  データソースから、`Explore` を選択します。新しい探索が表示されます。
    2.  変更を加えた後、`Publish` を選択して探索をワークブックとして保存します。

* **既存のワークブックから作成する**
    既存のワークブックのコピーを作成できます。
    1.  目的のワークブックから、ドキュメントメニューを選択します。
    2.  `File` > `Save as a new workbook` を選択します。
    3.  ワークブックの名前を入力し、`Save` を選択します。
    4.  変更を加えた後、`Publish` を選択して探索をワークブックとして保存します。

* **テンプレートから作成する**
    テンプレートを使用すると、迅速で一貫性のあるレポーティングのために、特定のワークブック構造を再利用および共有できます。「[Create workbooks from templates](https://help.sigmacomputing.com/docs/get-started-with-workbook-templates)」を参照してください。

#### 4-2-2. アドホックなデータ探索 (Ad hoc data explorations)

探索（Explorations）は、アドホックなデータ分析をサポートする、公開されていない[ワークブック](https://help.sigmacomputing.com/docs/workbooks-overview)です。

このドキュメントでは、新しい探索を作成し、既存のものに戻って分析を続けたり、他の組織ユーザーと共有したり、ワークブックとして保存したりする方法を説明します。

> 📘
> Sigmaはあなたの探索を `Recent` ページに保存します。保存された探索は削除できません。

#### **ユーザー要件 (User requirements)**

新しい探索を作成するには、`Create, edit, and publish workbooks` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。

#### **新しい探索を作成する (Create a new exploration)**

新しいワークブックを作成するのと同じ方法で探索を作成します。詳細は、「[ワークブックまたは探索を作成する](https://help.sigmacomputing.com/docs/create-a-workbook#create-a-workbook-or-exploration)」を参照してください。

#### **保存された探索を再度開く (Reopen a saved exploration)**

保存された探索を再度開いて、アドホックなデータ分析を続けます。

1.  あなたの**ホーム**ページに移動します。
2.  ナビゲーションメニューで、`Recent` を選択します。
3.  `Recent` ページで、`Explorations` タブを選択して、過去の探索のリストを表示します。
4.  特定の探索を開くには、`Created on` の日付をクリックします。

#### **探索を共有する (Share an exploration)**

他の組織ユーザーがあなたのアドホックなデータ分析に貢献できるように、探索を共有します。

1.  [新しい探索を作成する](https://help.sigmacomputing.com/docs/create-a-workbook#create-a-workbook-or-exploration)か、[保存されたものを再度開きます](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations#reopen-a-saved-exploration)。
2.  探索のヘッダーで、キャレット()をクリックして探索メニューを開き、`Share` を選択します。
3.  `Share workbook` モーダルで、`Allow access by link` トグルをオンの位置にクリックします。
4.  提供されたURLをコピーし、任意の組織ユーザーと共有します。

#### **探索をワークブックとして保存する (Save an exploration as a workbook)**

探索をワークブックとして保存し、特定のフォルダに公開します。

1.  [新しい探索を作成する](https://help.sigmacomputing.com/docs/create-a-workbook#create-a-workbook-or-exploration)か、[保存されたものを再度開きます](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations#reopen-a-saved-exploration)。
2.  探索のヘッダーで、`Save As` をクリックします。また、キャレット()をクリックして探索メニューを開き、`Save` を選択することもできます。
3.  `Save as` モーダルで、ワークブックを公開します。
    * `Name` フィールドに、ワークブックの名前を入力します。
    * `Destination` セクションで、ワークブックを公開したいフォルダを選択します。
    * `Save` をクリックします。

#### 4-2-3. 組織のプラグインを使用する (Use your organization's plugins)

Sigmaでは、ワークブックにプラグイン要素を追加して、Sigmaの標準展開では提供されないカスタム機能をサポートすることができます。あなたは、あなたの組織に登録されているプラグインにのみアクセスできます。プラグインは、既存の製品に追加機能をもたらすために構築されたサードパーティのアプリケーションです。例えば、あなたの組織のソフトウェア開発者が、Sigmaではサポートされていないチャートタイプでデータを表示できるプラグインを作成することがあります。

#### **要件 (Requirements)**

プラグインを通じてワークブック要素を追加または編集するには：
* あなたは`Creator`または`Admin`であるか、適切な権限を持つ[カスタムアカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)である必要があります。
* 関連するワークブックに対する`Can Edit`[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)を持っている必要があります。

#### **プラグインを通じてワークブックに要素を追加する (Add an element to a workbook through a plugin)**

プラグインベースの要素は、データソースとして[データ要素](https://help.sigmacomputing.com/docs/create-a-data-element)のみを受け付けます。ソースとなるデータ要素は、プラグインと同じワークブック内にある必要があります。

* **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ページの右上隅にある `Edit` をクリックします。「[Workbook lifecycle](https://help.sigmacomputing.com/docs/workbook-lifecycle)」を参照してください。

1.  ワークブックの `ADD NEW` パネルを開きます。
2.  `PLUGINS` を選択します。![f9e0a7f-1](https://github.com/user-attachments/assets/34f27cd1-3079-47b6-b9d5-c9796a165663)


3.  リストからプラグインタイプを選択します。![d3f4274-2](https://github.com/user-attachments/assets/97215572-2ac3-4a23-a552-84d2fad9a1c1)
 新しい空のプラグインベースの要素がページに表示されます。![bbd4ee0-3](https://github.com/user-attachments/assets/b3d4a472-f9e1-4e03-88d3-0ec07f5bd75b)

4.  エディタパネルを使用して、要素の値を構成します。
    * 個々のプラグインが、各要素の構成オプションを定義します。

プラグインは、データソースの最初の25,000行にしかアクセスできません。したがって、データの[グループ化と集計](https://help.sigmacomputing.com/docs/create-and-manage-tables#group-data)を行って、総行数を減らしてください。データソースに既にグルーピングが含まれている場合、エディタパネルは集計レベルを選択するように促します。   
<img width="1374" height="761" alt="da70c96-4" src="https://github.com/user-attachments/assets/53426cb4-6a94-4b88-80ec-32631b3205bf" />

#### 4-2-4. ワークブックのドラフトと公開 (Draft and publish a workbook)

ワークブックを編集すると、ドラフトが作成されます。変更を、ワークブックへの表示アクセス権や探索アクセス権を持つユーザーに見えるようにするには、ドラフトを公開します。また、ドラフトを破棄して、以前に公開されたバージョンに戻ることも選択できます。

複数のユーザーが同時にワークブックを編集する場合、編集内容は自動的に共有されたライブドラフトに保存されます。複数の編集者がこの単一のドラフトでリアルタイムに共同作業できます。「[Collaborate with Live Edit in workbooks](https://help.sigmacomputing.com/docs/collaborate-with-live-edit-in-workbooks)」を参照してください。

このドキュメントでは、ドラフトを編集し、ワークブックを公開する方法について説明します。

#### **要件 (Requirement)**

新しいワークブックのバージョンをドラフトし、公開するには、個々のワークブックに対する`Can edit`[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)を持っている必要があります。

#### **既存のワークブックを編集する (Edit an existing workbook)**

既存のワークブックを表示モードから編集を開始するには、ワークブックヘッダーの `Edit` をクリックします。
![bf5fc6ce02960fc2cd3349e597101b22597a3255a6c154ca49a98bd23119ca66-clickedit_header](https://github.com/user-attachments/assets/e3ed98cf-1477-49c6-a94c-2ffe9b6cf454)

カスタムビューから既存のワークブックの編集を開始するには、ドキュメントメニューをクリックし、次に `Edit` > `Edit workbook` をクリックします。
![ea37e0ac80b571143af58622cc3a1973c52d482a7a842f9b9c1e5b20ac198a88-edit-from-custom-view](https://github.com/user-attachments/assets/581f824a-0273-4fa3-82a6-a7720ddb4a4f)

ワークブックが編集モードに入ると、ワークブックのヘッダーが変更されます。
* `Edit` ボタンが `Publish` メニューに変わります。
* ドキュメントメニューに `Draft` が追加されます。
* ヘッダーには、現在編集モードにいる他のすべてのユーザーのイニシャルが表示されます。「[Collaborate with Live Edit in workbooks](https://help.sigmacomputing.com/docs/collaborate-with-live-edit-in-workbooks)」を参照してください。
![e45e3f3d0837afe527b90edf54a58ab2acdcfe556fbf12b11704df2380501618-editmode-header](https://github.com/user-attachments/assets/c334ee9d-78b6-4775-b64d-cde542ad33bc)

さらに、ワークブックが編集モードに入ると：
* エディタパネルがページの右側に表示されます。
* `Add element bar` がキャンバスの下部に表示されます。
* フッターに追加のオプションが表示されます。

#### **編集モードでの変更 (Making changes in edit mode)**

ドラフトに加えた変更は、すべての編集者が共有するライブドラフトに自動的に保存されます。
編集者が `Publish` をクリックすると、Sigmaはライブドラフト上で他の編集者によって行われた変更を含む、すべてのドラフトされた変更を公開します。

#### **ドラフトされた変更をプレビューする (Preview drafted changes)**

公開前に、探索モードと表示モードの両方で、すべてのドラフトされた変更をプレビューできます。これは、ワークブックへの表示アクセス権または探索アクセス権を持つユーザーにワークブックがどのように見えるかを確認したい場合に役立ちます。

ドラフトされた変更をプレビューするには：
1.  キャレットをクリックして `Publish` メニューを開きます。
2.  `Preview with` の下で、`View access` または `Explore access` のいずれかを選択します。![e4a61181ae8c22271793328436260066c80e4517a15849c462af0aaee39906c0-preview-with-explore](https://github.com/user-attachments/assets/8b073fca-f5a7-4dd5-a508-e27446c31ace)

3.  プレビューが終了したら、`Exit preview` をクリックします。

#### **ドラフトされた変更を公開する (Publish drafted changes)**

編集内容を公開するには、ワークブックヘッダーにある `Publish` ボタンをクリックします。
<img width="640" height="56" alt="425a499069dbf1dd267baf2fd2e98f6bda0c7591ab76eafbdfe0bf215761cf85-click-publish" src="https://github.com/user-attachments/assets/3ab432e5-f492-4fb1-bbb3-06bd9db4e496" />

このアクションは、ライブドラフトを使用して他の編集者によって行われた変更を含む、ワークブックへのすべてのドラフトされた変更を公開します。

#### **ドラフトされた変更を破棄する (Discard drafted changes)**

ドラフトされた変更を破棄するには、キャレットをクリックして `Publish` メニューを開き、次に `Discard draft` をクリックします。
![425a499069dbf1dd267baf2fd2e98f6bda0c7591ab76eafbdfe0bf215761cf85-click-publish](https://github.com/user-attachments/assets/8148c19d-22c2-4fc0-a2dc-d488e4f476ee)

> 🚧
> いずれかの編集者がドラフトを破棄すると、Sigmaはどの編集者によって行われた未公開の編集もすべて破棄します。

#### **最新の公開バージョンに戻る (Return to the latest published version)**

ワークブックの最新の公開バージョンに戻るには、キャレットをクリックして `Publish` メニューを開き、次に `Go to published version` をクリックします。
![3a00de808cd3a355d3c599ff30335dcf113581d15a26e114291a7cd14d0990b9-go-to-published](https://github.com/user-attachments/assets/d36a2617-6d0a-46cb-8a5b-2bb8ea1a6fce)

Sigmaはあなたのドラフトされた変更を破棄しません。公開バージョンの `Edit` ボタンをクリックすることで、いつでも共有ドラフトに戻ることができます。
詳細は、「[Workbook version history](https://help.sigmacomputing.com/docs/document-versions-and-version-history)」を参照してください。

### 4-2-5. ワークブックのページをコピーする (Copy workbook pages)

あるワークブックから別のワークブックへページをコピーしたり、同じワークブック内のあるページを別のページにコピーしたりすることができます。

#### **要件 (Requirements)**

* ワークブック間でコピー＆ペーストする場合、両方のワークブックは同じ組織に属している必要があります。
* ワークブック間でコピー＆ペーストする場合、両方のワークブックは同じレイアウトスタイルを使用している必要があります。古いレイアウトから新しいグリッドレイアウトへページをコピーすることはできません。新しいグリッドレイアウトの詳細については、「[Create and manage workbook layouts](https://help.sigmacomputing.com/docs/design-workbook-layouts)」を参照してください。
* 一つまたは複数のワークブックについて、あなたのアカウントタイプはProまたはAdminであるか、`Edit Workbook` または `Explore Workbook` 権限が有効になっているカスタム[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)である必要があります。
* 一つまたは複数のワークブックに対して、あなたがワークブックの所有者であるか、`Can edit` または `Can explore` の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **ワークブックページをコピー＆ペーストする際のヒント (Tips for copy and pasting workbook pages)**

* Sigmaはページ全体に加え、ページ上の要素の依存ソースもコピーします。たとえそのソースがページ上にない場合でもです。ページ上にないソースについては、Sigmaは「ページ名 - Dependencies」という命名規則で2番目のページを作成します。
* コピー操作を行うユーザーが、ページ上の要素のソースデータへのアクセス権を持っていない場合、Sigmaはそれをコピー＆ペーストしますが、ユーザーにはデータが表示されず、貼り付けられた要素には権限エラーメッセージが表示されることがあります。
* リンクされた入力テーブルは、ワークブックページのコピー＆ペースト時にはサポートされていません。Sigmaは、空の入力テーブルと、すべてのデータ、UI、およびコントロール要素をコピーできます。
* もしページ上の要素だけをコピーする必要がある場合は、その操作を検討してください。「[Copy and paste elements](https://help.sigmacomputing.com/docs/copy-and-paste-elements)」を参照してください。

#### **ページをコピー＆ペーストする (Copy and paste a page)**

1.  ページメニューから、`Copy page` を選択します。Sigmaがページをコピーします。
2.  (任意) コピー確認メッセージの外側をクリックするか、数秒待って消えるのを待ちます。
3.  コピーしたページを貼り付けます。
    * **同じワークブックにコピーする場合、** `cmd/ctrl-v` を押すか、右クリックして `Paste` を選択します。<img width="182" alt="be30309-2" src="https://github.com/user-attachments/assets/cd6f7e8f-0929-4343-a440-98067d6a48e1" />

        * Sigmaは新しいページをワークブックに貼り付け、ページ名に「Copy」を追記します。<img width="204" alt="7b0048a-3" src="https://github.com/user-attachments/assets/9f884920-fef2-44f0-808d-553228bfaaed" />


    * **別のワークブックにコピーする場合、** そのワークブックに移動して編集モードに入ります。`cmd/ctrl-v` を押すか、右クリックして `Paste` を選択します。
        * Sigmaは新しいページをワークブックに貼り付け、ページ名に「Copy」を追記します。

        * 依存関係がある場合、Sigmaはそれらを別のページに貼り付け、ページ名に「Dependencies」を追記します。
4.  新しい、コピーされたページを好きなように編集します。

### 4-2-6. ワークブックの要素をコピー＆ペーストする (Copy and paste workbook elements)

Sigmaのコピー＆ペースト機能を使用すると、様々な場所に要素を複製できます。要素を元のワークブック内でコピー＆ペーストすることも、あるワークブックから要素をコピーして別のワークブックに貼り付けることもできます。

#### **ユーザー要件 (User requirements)**

要素をコピー＆ペーストする機能には、以下が必要です。
* `Explore workbooks` または `Create, edit, and publish workbooks` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがワークブックの所有者であるか、`Can explore` または `Can edit` の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **要素をコピー＆ペーストする (Copy and paste an element)**

要素をコピーし、それを空のスペースに、または宛先ワークブックの既存の要素の真下に貼り付けます。子要素をコピーした場合、そのリネージ（系譜）もコピー＆ペーストされます。

> 🚩
> リンクされた入力テーブルは、現在コピー＆ペースト機能をサポートしていません。しかし、空の入力テーブルと、すべてのデータ、UI、およびコントロール要素はコピーできます。

##### **要素をコピーする (Copy the element)**

1.  任意のモードでワークブックを開き、コピーしたい要素を選択するか、カーソルを合わせます。
2.  要素のツールバーで、`More` をクリックして要素メニューを開き、`Copy element` を選択します。元の要素と、そのリネージ内の適用可能なすべての親要素がコピーされます。![copy-paste_copy-element](https://github.com/user-attachments/assets/c4cbc6ca-6a08-44fd-ba23-fc7a3dc6c7c7)


##### **空のスペースに要素を貼り付ける (Paste the element in an empty space)**

1.  宛先のワークブックを `Explore` または `Edit` モードで開き、キャンバス上の空のスペースを見つけます。
2.  空のスペースを右クリックしてアクションメニューを開き、`Paste element` を選択します。![copy-paste_paste-element](https://github.com/user-attachments/assets/b0fbcf50-452a-42a0-adc4-c4832699fc70)
 元の要素のレプリカが空のスペースに追加されます。![copy-paste_paste-element_outcome](https://github.com/user-attachments/assets/523d51e2-fcbc-4a98-9ecc-8d976753e6ce)


##### **既存の要素の下に要素を貼り付ける (Paste the element below an existing element)**

1.  宛先のワークブックを `Explore` または `Edit` モードで開き、既存の要素を選択するか、カーソルを合わせます。
2.  要素のツールバーで、`More` をクリックして要素メニューを開き、`Paste element below` を選択します。![copy-paste_paste-element-below](https://github.com/user-attachments/assets/5489a4c4-22d1-4600-b01d-5463c79f54db)
元の要素のレプリカが既存の要素の下に追加されます。
![copy-paste_paste-element-below_outcome](https://github.com/user-attachments/assets/e79d6f25-42e6-4235-b7d0-ca190c264516)

#### **よくある質問 (Frequently asked questions)**

##### **`Copy/Paste element` アクションと `Duplicate` アクションはどのように違いますか？それぞれいつ使用すべきですか？**

| | 複製 (Duplicate) | 要素のコピー/ペースト (Copy/Paste element) |
| :--- | :--- | :--- |
| **アクションタイプ** | 単一ワークブックのアクション | ワークブック間のアクション |
| **コピーされる内容** | 元の要素のみ | 元の要素 + リネージ |
| **宛先** | 現在のワークブック/ページ | 任意のワークブック/ページ |
| **リネージの関連付け** | 元の要素と複製は同じリネージを参照 | 元の要素とレプリカは別のリネージを参照 |

要素メニューで `Duplicate` を選択すると、Sigmaは同じワークブックの同じページにある元の要素の真下に即座に複製を追加します。元の要素が子要素の場合、複製はそのリネージを共有します。言い換えれば、元の要素とその複製はワークブック内の同じ親要素を参照します。親要素に適用された変更は、元の要素とその複製に反映されます。この機能は、元の要素を含む同じワークブック内に複製を作成する必要がある場合に推奨されます。

要素メニューで `Copy element` を選択すると、Sigmaは要素をブラウザにコピーします。その後、`Paste element` を選択して、コピーされた要素のレプリカを組織全体の任意のワークブックやページに追加できます。元の要素が子要素の場合、そのリネージも宛先のワークブックページにコピー＆ペーストされます。この場合、元の要素とそのレプリカは関連付けが解除され、同じリネージを共有しません（それらは別々の親要素を参照します）。この機能は、元の要素を別のワークブックに複製する必要がある場合に推奨されます。

##### **子要素をコピーしたが、その親要素がワークブックの別のページに存在する場合、Sigmaは宛先で親要素を複製しますか？**
はい。親要素が元のワークブックのどこにあっても、要素の完全なリネージがコピーされます。ただし、宛先のワークブックでは、子要素と親要素は同じページに貼り付けられます。

##### **ある要素をコピーして、別の組織のワークブックに貼り付けることはできますか？**
いいえ。要素は、同じSigma組織で作成されたワークブック間でのみコピー＆ペーストできます。

##### **コントロール要素は、要素と一緒にコピー＆ペーストされますか？**
はい。元の要素とそのリネージに影響を与えるほとんどのコントロール要素は、宛先のワークブックページにコピー＆ペーストされます。例外は、パラメータコントロールがカスタムSQLソースを持つ要素に影響を与える場合に発生します。詳細については、カスタムSQL要素のコピー＆ペーストに関する次の質問を参照してください。

##### **カスタムSQL要素をコピー＆ペーストできますか？**
はい。カスタムSQLソースを持つ要素は、それが元の要素であれ、そのリネージの一部であれ、コピー＆ペーストできます。関連するパラメータコントロールはカスタムSQL要素と一緒に複製されませんが、別々にコピー＆ペーストできます。宛先のワークブックでは、カスタムSQL要素は、コピーされたコントロール要素または同じコントロールIDを持つ既存のパラメータコントロールに自動的に再マッピングされます。

##### **異なるワークブック間で要素をコピー＆ペーストした場合、権限はどのように適用されますか？誰が要素のデータを閲覧できますか？**
要素のデータを閲覧できるかどうかは、ユーザーのデータソースへのアクセス権に依存します。特定の要素のデータソース（ソースデータセットまたは接続テーブル）へのアクセス権がないユーザーとワークブックを共有した場合、そのユーザーは共有されたワークブック内でのみその要素のデータを閲覧できます。もしそのユーザーが要素をコピーして別のワークブックに貼り付けた場合、レプリカは宛先のワークブックページにデータをロードせず、Sigmaはそのユーザーにアクセス権がないことを通知します。

##### **要素のフィルターは、コピー＆ペーストされたときに引き継がれますか？**
はい。元の要素にコピー時に既にフィルターが適用されている場合、それらのフィルターは宛先のワークブックページのレプリカにも適用されます。これは、元の要素のリネージの一部としてコピー＆ペーストされる親要素にも適用されます。

##### **ワークブックのページ全体をコピー＆ペーストできますか？**
はい。詳細は「[ワークブックのページをコピー＆ペーストする](https://help.sigmacomputing.com/docs/copy-workbook-pages)」を参照してください。

### 4-2-7. ワークブックのレイアウトをデザインする (Design workbook layouts)

ワークブックの開始状態は、要素やコンテナを追加・配置したり、テーマや色の設定を管理したりできる、空白のキャンバスです。

ワークブックのレイアウトをカスタマイズする方法は複数あります。例えば：
* ページを追加して、分析をコンセプトごとにグループ化する
* 要素を追加して、データ、インタラクティビティ、フィルタリングを追加する
* テーマやフォントなどのワークブック設定を変更して、会社のブランディングに合わせる
* ページ上の要素のサイズを変更・配置して、よりクリーンなワークブックを作成する
* 不要なスペースを削除したり、パディングを追加したりするなど、ベストプラクティスを念頭に置いて最適なレイアウトをデザインする

また、要素をグループ化するためにコンテナを追加したり（「[Organize workbook layouts with containers](https://help.sigmacomputing.com/docs/organize-workbook-layouts-with-containers)」を参照）、アプリのような体験を作成するためにモーダルを追加したりすることもできます（「[Add a modal to a workbook](https://help.sigmacomputing.com/docs/create-and-manage-modals)」を参照）。

#### **ユーザー要件 (User requirements)**

レイアウトを変更するには、個々のワークブックに対する`Can edit`の[ワークブックアクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。

#### **ワークブックにページを追加する (Add pages to a workbook)**

ワークブックは複数のページを含むことができます。これらのページを使用して、分析を異なるコンセプトやコーホートにグループ化したり、「ダッシュボード」として機能させたりすることができます。ページを追加するには、ワークブックを編集中であることを確認し、`+ Add page` を選択します。

#### **ワークブックのページに要素を追加する (Add elements to a workbook page)**

要素を使用して、データ、UI機能、またはコントロールをワークブックのページに追加します。様々な要素の追加と構成に関する詳細は、「[Create a data element](https://help.sigmacomputing.com/docs/create-a-data-element)」、「[Create and manage a control element](https://help.sigmacomputing.com/docs/create-and-manage-control-elements)」、または「[Create a UI element](https://help.sigmacomputing.com/docs/intro-to-ui-elements)」を参照してください。

ワークブックに最初の要素を追加すると、スナップ式のグリッドが表示され、要素を好みに合わせて配置できます。

#### **異なるデバイスレイアウトのプレビューと編集 (Previewing and editing different device layouts)**

ワークブックは、モバイルとデスクトップの両方のレイアウトをサポートしています。ワークブックのデバイスビューを切り替えるには、編集中に `Publish` メニューを選択し、`Desktop` または `Mobile` を選択します。Sigmaのワークブックはレスポンシブフレームワーク上に構築されているため、小さな画面で表示すると、ワークブックのレイアウトは自動的にモバイルフレンドリーなレイアウトに適応します。

#### **ワークブックのページ上で要素を配置する (Arrange elements on a workbook page)**

ワークブックのページ上で要素のサイズを変更したり、再配置したりするには、複数の方法があります。
* **要素のサイズを変更する:** 要素をクリックし、ドラッグハンドルを引いてサイズを変更します。
* **要素を移動する:** 要素を選択してドラッグし、移動します。
* **一度に複数の要素を選択する:** `⌘ Command` + `Click` (Mac) または `Ctrl` + `Click` (Windows)で複数の要素を選択するか、選択したい要素の上でカーソルをクリック＆ドラッグします。その後、要素をグループとして移動できます。
* **要素の位置とサイズを交換する:** ある要素を別の要素の上にドラッグ＆ドロップして、それらの位置とサイズを交換します。![58aee0d5fb1a19d0c920ecc14c4706353bc0b23a6d1a1ff3dcb8d4e825c92dae-swap_gif](https://github.com/user-attachments/assets/a1fad53d-fa3b-4b1c-a08f-ce170d84ff44)

* **要素間に要素を挿入する:** ある要素を他の2つの要素の間にドラッグ＆ドロップします。

#### **ワークブックページの空白とパディングを編集する (Editing whitespace and padding on a workbook page)**

不要なスペースを削除したり、要素をより近づけたり、追加のパディングを加えたりすることで、より最適なレイアウトをデザインできます。

よりクリーンなワークブックのために、ワークブックページの空白を追加、削除、または分割するには：
* **要素間の垂直スペースを追加または削除する:** ワークブックの左端にカーソルを合わせ、リサイザーハンドルが表示されるまで待ちます。ハンドルを上下にドラッグして、2つの要素間の垂直スペースを増減させます。
* **空きスペースを削除する:** 2つの要素間の空きスペースにカーソルを合わせ、`Trim space` ボタンが表示されるまで待ちます。それを選択して、間のスペースを削除します。
* **要素間でスペースを分割する:** 別の要素をドラッグ＆ドロップして、ある要素が使用しているスペースを共有または分割できます。下にある要素が占めるスペースは、両方の要素を収容するのに十分な大きさでなければなりません。![3a57f8ffa7b8d85e584def8be532eb91beca028b37f6c8b390d1eb43aaac2f42-split_example](https://github.com/user-attachments/assets/21bfe5ea-7e12-4688-ba77-0df664b0aa25)


また、ページ上の空白を増やすために要素にパディングを追加することもできます。「[Customize element background and styles (Beta)](https://help.sigmacomputing.com/docs/customize-element-background-and-styles-beta#add-padding-to-an-element)」の「Add padding to an element」を参照してください。

#### **ワークブック設定を変更する (Change workbook settings)**

テーマ、色、フォントなどのグローバルなワークブック設定を管理します。編集中に、ワークブックの背景のどこかをクリックして `Settings` タブを開き、`Workbook Settings` を選択します。詳細は、「[Workbook settings overview](https://help.sigmacomputing.com/docs/workbook-settings-overview)」を参照してください。

### 4-3-1. データ要素を作成する (Create a data element)

[ワークブック](https://help.sigmacomputing.com/docs/workbooks-overview)は多くの[要素タイプ](https://help.sigmacomputing.com/docs/intro-to-element-types)をサポートしています。データ要素は、データソースから直接構築される要素で、[テーブル](https://help.sigmacomputing.com/docs/create-and-manage-tables)、[ピボットテーブル](https://help.sigmacomputing.com/docs/create-and-manage-pivot-tables)、および[チャート](https://help.sigmacomputing.com/docs/build-a-chart)が含まれます。

各タイプのデータ要素はデータを異なる方法で表示しますが、基盤となるデータは常に表形式で列ベースです。可視化またはピボット化されたデータの構造を理解するには、そのデータ要素の基盤となるデータを表示します。「[View underlying data](https://help.sigmacomputing.com/docs/view-underlying-data)」を参照してください。
<img width="2120" height="1106" alt="1b9a491-1" src="https://github.com/user-attachments/assets/1099772c-e3cf-47ea-8fae-918ba0821d45" />

#### **データ要素のデータソース (Data sources for data elements)**

ワークブックを作成する際、様々なデータソースから要素を追加できます。いつでも新しいソースを追加でき、ワークブックごと、またはワークブックのページごとに単一のソースに制限されることはありません。

利用可能なデータソースには、接続されたクラウドデータウェアハウス（CDW）のテーブル、Sigmaのデータモデルまたはデータセット、アップロードしたCSV形式のファイル、SQLコマンド、他のワークブックのデータ要素などが含まれます。

いくつかの異なるソースからデータ要素を作成できます。
* 新しいソース。
* ワークブックで既に使用中のソース。
* 既存のデータ要素。別の要素から要素を作成するには、「[Create a data element from an existing element on the canvas](#create-a-data-element-from-an-existing-element-on-the-canvas)」を参照してください。

#### **上流の変更の影響 (Effects of upstream changes)**

データソースに加えられた変更は、そのデータソースに依存する子要素に影響を与える可能性があります。例えば、棒グラフ要素がデータソースとしてテーブル要素に依存している場合、テーブル要素から列を削除すると、その列は棒グラフ要素からアクセスできなくなります。列を非表示にすると、その列はデフォルトでは利用できなくなり、棒グラフにはソース列としてのみアクセス可能になります。

ワークブックを構築し、データ要素を作成する際には、データソースの再利用性を考慮してください。
* ワークブック間で再利用するために、データ要素をデータモデルに変換する。
* ソーステーブルに計算列やフィルターを作成する。
* 予期しないデータの変更をトラブルシューティングする際に、要素のリネージを確認する。

#### **要件 (Requirements)**

データ要素を作成するには、個々のワークブックに対する`Can edit`または`Can explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。
ワークブックは`Edit`モードまたは`Explore`モードである必要があります。「[Workbook modes overview](https://help.sigmacomputing.com/docs/workbook-modes-overview)」を参照してください。
CSVのアップロードやカスタムSQLの記述には、`Upload CSV`または`Write SQL`権限が有効になっているアカウントタイプを割り当てられている必要があります。「[Account types](https://help.sigmacomputing.com/docs/account-type-and-license-overview)」を参照してください。

#### **ワークブックのページにデータ要素を追加する (Add a data element to a workbook page)**

ワークブックのページにデータ要素を追加するには、以下を実行します。

1.  カスタマイズまたは編集のためにワークブックを開きます。
2.  `Add element`バーで、追加するものを選択します。テーブルまたはピボットテーブルを追加するには、`Data`を選択し、関連するオプションを選択します。チャートを追加するには、`Charts`を選択し、追加したいチャートを選択します。![6548f3d62f2bf56e028d80d33d25cff17dc6240d89c119c06d5f1822132bb083-element-bar-charts](https://github.com/user-attachments/assets/926712ca-999c-47c8-b835-e6b8742d129d)
<img width="417" height="478" alt="6548f3d62f2bf56e028d80d33d25cff17dc6240d89c119c06d5f1822132bb083-element-bar-charts" src="https://github.com/user-attachments/assets/9ad95dab-83b4-4a47-8364-6a4a565495a1" />

3.  データソースを選択します。データソースをすぐに追加するか、プレビューして特定の列を選択して追加することができます。
    * データモデル、データベースまたはカタログのテーブル、データセット、または他のワークブック要素をデータソースとして使用するには、検索を実行するか、現在のワークブックから`Elements`を参照するか、`Tables and Datasets`からテーブル、データモデル、またはデータセットを選択します。
        > 💡
        > 利用可能なデータソースにカーソルを合わせ、`Preview`を選択してデータソースの列と値を表示します。ワークブックで既に使用中のソースや、アクセス権のある他のワークブックで使用中のソースは、異なるアイコンで表示されます。リネージアイコン()にカーソルを合わせると、現在のワークブックで使用中のソースを特定できます。
    * データソースをプレビューする場合、データソース内の異なる列を選択または選択解除し、その後`Add`を選択してデータソースを追加できます。
    * CSV形式のファイルをアップロードするには、`CSV`を選択します。
    * データプラットフォームからデータを取得するためにカスタムSQLを記述するには、`SQL`を選択します。「[Write custom SQL](https://help.sigmacomputing.com/docs/write-custom-sql)」を参照してください。
    * データソースを組み合わせるには、`Join`または`Union`を選択します。「[Join data in workbooks](https://help.sigmacomputing.com/docs/join-data-in-workbooks)」を参照してください。
    * 既存のデータソースを転置するには、`Transpose`を選択します。「[Transpose a table](https://help.sigmacomputing.com/docs/transpose-a-table)」を参照してください。![90a6e3737967ff9d7b37c7b35a3d928aa62fb03ae773b312f7b13fc94174e1f9-source-picker](https://github.com/user-attachments/assets/982885ca-c810-4004-8f9a-dc2aba2ba85d)

要素のデータソースを選択すると、新しい要素がページに表示され、その要素のエディタパネルが開きます。

#### **キャンバス上の既存の要素からデータ要素を作成する (Create a data element from an existing element on the canvas)**

ワークブックページのテーブル、ピボットテーブル、または入力テーブルから子データ要素を作成できます。例えば、テーブル要素からチャートを作成します。

1.  データソースとして使用したい要素にカーソルを合わせます。
2.  `Create child element`を選択して、選択した要素に基づいて子要素を作成します。
3.  要素タイプ（`Chart`, `Table`, `Pivot table`, `Linked input table`）を選択します。
4.  新しい要素がページに表示され、その要素のエディタパネルが開きます。

#### **要素のデータソースを特定・編集する (Identify and edit an element's data source)**

データ要素のデータソースを特定し、変更を加えるには、要素を選択し、エディタパネルの`Properties`タブを確認します。

1.  カスタマイズまたは編集のためにワークブックを開きます。
    > 💡
    > エディタパネルが表示されていない場合は、`Show panels` ()をクリックします。
2.  ワークブックキャンバスで要素を選択し、エディタパネルの`Properties`タブを選択します。<img width="344" height="214" alt="4baa4ca6ff00a9bf2c2b4ff1fa358a53906f2198677fe69a0bc409b9ed4eea94-change-groupings" src="https://github.com/user-attachments/assets/9998fdb3-a1e1-4cd3-93f7-39670e6f0d26" />

3.  データソースは`Data source`の下に表示されます。
4.  選択した要素のデータソースを表示、変更、または変換するには、データソース名の隣にある下矢印()を選択します。「[Change the data source for a workbook or element](https://help.sigmacomputing.com/docs/change-the-data-source-for-a-workbook-or-element)」を参照してください。<img width="340" height="232" alt="41b8041f63eb1869e65ef605b02c3ce4e4267acfa6a7fdd2d6aeea4a4126ea0d-change-groupings-open" src="https://github.com/user-attachments/assets/fa04a198-2b52-45cf-aeb4-09e65b029af5" />


#### **データソースのグルーピングレベルを変更する (Change the grouping level of a data source)**

グループ化されたテーブルがデータ要素のデータソースとして使用される場合、デフォルトではテーブルのすべてのソース列がデータソースとして使用されます。特定のグルーピングレベルの列のみを使用するなど、テーブルで利用可能な列を変更するには、データソースの粒度を変更します。

1.  テーブルを選択し、エディタパネルの`Properties`タブを選択します。
2.  `Data source`で、ソーステーブルと`Source grouping`オプションを確認します。![4baa4ca6ff00a9bf2c2b4ff1fa358a53906f2198677fe69a0bc409b9ed4eea94-change-groupings](https://github.com/user-attachments/assets/e5592c7d-4b81-43b0-8e9d-10cfecb3b6d0)

3.  列名を開いて利用可能な粒度オプションを確認し、含めたい列を選択します。下位レベルのグルーピングオプションには、上位レベルのグルーピングオプションからの列が含まれます。すべての列を表示したい場合は、`All source columns`を選択します。![41b8041f63eb1869e65ef605b02c3ce4e4267acfa6a7fdd2d6aeea4a4126ea0d-change-groupings-open](https://github.com/user-attachments/assets/2156c026-7559-4673-87f6-a6eb45153b85)
要素は、利用可能なソース列を反映して更新されます。

### 4-3-2. ワークブックまたはデータモデルで関連する列を使用する (Use related columns in a workbook or data model)

ワークブックまたはデータモデル内のデータ要素のデータソースが、一つ以上のリレーションシップを持つデータモデルテーブルである場合、関連するテーブルからデータ要素に列を追加できます。作成するすべての子要素も、関連する列にアクセスできます。

> 💡
> まずプライマリソース要素から子テーブルを作成すれば、同じデータモデル内で作成されたリレーションシップを使用できます。

#### **要件 (Requirements)**

* データソースは、一つ以上のリレーションシップが定義されたデータモデル内のテーブル要素である必要があります。
* あなたはワークブックまたはデータモデルの所有者であるか、そのドキュメントに対する `Can explore` または `Can edit` の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **データ要素に関連する列を追加する (Add a related column to a data element)**

ワークブックまたはデータモデル内のデータ要素のデータソースに一つ以上のリレーションシップが定義されている場合、関連する列をデータ要素に追加できます。

1.  ワークブックをカスタマイズするか、ワークブックまたはデータモデルを編集用に開きます。
2.  データ要素を選択します。
3.  エディタパネルで、列の `+` (Add columns...) を選択します。
4.  メニューで、`Add source columns...` を選択して `Source columns` リストを開きます。![910f668d28a67aa902675f0aa4737b87b63ffedcd92163fad0d59e67033d1bce-dm-rel-src-column](https://github.com/user-attachments/assets/17892a0e-d4cd-4835-8bfa-0ddb26fc351e)

5.  `Source columns` リストで、データモデルのリレーションシップを通じてリンクされたテーブルから利用可能な列を確認します。直接関連するテーブルの列だけでなく、継承されたリレーションシップからの列も表示できます。
6.  列のチェックボックスを選択して、データ要素に追加します。
7.  関連する列は、`Column Name (Relationship Name)` というタイトルでデータ要素に表示されます。

#### **数式で関連する列を使用する (Use a related column in a formula)**

ワークブック内のデータ要素のデータソースに一つ以上のリレーションシップが定義されている場合、そのデータ要素の計算列の数式で関連する列を使用することもできます。

> 📘
> 数式で使用する前に、関連する列をデータ要素に追加する必要はありません。

1.  ワークブックを探索するか、編集用に開きます。
2.  データ要素を選択します。例えば、あるレンタルバイクのドッキングステーションから別のステーションへのバイクトリップのテーブル `TRIP` などです。
3.  要素内、またはエディタパネルで、`+` (Add column...) を選択します。
4.  数式バーに、関連する列を参照する数式を入力します。入力中に、関連する列がオートコンプリート候補のリストに表示されます。![1d44a0ada1842a8cc8e9dec051b29abdf5ba111b054e0f8af7f41704a9eed352-dm-formula-auto](https://github.com/user-attachments/assets/d494265f-623b-42ed-9a0a-72406eb65949)
例えば、出発ステーションでのドッキングステーションの利用可能性を評価するには、以下の数式を記述することがあります。
    ```
    If([TRIP/Start Station Details/Dock Count] > 15, "high availability", [TRIP/Start Station Details/Dock Count] = 15, "medium availability", [TRIP/Start Station Details/Dock Count] < 15, "low availability")
    ```
結果のテーブルには、`Start Station Dock Availability` という名前の計算列が含まれます。<img width="1164" alt="77a045d38b587c5fc1cbe87d3091c90854da8a75273a77a3bd02aee757d629a0-Screenshot_2025-03-26_at_5 45 43_PM" src="https://github.com/user-attachments/assets/41cc196a-5f48-498e-8537-b3f0dc8e3e09" />

### 4-3-3. ワークブックでリンクされた列を使用する (Use linked columns in workbooks)

[データセットにリンク](https://help.sigmacomputing.com/docs/dataset-links)がある場合、ワークブックでデータを分析・探索する際に、リンクされた列を使用できます。

#### **ユーザー要件 (User requirements)**

ワークブックでリンクされた列を使用するには、あなたがワークブックの所有者であるか、`Can explore` または `Can edit` のワークブック権限を付与されている必要があります。

#### **ワークブックでリンクされた列を使用する (Use linked columns in workbooks)**

リンクは、Sigma内で2つのデータソース間に作成される、列ベースのリレーションシップです。これにより、あるデータソースが別のデータソースと共有する列に基づいて、一方のデータソースからデータにアクセスできます。

クラウドデータウェアハウス（CDW）のテーブルは、他のCDWテーブルにリンクできます。Sigmaのデータセットは、他のデータセットにリンクできます。そして、CDWテーブルはデータセットにリンクできます。一つのデータソースは、複数の他のデータソースへのリンクを持つことができます。
<img width="1587" alt="20a1aa7-1" src="https://github.com/user-attachments/assets/1b4a7a64-e35f-49af-92ef-95fbd898bc76" />

##### **ワークブックでのリンクのアクセシビリティ (Link accessibility in workbooks)**

リンクは、リンクされた列を含むデータソースから直接作成された[データ要素](https://help.sigmacomputing.com/docs/create-a-data-element)を通じてのみ、ワークブックでアクセスできます。CDWまたはデータセットの親からリンクを継承したデータ要素の子要素は、それらのリンクを引き続き継承しません。

これは、データ要素からリンクされた列にアクセスしたい場合、(1) リンクを含む元のデータソースからその要素を作成するか、あるいは (2) [必要な列を](https://help.sigmacomputing.com/docs/dataset-worksheet-columns#add-a-new-column)親要素に追加して、子が直接継承できるようにする必要があることを意味します。

##### **テーブル要素でリンクから列を追加する (Add columns from a link in a table element)**

テーブル内のリンクされた列は、セル値の薄い青色の背景で識別できます。
1.  リンクされた列のセルをクリックして、リンクのポップアップを開きます。
2.  テーブルに表示したい任意の列の横にあるチェックボックスをオンにします。
![4f8e124-2](https://github.com/user-attachments/assets/9e43ead9-594d-4650-9bed-b9e22e4e1305)

##### **ビジュアライゼーションまたはピボットテーブルでリンクから列を追加する (Add columns from a link in a visualization or pivot table)**

ビジュアライゼーションとピボットテーブル内のリンクされた列は、要素が[最大化](https://help.sigmacomputing.com/docs/maximize-an-element)されている場合にのみアクセス可能です。そこから、基盤となるデータテーブルを通じてリンクにアクセスできます。テーブル要素と同様に、リンクされた列はセル値の青い背景で識別できます。
1.  要素を最大化します。
2.  基盤となるデータテーブルで、リンクされた列の任意のセルをクリックします。
3.  これにより、リンクのポップアップが開きます。
テーブルに表示したい任意の列の横にあるチェックボックスをオンにします。
![6a93b12-3](https://github.com/user-attachments/assets/7f16ba7a-8e4e-47f3-a3b5-e3897dbcd139)

### 4-3-4. ルックアップで列を追加する (Add columns through Lookup)

[ルックアップ](https://help.sigmacomputing.com/docs/lookup)とは、2つのデータ要素間で関連する列を接続し、ある要素から別の要素へデータを注入することを可能にするアクションです。2つの要素は、共通の値を共有する一対の列（各要素から一つずつ）によって結合されます。私たちはこれらの結合列を**結合キー**と呼びます。

ルックアップから作成される列は、`Lookup`関数を使用して追加できます。しかし、明示的に数式を記述することなく、新しいルックアップ列を追加することもできます。この2番目のオプションについて、以下に説明します。

#### **要件 (Requirements)**

この機能を使用するには、個々のワークブックに対する`Can Edit`または`Can Explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。

#### **ルックアップで列を追加する (Add a Column via Lookup)**

* **前提条件:**
    * 少なくとも2つのデータ要素（結合先と結合元）が必要です。
    * 両方の要素は同じワークブック内に存在する必要があります。
    * 両方の要素は同じ接続からソースされている必要があります。
    * 結合先の要素は、結合元の要素の子であってはなりません。

* **ルックアップ経由で列を追加する**
    * **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ページの右上隅にある `Edit` をクリックします。

    1.  列を追加したいデータ要素を選択します。
    2.  任意の列名の隣にあるキャレットアイコンをクリックして、そのメニューを開きます。
    3.  `Add column via lookup` を選択します。
    4.  これにより、`Add Lookup` モーダルが開きます。
        * 最初のセクション「**Which column would you like to add?**」では、以下を選択するよう促されます。
            * ソース要素
            * 新しい列で使用する、ソース要素からの列
            * [任意] 列に適用する集計値
        * 2番目のセクション「**Map two elements**」では、一つ以上の結合キーのセットを定義するよう促されます。
    5.  `Select element` の下で、ソース要素を選択します。
        * 要素は、そのワークブックのページごとに整理されています。
    6.  `Column to add` の下で、新しい列で使用したい列を選択します。
    7.  [任意] `aggregate` の下で、列の値に適用する集計関数を選択します。
        * *注：内部的には、集計はルックアップをロールアップに変換します。*
    8.  `Map two elements` の下で、結合キーとして使用する各データ要素から列を選択します。
    9.  [任意] 追加の結合キーのペアを追加するには、`+ add another mapping` をクリックし、ステップ7を繰り返します。
 
### 4-3-5. 期間比較分析の作成と編集 (Create and edit period-over-period analysis)

Sigmaの期間比較分析構築のためのガイド付きワークフローは、時間経過に伴うパフォーマンスを評価するための迅速で便利な方法を提供します。複雑なカスタム数式を入力することなく動的な期間比較を生成し、その結果を簡単に視覚化して、トレンド、パターン、異常を特定できます。

このドキュメントでは、データ要素（テーブル、ピボットテーブル、およびビジュアライゼーション）で組み込みの期間比較機能を使用する方法について説明します。

#### **ユーザー要件 (User requirements)**

Sigmaの組み込み期間比較機能を使用するには、以下が必要です。
* `Edit Workbook`および/または`Explore Workbook`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがワークブックの所有者であるか、`Can explore`または`Can edit`の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **主要な用語 (Key terms)**

このドキュメントでは、以下の用語が使用されます。

* **現在の期間 (Current period)**
    比較の開始点として使用される参照期間。
* **比較期間 (Comparison period)**
    比較の終点として使用されるルックバック期間。
* **期間の値 (Period value)**
    現在の期間のメトリック値。
* **比較値 (Comparison value)**
    比較期間のメトリック値、または現在と比較期間を比較するために使用される値（比較値のタイプによる）。
* **比較値のタイプ (Comparison value type)**
    生成される比較のタイプ（差、%差、または値）。

#### **期間比較を構築する (Build a period-over-period comparison)**

Sigmaのガイド付きワークフローで期間比較分析をすぐに始めましょう。あなたの入力は、必要に応じて補強、編集、視覚化できる比較グルーピングを生成します。

1.  ワークブックを`Explore`または`Edit`モードで開き、更新したいデータ要素を選択します。ビジュアライゼーションで作業している場合は、要素を[最大化](https://help.sigmacomputing.com/docs/maximize-an-element)して基盤となるデータテーブルを表示および編集します。
2.  テーブルで、既存の列ヘッダーのキャレット()をクリックして列メニューを開きます。
3.  `Add column via`にカーソルを合わせ、`Period over period comparison`を選択します。![pop_add-column-via-period-over-period-comparison](https://github.com/user-attachments/assets/ba5d5fd4-4844-45df-9308-4e234f961713)
<img width="1143" height="469" alt="pop_add-column-via-period-over-period-comparison" src="https://github.com/user-attachments/assets/aa1ae932-e9e8-42ed-9977-015e729ea5b8" />
4.  `Add comparison`モーダルで、比較を構成し、`Done`をクリックします。
    * **Compare field:** 比較したいメトリックまたは変数を含む列を選択します。
    * **Aggregate:** 期間の値と比較値を計算するための集計方法を選択します。
    * **Using date column:** 現在および比較期間の集計に使用する[日付列](https://help.sigmacomputing.com/docs/supported-data-types-and-formats#date)を選択します。
    * **Comparison time frame:** ルックバックと日付の粒度を決定するための比較期間を選択します。
    * **Output:** 一つ以上の比較値のタイプを選択します。
        * **Difference (差):**
            期間比較の差を生の数値として。
        * **% difference (%差):**
            期間比較の差をパーセントとして。
        * **Value (値):**
            比較期間の合計メトリック値を生の数値として。
![pop_add-comparison](https://github.com/user-attachments/assets/01b77df3-8472-4810-b887-b58c2d0ef680)
<img width="1219" height="490" alt="pop_add-comparison" src="https://github.com/user-attachments/assets/7091516c-e90c-4859-89f9-1e11f9875546" />

テーブル要素では、Sigmaは現在の期間、期間の値、および比較値を含む期間比較のグルーピングを作成します（以下のスクリーンショットで示されています）。
ピボットテーブルとビジュアライゼーションでは、Sigmaは切り捨てられた日付（選択された比較期間に基づく）と比較値を含む基盤となるデータ列を作成します。その後、新しい列を使用して要素のプロパティを構成できます。

> 📘
> データ要素のタイプに関わらず、`Output`フィールドで複数の比較値タイプを選択すると、Sigmaはそれぞれに対して個別の列を生成します。
![pop_add-comparison_results](https://github.com/user-attachments/assets/2d97c64b-ee13-4dda-909e-5899b70c5bae)
<img width="1143" height="469" alt="pop_add-comparison_results" src="https://github.com/user-attachments/assets/d3269960-1fd4-4807-83a9-6daf7465648f" />

> 💡
> KPIチャートで期間比較を視覚化しましょう。詳細は、「[Build a KPI chart](https://help.sigmacomputing.com/docs/build-a-kpi-chart)」を参照してください。

#### **比較値を追加する (Add a comparison value)**

既存の期間比較グルーピングに比較値を追加します。

1.  テーブルで、比較したい期間の値を含む列を探し、列ヘッダーのキャレット()をクリックして列メニューを開きます。
2.  `Add column via`にカーソルを合わせ、`Comparison time frame`セクションでオプションを選択します。
    > 📘
    > 利用可能なオプションは、既存の比較の日付の粒度に依存します。例えば、期間の値が月ごとに集計されている場合、他の月次期間とのみ比較できます。この場合、`Comparison time frame`のオプションには`Last month`、`Same month last quarter`、`Same month last year`が含まれます。`Last year`や`Same week last quarter`のような他の比較は、比例した期間比較を提供しないため利用できません。
<img width="1143" height="469" alt="pop_add-column-via-comparison-time-frame" src="https://github.com/user-attachments/assets/56e401e9-a549-4034-9c1a-100b883d73ff" />

Sigmaは同じグルーピングに新しい比較値の列を追加します。
![pop_add-column-via-comparison-time-frame](https://github.com/user-attachments/assets/82955489-7a5c-4cc5-97ab-2a43a62c9e0e)
<img width="1143" height="469" alt="pop_add-column-via-comparison-time-frame_results" src="https://github.com/user-attachments/assets/764d674a-a3e0-4526-940e-d2c33077853a" />

#### **既存の比較を編集する (Edit an existing comparison)**

既存の比較の期間、値のタイプ、および集計方法を迅速に変更します。

> 💡
> Sigmaは`DateLookback`関数を使用して比較値を計算します。比較期間、比較値のタイプ、および集計方法以外の変更を行うには、列のSigmaが生成した数式を編集してください。

1.  テーブルで、変更したい比較値を含む列を探し、列ヘッダーのキャレット()をクリックして列メニューを開きます。
2.  比較期間、比較値のタイプ、または集計方法を編集します。
    * 比較期間または比較値のタイプを変更するには、`Edit comparison`にカーソルを合わせ、異なる`Comparison time frame`または`Output`オプションを選択します。![pop_edit-comparison](https://github.com/user-attachments/assets/67b1d3c4-2b44-46f9-92fe-6ddabf87f522)![pop_edit-comparison_results](https://github.com/user-attachments/assets/7a02c168-0fe7-47b1-a90f-6a037af830bc)
<img width="1255" height="489" alt="pop_edit-comparison" src="https://github.com/user-attachments/assets/febc9c47-f37f-44b8-87e7-21f1f9daa2c7" />
<img width="1143" height="469" alt="pop_edit-comparison_results" src="https://github.com/user-attachments/assets/e5dca5a4-4ae8-4594-b19a-34da582dbad0" />
    * 集計方法を変更するには、`Set aggregate`にカーソルを合わせ、異なるオプションを選択します。![pop_set-aggregate]![pop_set-aggregate_results](https://github.com/user-attachments/assets/6e19707d-2ddc-429a-ab0b-cf4a5427cb19)
(https://github.com/user-attachments/assets/de7873ac-b12e-4c28-b84f-fd8d27383d2f)
<img width="1265" height="471" alt="pop_set-aggregate" src="https://github.com/user-attachments/assets/30ecc20e-e5e5-448b-a988-a55fc34d90d6" />
<img width="1143" height="469" alt="pop_set-aggregate_results" src="https://github.com/user-attachments/assets/8cfbe669-b64e-421f-8720-cdfaaef5ba12" />

### 4-3-6. 列をフォルダに整理する (ベータ版) (Organize columns into folders (Beta))

> 🚩
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このページは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

データモデルやワークブックのデータ要素で作業する際、列をフォルダに整理し、関連するグループに列をネストさせることができます。

列をフォルダに整理すると、以下のことができます。
* 好きなだけ列のフォルダを作成する。
* 他のフォルダ内にフォルダをネストする。
* 列のフォルダをテーブルのグルーピングやチャートの軸に追加する。
* フォルダとその列を削除または複製する。

データセットやウェアハウステーブルの列に対してフォルダを作成することはできません。

フォルダは子要素や下流の要素で利用可能です。データモデルのテーブルで列のフォルダを作成すると、そのテーブルをデータソースとして使用するデータ要素にはそのフォルダが表示されます。

> 📘
> 子要素が作成された後に作成されたフォルダは自動的には表示されませんが、`+` (Add columns...) を選択し、次に `Add source columns…` を選択してソース列リストを開くことで追加できます。

#### **要件 (Requirements)**

ワークブックまたはデータモデルに対する`Can edit`または`Can explore`のアクセス権が必要です。

#### **新しいフォルダに列を追加する (Add columns to a new folder)**

列メニューから、または列のリストから、新しいフォルダに列を追加できます。

1.  編集のためにドキュメントを開くか、ワークブックのカスタマイズを開始します。
2.  データ要素を選択します。
3.  一つ以上の列を選択し、下矢印 を選択して列メニューを開き、`Move to new folder` を選択します。
4.  新しいフォルダが表示されます。列リストの異なる部分で列を選択した場合、フォルダとその列は、最初に選択した列と同じ場所に表示されます。
    > 💡
    > `+` > `Add folder` をクリックして空のフォルダを追加し、その後で列をフォルダにドラッグ＆ドロップすることもできます。

#### **既存のフォルダに列やフォルダを追加する (Add columns or folders to an existing folder)**

既存のフォルダに追加する列やフォルダを選択できます。

1.  編集のためにドキュメントを開くか、ワークブックのカスタマイズを開始します。
2.  データ要素を選択し、エディタパネルで列のリストを探します。
3.  既存のフォルダに追加したい列やフォルダを選択し、選択した列やフォルダをフォルダにドラッグ＆ドロップします。

#### **フォルダから列を削除する (Remove columns from a folder)**

フォルダから列を削除するには：
1.  フォルダを開き、各列をフォルダの外にドラッグ＆ドロップします。
2.  下矢印 を選択してフォルダメニューを開き、`Delete folder` を選択します。
    > 🚧
    > 列を移動せずにフォルダを削除すると、その列もデータ要素から削除されます。削除された列を再度追加するには、`+` (Add columns...) を選択し、次に `Add source columns...` を選択してソース列リストを開きます。

#### **列フォルダを管理する (Manage a column folder)**

列のリストでフォルダを右クリックすると、以下のタスクを実行できます。
* **フォルダの名前を変更する**
    > 💡
    > フォルダ名をダブルクリックして名前を変更することもできます。
* **フォルダと、それに含まれるすべての列およびフォルダを削除する。** 削除された列をデータ要素に再度追加するには、`+` (Add columns...) を選択し、次に `Add source

### 4-4-1. テーブルの作成と管理 (Create and manage tables)

テーブルは、Sigmaでデータと対話するための基本的な方法です。接続されたデータウェアハウス、Sigmaのデータモデルからテーブルを追加したり、CSV形式のファイルをアップロードしたりできます。

従来の表計算ツールに慣れている方は、セル単位でデータや数式を扱うことに慣れているかもしれません。Sigmaのテーブルは非常にスプレッドシートに似ていますが、データはセルレベルではなく列レベルで管理されます。その結果、計算や書式設定の変更は、列内のすべてのセルに適用されます。

列レベルでデータを管理することで、一貫性と正確性が保証され、大規模なデータセット全体でよくあるエラーを防ぐのに役立ちます。

Sigmaでは、[テーブル内の列をグループ化する](https://help.sigmacomputing.com/docs/create-and-manage-tables#group-columns-in-a-table)こともでき、複雑なピボットテーブルを作成することなく、異なるレベルで簡単に集計を実行できます。

#### **テーブルを作成する (Create a table)**

テーブルを作成するには、データ要素を作成する手順に従ってください。「[Create a data element](https://help.sigmacomputing.com/docs/create-a-data-element)」を参照してください。

テーブルを作成した後、列を追加して分析を拡張できます。
* [テーブルに計算列を追加する](#add-a-calculated-column-to-a-table)
* [テーブルにデータソース列を追加する](#add-a-data-source-column-to-a-table)
* [ルックアップで列を追加する](https://help.sigmacomputing.com/docs/add-columns-through-lookup)
* [期間比較分析で列を追加する](https://help.sigmacomputing.com/docs/create-and-edit-period-over-period-analysis)
* [JSONまたはバリアントデータから列を抽出する](https://help.sigmacomputing.com/docs/extract-columns-from-json-or-variant-data)

#### **テーブルに計算列を追加する (Add a calculated column to a table)**

Sigmaの任意の[関数](https://help.sigmacomputing.com/docs/function-index)を使用して、テーブルに計算列を追加できます。`Profit`と`Sales`列に基づいて`Profit Margin`列を作成するなどの基本的な計算や、`If`を使用した条件付き評価や`Coalesce`を使用したデータクリーニングなどのより複雑なタスクを実行できます。

すべての計算は、数式バーを使用して列レベルで実行されます。データ要素内の列を選択し、数式バーを確認することで、列の計算に使用された数式を表示できます。列を選択しない場合、数式バーは空になります。

##### **前提条件 (Prerequisites)**
列を追加するには、ドキュメントに対する`Can edit`または`Can explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。
このアクションはエディタパネルを使用します。まだ行っていない場合は、ドキュメントをカスタマイズまたは編集中にエディタパネルを開いてください。

##### **計算列を追加する (Add a calculated column)**
テーブルに列を追加するには、以下を実行します。
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  `Columns`ヘッダーの隣にある`+ Add column...`をクリックします。
3.  `Add new column`を選択して、テーブルに新しい計算列を追加し、フォーカスを数式バーに移します。
4.  数式バーに数式を入力します。入力中に、候補の関数名と列名が表示されます。
5.  数式の記述が完了したら、キーボードの`Enter`または`Return`を押すか、数式バーの隣にあるチェックマークをクリックして数式を保存します。
6.  列は数式の結果で更新されます。
7.  (任意) デフォルトの列名をダブルクリックするか、列メニュー()を開いて列の名前を変更します。

#### **テーブルにデータソース列を追加する (Add a data source column to a table)**

ワークブックにテーブルを追加する際、データソースのすべての列が含まれていない場合があります。テーブルにデータソース列を追加したり、ソーステーブルの粒度を変更してより多くの列を追加したりできます。

> 💡
> データソースを追加する際、デフォルトでは含まれている列のみがテーブルに追加されます。アンダースコアで始まる名前の列（_column_name）など、一部の列は追加可能ですが、デフォルトでは含まれません。

##### **前提条件 (Prerequisites)**
列を追加するには、ワークブックに対する`Can edit`または`Can explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。
このアクションはエディタパネルを使用します。まだ行っていない場合は、ドキュメントをカスタマイズまたは編集中にエディタパネルを開いてください。

##### **データソース列を追加する (Add a data source column)**
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  `Columns`ヘッダーの隣にある`+ Add column...`をクリックします。
3.  `Add source columns...`を選択して、テーブルのデータソースから列を選択します。
4.  データソースから利用可能な列の完全なリストを確認し、列名の隣にあるチェックボックスを選択してテーブルに追加します。
    > 📘
    > `Unavailable source columns`のリストが表示される場合、あなたのテーブルはグループ化されたソーステーブルに基づいており、グループ化された列のみが含まれている可能性があります。「[Change the granularity of a grouped element data source](https://help.sigmacomputing.com/docs/create-a-data-element#change-the-grouping-level-of-a-data-source)」を参照してください。

#### **テーブル内の列をグループ化する (Group columns in a table)**

テーブル内の列をグループ化して、列内の共通の値に基づいてデータの行を比較します。テーブル内の任意の列を使用してグルーピングを定義でき、複数のグルーピングを定義できます。

グルーピングとは、グループ化した列内の同じ個別値を共有するすべての行のグループを作成し、それらのグループに基づいて集計計算を作成できるデータテーブル内の構造です。

テーブルでグルーピングを使用する詳細な例については、「[Example: Group website analytics by host name and calculate statistics](#example-group-website-analytics-by-host-name-and-calculate-statistics)」を参照してください。

##### **前提条件 (Prerequisites)**
列をグループ化するには、ワークブックに対する`Can edit`または`Can explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。
このアクションはエディタパネルを使用します。まだ行っていない場合は、ドキュメントをカスタマイズまたは編集中にエディタパネルを開いてください。

##### **テーブルにグルーピングを追加する (Add groupings to a table)**
テーブル内の列をグループ化するには、以下を実行します。
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  `Groupings`ヘッダーの隣にある`+ Add grouping...`を選択し、グループ化したい列を選択します。

##### **グルーピングに計算を追加する (Add calculations to a grouping)**
列の各値ではなく、グループの各値に対して集計を計算するには、グルーピングに計算を追加します。
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  グルーピングについて、`Calculations`ヘッダーの隣にある`+ Add calculation...`を選択し、グループに対して集計したい列を選択します。
    * 例えば、グループ内の各`Host Name`に対する`Unique Users`など、一部の計算はグループレベルでのみ関連性があります。

##### **テーブル内のグループを管理する (Manage groups in a table)**
テーブルにグルーピングを作成した後、以下のことができます。
* グループ列のヘッダーまたは値の隣にある`+`または`-`を選択して、グループ化されたデータを展開または折りたたみます。
* 列メニューを開いて`Remove from grouping`を選択することで、グルーピングから列または計算を削除します。
* グルーピング全体を削除するには、`Group by`の隣にある`More` > `Remove grouping`を選択します。
* 折りたたまれた列を非表示にします。「[Hide and show table components](https://help.sigmacomputing.com/docs/format-and-customize-a-table#hide-and-show-table-components)」を参照してください。

#### **テーブル内の列をグループ化する (Group columns in a table)**

テーブル内の列をグループ化して、列内の共通の値に基づいてデータの行を比較します。テーブル内の任意の列を使用してグルーピングを定義でき、複数のグルーピングを定義できます。

グルーピングとは、グループ化した列内の同じ個別値を共有するすべての行のグループを作成し、それらのグループに基づいて集計計算を作成できるデータテーブル内の構造です。

テーブルでグルーピングを使用する詳細な例については、「[Example: Group website analytics by host name and calculate statistics](#example-group-website-analytics-by-host-name-and-calculate-statistics)」を参照してください。

##### **前提条件 (Prerequisites)**
列をグループ化するには、ワークブックに対する`Can edit`または`Can explore`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。
このアクションはエディタパネルを使用します。まだ行っていない場合は、ドキュメントをカスタマイズまたは編集中にエディタパネルを開いてください。

##### **テーブルにグルーピングを追加する (Add groupings to a table)**
テーブル内の列をグループ化するには、以下を実行します。
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  `Groupings`ヘッダーの隣にある`+ Add grouping...`を選択し、グループ化したい列を選択します。

##### **グルーピングに計算を追加する (Add calculations to a grouping)**
列の各値ではなく、グループの各値に対して集計を計算するには、グルーピングに計算を追加します。
1.  テーブルを選択し、エディタパネルで列のリストを探します。
2.  グルーピングについて、`Calculations`ヘッダーの隣にある`+ Add calculation...`を選択し、グループに対して集計したい列を選択します。
    * 例えば、グループ内の各`Host Name`に対する`Unique Users`など、一部の計算はグループレベルでのみ関連性があります。

##### **テーブル内のグループを管理する (Manage groups in a table)**
テーブルにグルーピングを作成した後、以下のことができます。
* グループ列のヘッダーまたは値の隣にある`+`または`-`を選択して、グループ化されたデータを展開または折りたたみます。
* 列メニューを開いて`Remove from grouping`を選択することで、グルーピングから列または計算を削除します。
* グルーピング全体を削除するには、`Group by`の隣にある`More` > `Remove grouping`を選択します。
* 折りたたまれた列を非表示にします。「[Hide and show table components](https://help.sigmacomputing.com/docs/format-and-customize-a-table#hide-and-show-table-components)」を参照してください。

##### **グループ化されたテーブルに合計を表示する (Show totals in a grouped table)**
デフォルトでは、グループ化されたテーブルでは合計は非表示になっています。グループ化されたテーブルで合計を表示または非表示にするには（例えば、グルーピングの小計を表示するなど）、以下を実行します。
1.  グルーピング内の列について、下矢印()を選択して列メニューを開きます。
2.  `<Column Name> totals`を選択します。
3.  表示または非表示にする合計を選択します。
    * 1つのグルーピングレベルを持つテーブルの場合、`Show grand total`を選択します。
    * 1つ以上のグルーピングレベルを持つテーブルの場合、`Show grand total`または`Show subtotal`の一方または両方を選択します。
    > 📘
    > グルーピングの小計を表示するには、上位レベルのグルーピングの最初のグループ化列の列メニューを開きます。
また、グループ化されたテーブルの**すべて**の合計を表示または非表示にすることもできます（例えば、すべてのグルーピングレベルの合計を表示するなど）。すべての合計を表示するには、テーブルセルを右クリックしてコンテキストメニューを開き、`Show all totals`を選択してテーブルのすべてのグルーピングレベルの合計を表示します。いずれかの合計が表示されている場合は、まず`Hide all totals`を選択し、次に`Show all totals`を選択してすべてを表示します。

##### **例：ウェブサイト分析をホスト名でグループ化し、統計を計算する (Example: Group website analytics by host name and calculate statistics)**
例えば、ホスト名でグループ化されたウェブサイト分析を表示するためにテーブルを使用したい場合があります。この例では、ホスト名のグルーピングを作成し、そのグルーピング内に計算列を追加して、総ページビューと総ユニークユーザーを計算します。
> 📘
> この例では、Sigmaサンプルデータベースの`Events`テーブルを使用します。テーブルへのフルパスは`APPLICATIONS.GOOGLE_ANALYTICS.EVENTS`です。

1.  `Events`テーブルをデータソースとしてテーブルを作成します。
    a.  `Add element`バーで、`Data`を選択し、次に`Table`を選択します。
    b.  `Select source`で、Sigmaサンプルデータベースの`APPLICATIONS.GOOGLE_ANALYTICS.EVENTS`テーブルを検索または参照します。
    c.  データソースを選択して、データが入力されたテーブルをワークブックに追加します。!
![4c665843caf925b207ece88ed952cb376e5a14e4dd5171d85559b1839d884d62-group-events-start](https://github.com/user-attachments/assets/396063dc-a75d-4924-802f-2c9c145b0070)

2.  `Groupings`の隣で、`+ Add grouping...`を選択し、`Host Name`を選択します。![76a4104c94711bcde148f8fd4f47f57bc779a1f30a842c3b08e1a65ee3842e68-group-add-column](https://github.com/user-attachments/assets/c970389d-29bd-4878-baee-c48ff8862702)

3.  グルーピング内で、`Calculations`の隣にある`+ Add calculation...`を選択し、`User Pseudo Id`を選択します。
 `Count of User Pseudo Id`として計算列が作成されます。ユニークユーザーのみを見るように列を更新するには、集計を`CountDistinct`に変更します。
    a.  エディタパネルで、計算列名にカーソルを合わせ、下矢印()をクリックして列メニューを開きます。
    b.  `Set aggregate > CountDistinct`を選択します。
        列は`CountDistinct of User Pseudo Id`に更新されます。
    c.  列名をダブルクリックして`Total Unique Users`に名前を変更します。![32c7bac2de9573341acbbd26bbf5a9186c59d5c0c4584456b1dce766fb2dd923-group-events-2-calc](https://github.com/user-attachments/assets/0d4beb43-d2ad-411f-b45b-5cd29b96c16e)

4.  グルーピング内で、`Calculations`の隣にある`+ Add calculation...`を選択し、`Event Name`を選択します。
   `Count of Event Name`として計算列が作成されます。ページビューのみに焦点を当てるように列を修正するには、`CountIf`関数を使用して数式バーに新しい数式を入力します。
    a.  `Count of Event Name`列を選択します。
    b.  数式バーで、数式を`Count([Event Name])`から以下に変更します。
        `CountIf([Event Name] = "page_view")`
    c.  キーボードのenterまたはreturnを押すか、チェックマークをクリックして数式を保存し、列を更新します。
    d.  列名は`CountIf of Calc`に更新されます。
    e.  列名をダブルクリックして`Total Page Views`に名前を変更します。
5.  テーブルで、`Host Name`列の隣にある`-`を選択して、テーブル内のグループ化されていない行を折りたたみ、グループ化されたデータのみを表示します。![a7bb01d11d1e461de50ac4d87f06a879fbe64eb64e14176c864a3632cffdc4d8-group-events-collapse-3](https://github.com/user-attachments/assets/0b002c61-a450-47a7-9306-1317c01ecb3d)

6.  テーブルを読みやすくするために、総ページビューで列をソートできます。`Total Page Views`列について、下矢印()をクリックして列メニューを開き、`Sort descending`()を選択します。<img width="897" height="140" alt="0ad87ade60f6dceeaf0d7157fbfbe22404f6ae00f0fa9817181733aa5bfce3b8-group-events-table-result-4" src="https://github.com/user-attachments/assets/71673a14-f768-4b34-8c42-d4bf46d92702" />

これで、各ホスト名の総ページビューとユニークユーザーが、総ページビューでソートされたテーブルができました。テーブルをフォーマットすることで、折りたたまれた列を非表示にするなどの書式変更ができます。「[Format and customize tables](https://help.sigmacomputing.com/docs/format-and-customize-a-table)」を参照してください。
テーブルを修正し、追加の列でグループ化できます。例えば、各ホスト名のトラフィックソース別のトップセッション開始を知りたい場合は、これらのステップを繰り返して`Traffic Source`列で2番目のグルーピングを追加し、`CountIf([Event Name] = "session_start")`でグルーピング内に計算を作成します。![2e1535ebcf679ed5ba8a760184cc7c46dbeffade67cd6b13426eb2b439136a33-group-events-grouping2](https://github.com/user-attachments/assets/e4462abd-809e-4386-969f-dc67c7059baf)

テーブルの分析をさらに絞り込むには、`Total Sessions Started`列を降順でソートし、次に`Top N filter`を使用して列をフィルタリングし、各ホスト名のトラフィックソース別のトップ10セッション開始のみを表示します。テーブルのフィルタリングに関する詳細は、「[Data element filters](https://help.sigmacomputing.com/docs/data-element-filters)」を参照してください。![22fdee2d6c1da02bee7d6ef8500758b18caa477a8d0ca623208131e18196c068-group-events-grouping-2-sort](https://github.com/user-attachments/assets/6185de45-9bc7-4740-abcf-7abf109a276a)


#### **テーブルにサマリー統計を追加する (Add summary statistics to a table)**

どのテーブルでも、各列のサマリー統計を表示できます。**サマリー**は、テーブルの最高集計レベルで計算される単一値の列集計です。
テーブルにサマリーを追加するには、ドキュメントを編集中またはカスタマイズ中である必要があります。

テーブルのサマリー統計を表示するには、以下を実行します。
1.  キャンバスでテーブルを選択し、`Show summaries`()を選択します。
2.  `+ Add summary...`を選択します。
3.  列オプションを選択します。
    * `New summary`を選択して、カスタム数式でカスタムサマリーを計算します。
    * `Row count`を選択して、総行数をカウントします。
    * 既存の集計列を選択して、その列のサマリーを作成します。サマリーに使用されるデフォルトの[集計](https://help.sigmacomputing.com/docs/aggregate-functions)は列のデータ型に依存しますが、変更できます。

他の列と同様に、サマリー統計を名前で列から参照できます。例えば、`Min([Event Date])`という数式を持つ`Earliest Date`というサマリー統計に対して、そのサマリーを参照する数式で`Days Since Start`という列を計算することができます。
`DateDiff("day", [Earliest Date], [Event Date])`

#### **テーブルの列をソートする (Sort table columns)**

テーブルを列の値でソートできます。1つの列で昇順、1つの列で降順、または1つ以上の列でカスタムソート順でソートできます。
* テーブルを1つの列で昇順にソートするには、右クリックまたは下矢印()をクリックして列メニューを開き、`Sort ascending`()を選択します。
* テーブルを1つの列で降順にソートするには、右クリックまたは下矢印()をクリックして列メニューを開き、`Sort descending`()を選択します。
* テーブルのソート順をカスタマイズするには、「[Customize the sort order of data elements](https://help.sigmacomputing.com/docs/customize-the-sort-order)」を参照してください。

### 4-4-2. 表の書式設定とカスタマイズ (Format and customize a table)

Sigma では、表形式データの表示を効率的かつ効果的にデザインし、フォーマットすることができます。Sigma には、すぐに使える美しさと読みやすさを実現するプリセットの表示スタイルが用意されているほか、スタイルコンポーネントを個別にカスタマイズして、よりパーソナライズされた表デザインを実現することもできます。

テーブル、ピボットテーブル、入力テーブルの書式を設定およびカスタマイズし、ワークブック開発のさまざまなレベルで書式設定を適用できます。
* 管理者は、組織全体のワークブックテーマでデフォルトの表スタイルを定義できます。「[ワークブックテーマの作成と管理](https://help.sigmacomputing.com/docs/workbook-themes)」をご覧ください。
* ワークブック内のすべてのテーブル（ピボットテーブルと入力テーブルを含む）にテーブルスタイルを指定します。「[ワークブック設定の概要](https://help.sigmacomputing.com/docs/workbook-settings-overview)」の「テーブルスタイルの設定」を参照してください。
* 1つの表要素に表スタイルを適用します。このページの「[個々の要素のテーブルスタイルをカスタマイズする](#customize-the-table-style-for-an-individual-element)」をご覧ください。
* 特定の列、合計行、または合計列のデータを書式設定します。このページの「[列と合計データの書式設定](#format-column-and-totals-data)」を参照してください。
* 条件に基づいて列のデータを書式設定します。このページの「[条件付き書式の適用](#apply-conditional-formatting-to-table-columns-and-cells)」を参照してください。

#### **ユーザー要件 (User requirements)**
* **始める前に：** このアクションはエディターパネルを使用します。まだ開いていない場合は、`Explore`または`Edit`モードからエディターパネルを開いてください。「[Workbook modes](https://help.sigmacomputing.com/docs/workbook-modes-overview)」を参照してください。
* `Full explore`または`Create, edit, and publish workbooks`権限が有効になっているアカウント タイプが割り当てられている必要があります。
* ワークブックの所有者であるか、ワークブックを参照または編集できる `Can explore`または`Can edit`の権限が付与されている必要があります。

#### **個々の要素のテーブルスタイルをカスタマイズする (Customize the table style for an individual element)**
個々のテーブル、ピボットテーブル、または入力テーブル要素にカスタムテーブルスタイルを適用します。カスタムテーブルスタイルは、[ワークブックレベルで設定された](https://help.sigmacomputing.com/docs/workbook-settings-overview#set-the-table-style)スタイルよりも優先されます。

1.  ワークブックのカスタマイズを開始するか、ワークブックを開いて編集します。
2.  変更するテーブル、ピボット テーブル、または入力テーブル要素を選択します。
3.  サイド パネルで**書式**を選択し、 **表スタイル**ヘッダーをクリックしてセクションを展開します。
4.  テーブル スタイルのプリセットを選択するか、必要に応じてテーブル スタイルのコンポーネントをカスタマイズします。
    詳細は、「[カスタマイズ可能なテーブルスタイルオプション](#customizable-table-style-options)」を参照してください。

##### **利用可能なテーブルスタイルのプリセット (Available table style presets)**
Sigmaには、ワークブックのすべての表スタイルオプションを自動的に設定する2つのプリセットが含まれています。プリセットは、ワンクリックソリューションとして、またはカスタム表デザインの出発点として使用できます。
* **スプレッドシート (Spreadsheet)**
    スプレッドシートプリセット（デフォルト）は、継続的な分析と共同作業のために設計されています。読みやすさを確保し、ツールヒントや画像などの追加コンテキストを含めるのに最適です。<img width="784" height="354" alt="eb2ccc5-image" src="https://github.com/user-attachments/assets/b4535931-89c2-42d7-b927-05e6e5e47195" />

* **プレゼンテーション (Presentation)**
    プレゼンテーションプリセットは、表形式での表示向けに設計されています。企業ブランディングに合わせ、ワークブックに視覚的な魅力を加えるのに最適です。
<img width="784" height="354" alt="7db37b0-image" src="https://github.com/user-attachments/assets/6300ad22-a46e-4193-9718-321b44c6a9c6" />

##### **カスタマイズ可能なテーブルスタイルオプション (Customizable table style options)**
テーブル、ピボット テーブル、入力テーブル要素を使用して、ブランド化と美的要件を満たすように次のテーブル スタイル コンポーネントをカスタマイズできます。
* セル間隔 (Cell spacing)
* グリッド線 (Grid lines)
* バンディング (Banding)
* ヘッダー形式 (Header format)
* サブヘッダーの形式 (Subheader format)
* セル形式 (Cell format)

* **セル間隔 (Cell spacing)**
    セル間隔設定では、表のセル内のテキストの周囲のパディングを調整できます。「極小(Extra small)」、「小(Small)」、「中(Medium)」、「大(Large)」の4つのオプションから選択できます。<img width="376" height="220" alt="473d8a8-image" src="https://github.com/user-attachments/assets/3715b8ee-1899-4db5-8868-9551f477ec6a" />
<img width="376" height="219" alt="5fcc740-image" src="https://github.com/user-attachments/assets/f17a88f0-57e0-4501-bbf3-08bc9d94718f" />
<img width="376" height="219" alt="a7c8be7-image" src="https://github.com/user-attachments/assets/c6017d83-f189-4fde-bc3f-38880a5a5d53" />
<img width="376" height="219" alt="3a0ab4b-image" src="https://github.com/user-attachments/assets/377b78e6-8bf7-403e-a2a2-7f6af132b801" />

* **グリッド線 (Grid lines)**
    グリッド線の設定では、セルの境界線の表示を管理できます。「グリッドなし(No grid)」、「垂直グリッド(Vertical grid)」、「水平グリッド(Horizontal grid)」、「すべてグリッド(All grid)」の4つのオプションから選択できます。
<img width="376" height="220" alt="769cfab-image" src="https://github.com/user-attachments/assets/b673626e-d0a0-4c64-923e-9b409948e4d0" />
<img width="376" height="220" alt="9840201-image" src="https://github.com/user-attachments/assets/71c2de69-4064-4339-8aaf-7a2c9451f0ce" />
<img width="376" height="218" alt="a63ea2f-image" src="https://github.com/user-attachments/assets/ac84a52e-5af3-4d6b-bae2-2a7d1d0d5280" />
<img width="376" height="219" alt="af58fb0-image" src="https://github.com/user-attachments/assets/6243517a-44d1-4045-b975-c2f12fcbdc6a" />

* **バンディング (Banding)**
    「バンドを表示(Show banding)」設定では、データ行の背景色を交互に変更できます。バンド表示の行の背景色は、デフォルトのヘッダーの背景色と一致します。
<img width="376" height="220" alt="62da251-image" src="https://github.com/user-attachments/assets/565be85b-68ce-4f92-9431-42bd8e4f9c50" />
<img width="376" height="220" alt="ad2addf-image" src="https://github.com/user-attachments/assets/675a5262-59e6-4ef7-a424-6a9ce60e49d2" />

* **ヘッダー形式 (Header format)**
    「ヘッダー」タブには、表のヘッダーの書式設定に必要な設定とツールが含まれています。フォントの種類、サイズ、太さ、色、テキストの折り返し、テキストの配置、背景色、区切り線の色などをカスタマイズできます。
<img width="648" height="313" alt="bc13511-image" src="https://github.com/user-attachments/assets/73609c3c-461d-4c06-ad7d-fe55fb32faa1" />

* **サブヘッダー形式（ピボットテーブルのみ）(Subheader format (pivot tables only))**
    「サブヘッダー」タブには、サブヘッダーの行と列の書式設定を行うための設定とツールが含まれています。行ヘッダーと列ヘッダーの両方について、フォントの種類、サイズ、太さ、色、テキストの折り返し、テキストの配置、背景色の設定をカスタマイズできます。
<img width="648" height="313" alt="9231f92-image" src="https://github.com/user-attachments/assets/a6de17d0-6f62-4da2-8883-da73cac1dbce" />

* **セル形式 (Cell format)**
    「セル」タブには、データセルの書式設定に必要な設定とツールが含まれています。フォントの種類、サイズ、太さ、色、テキストの折り返し、テキストの配置、背景色の設定をカスタマイズできます。
    > 📘
    > ピボットテーブルでは、セルスタイルはデフォルトで値セルと合計セルの両方に適用されます。ピボットテーブルの合計セルに異なるスタイルを適用するには、 「[列と合計データの書式設定](#format-column-and-totals-data)」および「[ピボットテーブルの合計の書式設定](https://help.sigmacomputing.com/docs/format-pivot-table-totals)」をご覧ください。
<img width="648" height="313" alt="2eee376-image" src="https://github.com/user-attachments/assets/29f15860-33e2-4b28-a8d4-dd6d25086985" />

#### **表内の列の位置を書式設定する (Format column location in a table)**
テーブル内の列の表示と操作を管理するには、テーブルまたはピボット テーブル内の列の位置を書式設定できます。
列を右クリックするか、下矢印 () を選択して列をカスタマイズします。
* 「**列まで固定 (Freeze up to column)**」を選択すると、選択した列とその左側にあるすべての列の位置が固定されます。右にスクロールしても、固定された列は表示されたままです。固定された列の位置を解除するには、「**列の固定を解除 (Unfreeze columns)**」を選択します。
* 「**列を非表示 (Hide column)**」を選択すると、表の表示時に列が非表示になります。非表示の列は数式で参照できます。非表示の列を含む表から作成された子要素には非表示の列は含まれませんが、列を追加することは可能です。

ピボット テーブルでは、合計列を含む値列の固定がサポートされていますが、ピボット行列やピボット列として設定された列の固定はサポートされていません。
> 📘
> グループ化されたテーブル内の合計行の位置を変更することはできません。

#### **テーブルコンポーネントの表示と非表示 (Hide and show table components)**
テーブルにさまざまなテーブル コンポーネントを表示するかどうかを管理するには、テーブル コンポーネントをフォーマットします。
1.  ワークブックのカスタマイズを開始するか、ワークブックを開いて編集します。
2.  変更するテーブルまたは入力テーブル要素を選択します。
3.  サイドパネルで、**フォーマット**を選択します。
4.  **テーブル コンポーネント**ヘッダーをクリックしてセクションを展開し、設定を調整します。

| オプション | 詳細 |
| :--- | :--- |
| **表を表示 (Show table)** | 要素内の表の列と行を表示するかどうか。オンにすると、サマリーバーとタイトル（表示されている場合）のみが表示されます。|
| **折りたたまれた列を表示 (Show collapsed columns)** | 表の場合、グループ化が折りたたまれているときに、グループ化されていない列を表示するかどうかを指定します。グループ化されていない表は、このオプションの影響を受けません。複数のグループ化がある表については、「[表内のグループの管理](https://help.sigmacomputing.com/docs/create-and-manage-tables#manage-groups-in-a-table)」を参照してください。|
| **概要バーを表示 (Show summary bar)** | サマリー バーをテーブルまたは入力テーブルに表示するかどうか。|

#### **列と合計データの書式設定 (Format column and totals data)**
列は、その[データ型](https://help.sigmacomputing.com/docs/supported-data-types-and-formats)に応じて自動的に書式設定されます。書式を変更することで、列のデータを別の形式で表示できます。
グループ化された表またはピボットテーブルに合計が含まれている場合、ツールバーを使用して、合計行または合計列を表の列とは別に書式設定できます。合計行と合計列の両方に書式設定を適用した場合、行の書式設定が優先されます。ピボットテーブルの合計の書式設定に関するその他のオプションについては、「[ピボットテーブルの合計の書式設定](https://help.sigmacomputing.com/docs/format-pivot-table-totals)」をご覧ください。

* **数値の書式を変更する (Change number formatting)**
    列または合計セルを選択し、ツールバーのオプションを選択して数値の書式を変更します。
    * 通貨としてフォーマット
    * パーセント形式で表示
    * 小数点以下の桁数を減らしたり増やしたりします。
    * 数値データを別の形式で表示します。詳細については、「[サポートされているデータ型と形式](https://help.sigmacomputing.com/docs/supported-data-types-and-formats)」をご覧ください。

* **列データの外観を変更する (Change column data appearance)**
    書式設定ツールバーを使用して、特定の列のデータの外観を変更できます。表内のすべてのデータの外観を変更するには、「[セルの書式](#cell-format)」を設定します。これらの書式設定オプションは列ヘッダーには影響しません。
    列または合計セルを選択した後、ツールバーのオプションを選択してデータの外観を変更します。
    * データの配置を選択します。
    * テキストの色を選択します。
    * 背景色を選択します。列または合計セルを選択し、ツールバーの「背景色」をクリックします。
    * ()列内のテキストを折り返します。
    > 📘
    > [条件付き書式](https://help.sigmacomputing.com/docs/conditional-formatting)は、ツールバーから適用された書式よりも優先されます。

#### **表の列とセルに条件付き書式を適用する (Apply conditional formatting to table columns and cells)**
ルールまたは条件に基づいて表の列とセルを書式設定するには、条件付き書式を適用します。
> 📘
> 条件付き書式は、[ツールバーの列書式設定オプション](https://help.sigmacomputing.com/docs/format-and-customize-a-table#change-column-data-appearance)よりも優先されます。

条件付き書式を使用すると、書式設定ルールに基づいて、1つまたは複数の列に特定の書式を適用できます。デフォルトの書式設定ルールを選択するか、[論理関数](https://help.sigmacomputing.com/docs/logical-functions)や[テキスト関数](https://help.sigmacomputing.com/docs/text-functions)などのカスタム数式を指定します。
* 斜体、太字、下線、テキストの色などのテキスト書式を適用します。
* 背景色を設定します。
* 数値または日付の値をフォーマットします。
* 背景色またはテキスト色にカラースケールを適用します。
* データ値の上にデータ バーを表示するか、データ値を非表示にしてデータ バーのみを表示します。

表全体に書式を適用するには、「[カスタマイズ可能な表スタイル オプション](#customizable-table-style-options)」を参照してください。
1.  クリックしてテーブルを選択します。
2.  列の列メニュー、またはサイド パネルの**書式**セクションから、 **条件付き書式**を選択します。
3.  列メニューから条件付き書式を開いた場合、「条件付き書式」パネルにはその列のデフォルトのルールが表示されます。それ以外の場合は、「+ ルールを追加」をクリックします。
4.  （オプション）「**適用先**」で、条件付き書式を適用する列を選択します。「すべての列」を選択することもできます。
5.  書式設定には、**単色**、**カラースケール**、**データ バー**のオプションから選択します。
6.  **書式設定ルール**では、条件付き書式ルールを定義します。あらかじめ用意されたルールを選択するか、カスタム数式を定義します。
7.  ルールを作成し、書式を定義すると、該当する列とセルに書式が適用されます。
8.  (オプション) [ + ルールの追加]をクリックして、条件付き書式ルールをさらに追加します。
    > 💡
    > 表に合計が含まれている場合は、小計の行と列、または総計の行と列にのみ条件付き書式を適用できます。
### 4-4-3. 列にハイパーリンクと画像を追加する (Add hyperlinks and images to columns)

テーブルまたはピボットテーブルにURLが含まれている場合、それらのURLを使用して、別のテーブル列のデータにハイパーリンクを設定したり、リンクされた画像を表示したりできます。列メニューを使用して、任意のテーブルまたはピボットテーブルの列にハイパーリンクを追加できます。

#### **要件 (Requirements)**

個々のワークブックに対する`Can Explore`または`Can Edit`の[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。

#### **列にハイパーリンクを追加する (Add a hyperlink to a column)**

列内のデータに、別の列にあるURLを参照するか、数式でURLを構築してハイパーリンクを設定できます。データにハイパーリンクを設定するには、ワークブックが`Explore`または`Edit`モードである必要があります。

##### **数式でハイパーリンクを追加する (Add a hyperlink with a formula)**

一つ以上の列のデータからURLまたはリンクを構築し、そのテキストをクリック可能なハイパーリンクに変換できます。
例えば、店舗IDに基づいて店舗の場所のURLを構築し、その構築したURLを`Store Name`列のハイパーリンクとして使用します。

1.  テーブルまたはピボットテーブル要素を選択します。
2.  列にカーソルを合わせ、キャレット()をクリックして列メニューを開きます。
3.  列メニューで、`Transform` > `Set link...`を選択します。
4.  `Set Link for Column`モーダルが開きます。
5.  `Link source`で、`Custom formula`を選択します。
6.  `Create URL with formula`で、`Concat`関数を使用して数式を定義します。
    * 例えば、文字列と列でターゲットURLを構成します。
      `Concat("https://www.example.com/?location-id=", [Store Id])`
7.  `Enter`または`Return`を押すか、チェックマークをクリックして数式を適用します。`URL Column`で出力をプレビューします。
8.  `Set Link`をクリックします。

##### **既存のURL列からハイパーリンクを追加する (Add a hyperlink from an existing URL column)**

テーブルまたはピボットテーブルにURLを含む列がある場合、その列をソースとして使用して、別の列の値にハイパーリンクを追加できます。URL列には、自動的にハイパーリンクされるURLのテキスト、またはURLを構築する数式を含めることができます。

例えば、`Page Title`列のデータに`Page Link`列のURLでハイパーリンクを設定するには、以下を実行します。
1.  列にカーソルを合わせ、キャレット()をクリックして列メニューを開きます。例えば、`Page Title`列の列メニューを開きます。
2.  列メニューで、`Transform` > `Set link...`を選択します。
3.  `Set Link for Column`モーダルが開きます。
4.  `Link source`で、`Another column`を選択します。
5.  `Select column`で、URLを含む列を選択します。例えば、`Page Link`列を選択します。
6.  `URL Column`で出力をプレビューします。
7.  `Set Link`をクリックします。

#### **列からハイパーリンクを削除する (Remove a hyperlink from a column)**

列からハイパーリンクを削除（列のリンクを解除）するには、以下を実行します。
1.  ハイパーリンクされたデータを持つ列について、キャレット()をクリックして列メニューを開きます。
2.  列メニューで、`Transform` > `Set link...`を選択します。
3.  `Remove`をクリックしてリンクを削除します。

#### **URLを含む列を作成する (Create a column with URLs)**

列に完全なURLを表示する、URLを含む列を作成するには、以下を実行します。
> 📘
> クリック可能なハイパーリンク付きのテキストを表示するには、「[Add a hyperlink to a column](#add-a-hyperlink-to-a-column)」を参照してください。

1.  URLを追加する列を選択または作成します。
2.  数式バーと`Concat`関数を使用して、URLを構築する数式を記述します。
    * 例えば：
      `Concat("https://www.example.com/?location-id=", [Store Id])`
    * または、画像URLを作成する例として：
      `Concat("https://example.com/image/", [Product Id])`
3.  キーボードの`Enter`または`Return`を押すか、数式バーの隣にあるチェックマークをクリックして、数式を保存します。

画像へのURLを構築した場合、テーブルに画像を表示するように設定できます。「[Display linked images in a table column](#display-linked-images-in-a-table-or-pivot-table)」を参照してください。

#### **テーブルまたはピボットテーブルにリンクされた画像を表示する (Display linked images in a table or pivot table)**

テーブルまたはピボットテーブルに、小売製品のサムネイル画像など、画像へのリンクを含む列がある場合、その列を変換して、画像リンクを画像として表示できます。ピボットテーブルの行、列、または値の列に画像を表示できます。

* **前提条件:**
    * データ内に画像へのリンクを持つ列が必要です。
    * このアクションは編集モードでのみ利用可能です。編集を開始するには、ページの右上隅にある`Edit`をクリックします。

データ列のリンクから画像を表示するには：
1.  列にカーソルを合わせ、キャレット()をクリックして列メニューを開きます。
2.  `Transform > Set image...`を選択します。<img width="375" height="709" alt="ca08e01-image" src="https://github.com/user-attachments/assets/6c7bf17c-84c5-4a66-bb3a-dae5f645de3f" />

3.  `Set image options`モーダルで、`Display as image`トグルをオンにします。
4.  画像のサイジング、高さ、幅、および画像のアスペクト比を維持するかどうかを指定します。
5.  `Save`を選択します。
6.  画像がテーブルセルに表示されます。

### 4-4-4. JSONまたはバリアントデータから列を抽出する (Extract columns from JSON or variant data)

JSONデータ型は、本質的に階層的なデータを保存します。[列メニューを使用する](https://help.sigmacomputing.com/docs/extract-columns-from-json-or-variant-data#extract-json-data-from-a-column)か、[ドット記法を使用する数式を記述する](https://help.sigmacomputing.com/docs/extract-columns-from-json-or-variant-data#use-dot-notation-to-extract-values-from-json-columns)ことにより、JSONを含むテーブル列から完全な構造化および半構造化データを抽出できます。

#### **要件 (Requirements)**

JSONまたはバリアントデータから列を抽出する機能には、以下が必要です。
* `Basic explore`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがワークブックの所有者であるか、`Can explore`または`Can edit`の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **列からJSONデータを抽出する (Extract JSON data from a column)**

任意のデータ要素で、一つの列からJSONデータを別々の列に抽出できます。JSONまたはVariantのデータ型を持つ列には、列メニューに`Extract columns...`オプションがあります。データが半構造化されており、`Extract columns`オプションが表示されない場合は、[データ型を変換](https://help.sigmacomputing.com/docs/extract-columns-from-json-or-variant-data#convert-the-data-type-of-a-column)できます。列の抽出は上流の要素で行うのがベストプラクティスです。

> 🚧
> 抽出される列のリストは、テーブルの最初の1,000行から取得されます。それ以降の行にあるキーと値のペアは抽出されません。

一つの列からJSONデータを抽出し、JSONデータのキーに一致する別々の列を作成するには：
1.  ワークブック内の列に移動します。この例では、`EXAMPLES.PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA`サンプルデータの`Cust Json`列を使用します。
2.  列について、キャレット()をクリックして列メニューを開きます。
3.  `Extract columns`を選択します。
    `Extract Fields`モーダルが開きます。
4.  モーダルで、独自の列に抽出したいJSONキーを選択します。選択した各JSONキーに対して一つの列が作成されます。
5.  `Confirm`をクリックして、選択したキーと値のペアを抽出し、対応する列を作成します。
<img width="711" height="760" alt="1740b22dd46ddd5706ead9883a0a60ff5be62b63c333c703d7748ab7f6897ef2-extractjson_4" src="https://github.com/user-attachments/assets/7882238e-0d46-49c6-88d1-5c6eb74254d7" />
その後、新しい列をデータ探索や分析で使用できます。

#### **列のデータ型を変換する (Convert the data type of a column)**

列からJSONまたは半構造化データを抽出したいが、列メニューに`Extract columns`オプションが表示されない場合は、列のデータ型をJSONまたはVariantに変換します。
* `Json`または`Variant`の型関数を使用して列の数式を修正します。
* 列メニューを開き、`Transform` > `Convert to JSON`を選択します。

#### **ドット記法を使用してJSON列から値を抽出する (Use dot notation to extract values from JSON columns)**

ドット記法を使用した数式を記述することで、JSON列内のJSON配列やオブジェクトから値を抽出することもできます。


### 4-4-5. ピボットテーブル (Pivot tables)

#### 4-4-5-1. ピボットテーブルを操作する (Working with pivot tables)

Sigmaでは、ピボットテーブルを作成して、特定のやり方でデータをグループ化し、要約することができます。ピボットテーブルを使用して、データを2つの次元で表示し、グループに基づいてデータを自動的に要約し、様々な階層でデータを表示します。

テーブル内の列をグループ化して、特定のグループのデータを集計するなど、ピボットテーブルの一部の機能に近いことを行うこともできます。「[Create and manage tables](https://help.sigmacomputing.com/docs/create-and-manage-tables)」を参照してください。

##### **要件 (Requirements)**
データ要素を作成または編集するには、個々のワークブックに対する`Can edit`アクセス権が必要です。
一部の探索的アクションは、`Can explore`アクセスでもサポートされています。
詳細は、「[Folder and document permissions](https://help.sigmacomputing.com/docs/folder-and-document-permissions)」を参照してください。

##### **ピボットテーブルを作成する (Create a pivot table)**
既存のデータ要素から、または`Add element`バーで`Data` > `Pivot table`を選択してピボットテーブルを作成できます。詳細は、「[Create a data element](https://help.sigmacomputing.com/docs/create-a-data-element)」を参照してください。

ピボット行および/またはピボット列として使用するデータソース列を定義するまで、ピボットテーブルはデータを表示しません。エディタパネルの`Properties`タブで、以下のプロパティを構成します。
* **Pivot rows (ピボット行):** テーブルから一つ以上の列を選択し、ピボットテーブルの行として表示します。例えば、製品タイプごとの総コストを要約するには、製品タイプ列をピボット行として追加します。<img width="1298" height="531" alt="6fd7287721b59c1407cc826eb2cb3c038ccc161b32f688f9624be2351f28e3d1-pivot-one-row" src="https://github.com/user-attachments/assets/24a0177a-2b38-4769-ad5b-21259ef3e82a" />

* **Pivot columns (ピボット列):** [任意] 一つ以上のピボット行を定義した場合。各行の値を分割するために一つ以上の列を選択します。例えば、各店舗地域ごとの各製品タイプの総コストを要約するには、店舗地域列をピボット列として追加します。<img width="1298" height="531" alt="9394cca08b38349c8d7e2fb4b5035b0ab740f5015a1ab704623c196d9e49bac2-pivot-row-column-foreal" src="https://github.com/user-attachments/assets/60735bd5-bfbe-4d85-9701-a2f7f0f2a341" />

* **Values (値):** 各ピボット行と列の値を表示するために一つ以上の列を選択します。`Values`に追加された列はデフォルトで集計され、使用される集計のタイプは元の列のデータ型に依存します。例えば、コスト列を値として追加し、デフォルトの集計である`Sum`のままにするか、丸めて調整します。「[Change the aggregation of values](#change-the-aggregation-of-values)」を参照してください。<img width="1297" height="540" alt="05af48a26bb503feba86d2186a46024c2446c4144f64f0a3cbf3202bfd27b18e-pivot-row-column-value" src="https://github.com/user-attachments/assets/f6d7b161-dce3-4b13-ba39-8439a7c08318" />

##### **ピボットテーブルの書式設定とカスタマイズオプション (Pivot table formatting and customization options)**
多くの方法でピボットテーブルの書式設定と表示をカスタマイズできます。ピボットテーブルで合計を表示または非表示にするには、「[Pivot table totals and subtotals](https://help.sigmacomputing.com/docs/pivot-table-totals-and-subtotals)」を参照してください。
* **始める前に:** このタスクは要素の編集を必要とします。ワークブックをカスタマイズまたは編集することで要素を編集できます。

1.  エディタパネルで、`Format`タブを選択します。
2.  書式カテゴリをクリックして、その設定を表示・編集します。

ピボットテーブルで利用可能な書式カテゴリは以下の通りです。
* **Element Style:** 「[Customize element background and styles](https://help.sigmacomputing.com/docs/customize-element-background-and-styles-beta)」を参照してください。
* **Title:** 「[Customize element title](https://help.sigmacomputing.com/docs/customize-element-title)」を参照してください。
* **Table style:** 「[Format and customize a table](https://help.sigmacomputing.com/docs/format-and-customize-a-table)」を参照してください。
* **Totals:** 「[Format pivot table totals](https://help.sigmacomputing.com/docs/format-pivot-table-totals)」を参照してください。
* **Format:** 「[Specify empty cell display value](#empty-cell-display-value)」および「[Repeat row labels](#repeat-row-labels)」を参照してください。

また、ピボットテーブルの列を書式設定することもできます。「[Format pivot table columns](#format-pivot-table-columns)」を参照してください。

##### **空のセルの表示値を指定する (Empty cell display value)**
ピボットテーブルに空の値がある場合、空のセルを埋める値を指定できます。
1.  ワークブックをカスタマイズまたは編集用に開きます。
2.  ピボットテーブル要素を選択し、エディタパネルで`Format`タブを選択します。
3.  `Format`をクリックします。
4.  `Empty cell display value`に、値を入力します。
| 選択したオプション | 例 |
| :--- | :--- |
| Default | (<img width="1299" height="531" alt="50db5684821a699ca21f3784ac74a71c493c65f6f58d1b2ba231b96b42feb71f-pivot-empty-cell-empty" src="https://github.com/user-attachments/assets/15ff1c64-d244-4b98-9537-d8ecfabadc49" />
) |
| Empty Cell display value | (<img width="1299" height="533" alt="73ba99717cf8011a6ca863d99ee3667fb442cffb155fb97a697eda9404f94454-pivot-empty-cell-full" src="https://github.com/user-attachments/assets/d559bf69-92c0-4b1e-bb37-2c6ac5ae30cc" />
) |


##### **行ラベルを繰り返す (Repeat row labels)**
複数のピボット行が定義されており、ピボット行のグルーピングを別々の列として表示することを選択した場合、行ラベルを繰り返すことができます。
1.  ワークブックをカスタマイズまたは編集用に開きます。
2.  ピボットテーブル要素を選択し、エディタパネルで`Format`タブを選択します。
3.  `Format`をクリックします。
4.  `Repeat row labels`で、チェックボックスを選択します。

| 選択したオプション | 例 |
| :--- | :--- |
| Default | (<img width="1015" height="497" alt="e959ccd750408812bec170e10de3b6392fcb8b97f95ad0ceae132d110072809e-pivot-repeat-norepeat" src="https://github.com/user-attachments/assets/0ef4515f-9b12-4f65-af7d-ab3123b2cb2a" />
) |
| Repeat row labels | (<img width="1019" height="496" alt="6e415503b512c78f338619ad7950f21c783b228ed7ab596e72e73d80a57f809f-pivot-repeat-headers" src="https://github.com/user-attachments/assets/002b03d6-f059-44e7-b60e-72c64a0f1827" />
) |

##### **ピボットテーブルの列を書式設定する (Format pivot table columns)**
以下の列書式設定オプションが利用可能です。
* Alignment (配置)
* Font color (フォントの色)
* Background color (背景色)
* Conditional formatting (条件付き書式)

* **基本的な視覚的列書式設定を適用する**
    列の値の配置、フォントの色、または背景色を変更するには：
    1.  書式設定したい列またはセルを選択します。
    2.  背景色を設定するには、数式バーの`Background color`を選択します。
    3.  フォントの色を設定するには、数式バーの`Text color`を選択します。
    4.  データの配置を設定するには、数式バーの`Alignment`を選択します。

* **条件付き書式を適用する**
    ピボットテーブルの列、行、値に条件付き書式を適用できます。条件付き書式を使用して、値ごとに異なる背景色を表示したり、背景またはフォントのスケールでデータの不一致をハイライトしたり、データバーを表示して外れ値を迅速に視覚化したりします。
    > 📘
    > 条件付き書式は、ツールバーの列書式設定オプションよりも優先されます。
    1.  ワークブックをカスタマイズまたは編集用に開きます。
    2.  ピボットテーブル要素を選択し、エディタパネルで`Format`タブを選択します。
    3.  `Conditional formatting`をクリックします。
    4.  `+ Add rule`をクリックします。
    5.  ルールをカスタマイズします。
        * 書式を適用する列を選択します。
        * 単色、カラースケール、またはセルにデータバーを追加するかを選択します。
        * 書式を値、小計、または総計に適用するためのチェックボックスを選択します。
<img width="1285" height="603" alt="97ba76222412421ae945ba2abe556394ab67000e516d58d9838f3d14f743032b-pivot-condi-format" src="https://github.com/user-attachments/assets/a47e4d9b-cfe4-4861-9ad5-cff9c9975039" />

##### **ピボットテーブルでデータ表示を変更する (Change data presentation in a pivot table)**
ピボットテーブルのほとんどの複雑なデータ変換はフラット化されたソーステーブルで行うべきですが、いくつかの方法でピボットテーブルのデータ表示を操作できます。
* [値の集計を変更する](#change-the-aggregation-of-values)
* [ピボットテーブルに計算列を追加する](#add-a-calculated-column-to-a-pivot-table)
* [ピボットの列と行を交換する](#swap-pivot-columns-and-rows)
* [複数のピボット行を別々の列として表示する](#display-multiple-pivot-rows-as-separate-columns)
* [列をソートする](https://help.sigmacomputing.com/docs/customize-the-sort-order)
> 📘
> これらのタスクは要素の編集を必要とします。ワークブックをカスタマイズまたは編集することで要素を編集できます。

* **値の集計を変更する (Change the aggregation of values)**
    データ列をピボットテーブルの`Values`フィールドに追加すると、値はデータ型に応じて自動的に[集計](https://help.sigmacomputing.com/docs/aggregate-functions)されます。数値列は`Sum`で集計され、テキストと日付の列は`Count`で集計されます。
    列の集計を変更するには：
    1.  エディタパネルで、列にカーソルを合わせ、下矢印()をクリックします。
    2.  列メニューが開きます。
    3.  `Set aggregate`サブメニューから、新しい集計を選択します。例えば、`Sum`, `Avg`, `Median`, `Percentile`, `Min`, `Max`, `First`, `Last`, `Count`, `CountDistinct`、または合計に対するパーセンテージなどのより高度な計算を選択します。

* **ピボットテーブルに計算列を追加する (Add a calculated column to a pivot table)**
    合計に対するパーセンテージや期間比較分析など、ピボット全体で繰り返される計算を実行するために、ピボットテーブルに計算列を追加します。
    1.  ピボットテーブル要素を選択します。
    2.  `Values`セクションで、`+` > `Add new column`を選択します。
        `Calc`というタイトルの新しい列が表示され、フォーカスが数式バーに移動します。
    3.  計算列の数式を入力し、キーボードのEnterを押すか、チェックマークを選択して保存します。列は数式の後に自動的に名前が変更されます。
    計算列でピボットテーブルの合計を使用するガイダンスについては、「[Pivot table totals and subtotals](https://help.sigmacomputing.com/docs/pivot-table-totals-and-subtotals)」を参照してください。<img width="1293" height="434" alt="ab4cdda894a8c51f42486098735c1276156aa6cf1764279b4f996b296d471fd6-pivot-calc-column" src="https://github.com/user-attachments/assets/e8a26c65-f071-4366-87bc-05c108358bc0" />

* **ピボットの列と行を交換する (Swap pivot columns and rows)**
    ピボットテーブルのレイアウトを変更し、行と列を交換できます。
    1.  ピボットテーブル要素を選択します。
    2.  エディタパネルで、`Pivot rows`ヘッダーの隣にある`Swap rows with columns`をクリックします。<img width="1364" height="371" alt="3ca38ccd9f31250cf851bef8ca993d35e9996cf60658d888a86c43b4f02b760f-pivot-swap-rows-start" src="https://github.com/user-attachments/assets/8e4c38da-51b9-4dcb-8710-5f2b672c35dc" />

  ピボットテーブルの行と列が交換されます。
<img width="1362" height="370" alt="3c68b2270e8141950bcb90c38156cc8f06022eb37687491ead106abee355b418-pivot-swap-rows-end" src="https://github.com/user-attachments/assets/65d172d2-edf3-475a-b0d7-40e792cd1613" />

* **複数のピボット行を別々の列として表示する (Display multiple pivot rows as separate columns)**
    複数のピボット行がある場合、データを1つの列に結合して表示するか、別々の列として表示するかを選択できます。
    2番目のデータ列をピボット行として追加した後、`Display as separate columns`を選択します。表示を元に戻すには、`Display as a single column`を選択します。

| 選択したオプション | 例 |
| :--- | :--- |
| Display as a single column | (<img width="1363" height="544" alt="28730a10b906e444ccb4d2e1dd893fd4178ebc87aba1def10b5061c002b813c6-pivot-display-single-column" src="https://github.com/user-attachments/assets/942092f8-7d63-4858-8752-548e8244418b" />
) |
| Display as separate columns | (<img width="1362" height="540" alt="3c58634d4cff505bb4be5d9b5abb0dbd327308da1597607f9a202dcf4ebf876d-pivot-display-separate-column" src="https://github.com/user-attachments/assets/12ccb45e-e00b-4c2e-8999-57dc62ebd7a3" />
) |

* **グループ化された行と列を折りたたむ (Collapse grouped rows and columns)**
    ピボットテーブルに`Pivot rows`または`Pivot columns`として少なくとも2つのデータ列が追加されている場合、行と列を展開および折りたたむことができます。そのためには、ピボットテーブルの行、列、またはセルヘッダーの値の隣にある`+`または`-`をクリックします。

* **ピボットテーブルで値の階層を定義する (Define values hierarchy in a pivot table)**
    ピボットテーブルに複数の値がある場合、表示したいデータの要約を反映するように、データ列、値、および行の階層とグルーピングを定義できます。
    ピボットテーブルの値の階層を構造化するには：
    1.  ピボットテーブル要素を選択します。
    2.  `Values`として少なくとも2つの列を追加します。<img width="1272" height="532" alt="2d9a9ce-pivot-values-default" src="https://github.com/user-attachments/assets/7da6a498-331e-48b4-bfb7-8d348836b6c8" />

    3.  `Pivot columns`の下に`Values`というラベルの付いたボックスが表示されます。<img width="1103" height="356" alt="image" src="https://github.com/user-attachments/assets/a7544a77-7c4e-4d78-833c-467997973f65" />

    4.  デフォルトの階層を変更するには、`Values`ボックスを`Pivot columns`の下の別の位置または`Pivot rows`にドラッグ＆ドロップします。
        データの表示は、値の場所に基づいて変化します。

| 値の場所 | 例 |
| :--- | :--- |
| Default, below pivot columns. | (<img width="1364" height="430" alt="53d50c851c2bdab1452c1ebb5f9c43c0b9d93da752ae7045e944f4083a4b90b8-pivot-values-defalt" src="https://github.com/user-attachments/assets/9d0cfe8c-849a-4a73-8a60-b6c4d7772ab7" />
) |
| Above pivot columns. | (<img width="1362" height="432" alt="b7852d55a05a3fd65debac5362915a562a3c79bd2390492428d751ee0c3bc848-pivot-values-columns-top" src="https://github.com/user-attachments/assets/cbcc6a1b-8549-4ab0-a73e-99e511974da5" />
) |
| Below pivot rows. | (<img width="1363" height="434" alt="eb65999386026c99f1d62a148c2477753268a5b04c0d335978ed4f74edffcd8e-pivot-values-rows-bottom" src="https://github.com/user-attachments/assets/49f203f2-b7a1-43e3-878c-ce12debf6916" />
) |
| Above pivot rows. | (<img width="1365" height="433" alt="3e3ec295014bb68502a2699aed2984fa31d98ade839120152bd3648126c2d4af-pivot-values-rows-top" src="https://github.com/user-attachments/assets/8363348c-35f7-421e-a7b2-e0be9a96a0b8" />
) |

* **ピボットテーブルを最大化してフラット化されたテーブルを表示する (Maximize a pivot table to view the flattened table)**
    ワークブックを表示、カスタマイズ、または編集中、すべての[データ要素](https://help.sigmacomputing.com/docs/create-a-data-element)はデフォルトで最小化され、キャンバスに複数の要素を表示します。任意のデータ要素を最大化して、その詳細に焦点を当て、基盤となるデータを探索できます。
    要素を選択して`Maximize element`を選択するか、キーボードのスペースバーを押すと、基盤となるデータが表示されます。
    ピボットテーブルを最大化すると、ワークブックページの全幅に拡大され、基盤となるフラット化されたデータテーブルが表示されます。このビューを使用して、ピボットテーブルのグルーピングレベルを探索できます。要素と基盤となるデータは本質的にリンクしているため、一方に加えられた変更は自動的にもう一方に反映されます。
    > 📘
    > ドキュメントをカスタマイズまたは編集中にのみ、データ要素の基盤となるデータを変更できます。
    詳細は、「[View underlying data](https://help.sigmacomputing.com/docs/view-underlying-data)」を参照してください。

#### 4-4-5-2. ピボットテーブルの合計と小計 (Pivot table totals and subtotals)

グループ化されたテーブルとピボットテーブルは、合計と小計を計算します。ピボットテーブルに値の合計やカウントなどの集計値が含まれている場合、合計はデフォルトで表示されます。

グループ化されたテーブルまたはピボットテーブルで、合計と小計を非表示にしたり、管理したり、カスタマイズしたり、追加の計算を実行したりできます。
* 合計を非表示にするには、「[ピボットテーブルで合計を表示・非表示にする](#show-and-hide-totals-in-a-pivot-table)」または「[グループ化されたテーブルで合計を表示する](https://help.sigmacomputing.com/docs/create-and-manage-tables#show-totals-in-a-grouped-table)」を参照してください。
* 合計の計算に使用される数式をカスタマイズするには、「[合計と小計をカスタマイズする](#customize-totals-and-subtotals)」を参照してください。
* 合計をハイライトしたり、フォントの色を変更するなど、合計をフォーマットするには、「[ピボットテーブルの合計をフォーマットする](https://help.sigmacomputing.com/docs/format-pivot-table-totals)」を参照してください。

テーブルの詳細については、「[テーブルの作成と管理](https://help.sigmacomputing.com/docs/create-and-manage-tables)」を参照してください。
ピボットテーブルの詳細については、「[ピボットテーブルを操作する](https://help.sigmacomputing.com/docs/working-with-pivot-tables)」を参照してください。

##### **定義と主要な概念 (Definitions and key concepts)**
ピボットテーブルに値が含まれている場合、またはテーブルのグルーピングに計算が含まれている場合に、総計が計算されます。ピボットテーブルに値が含まれ、ピボット行またはピボット列として複数の列が追加されている場合、またはテーブルに計算を含む複数のグルーピングがある場合に、小計が計算されます。

デフォルトでは、合計はピボットテーブルまたはテーブルグルーピングの対応する値と同じ数式を使用して計算されますが、より高いレベルのデータのグルーピングに適用されます。合計の計算に使用される数式を変更したい場合は、「[合計と小計をカスタマイズする](#customize-totals-and-subtotals)」を参照してください。

総計の計算はテーブルまたはピボットテーブル全体に対して実行され、小計の計算はデータの各グルーピングに対して実行されます。
* **総計 (Grand total):** ピボット行、ピボット列、またはグルーピング計算の**すべて**の値の集計計算。例のスクリーンショットでは、総計はピンクでハイライトされています。
* **小計 (Subtotal):** ピボット行、ピボット列の**グループ**、または特定のテーブルグルーピングの値の集計計算。例のスクリーンショットでは、小計は黄色でハイライトされています。
<img width="1319" height="554" alt="c6fff12-grand-and-sub-totals-both" src="https://github.com/user-attachments/assets/4623c309-944a-423d-b7ae-305be89adf65" />

グループ化されたテーブルでは、各グルーピングの総計のみが数式で使用できます。ピボットテーブルでは、存在するピボット行、列、または値の数に応じて、`Subtotal`や`PercentOfTotal`などの関数で、他の計算済み合計を数式で使用できる場合があります。
* **行合計 (Row Total):** 行の総計。ピボット行全体の値を集計します。複数のピボット行がある場合、これはグルーピングの最下位レベルの行の総計です。
* **親行合計 (Parent Row Total):** 親行の総計。グルーピング内の列合計の集計に相当します。ピボットテーブルの各行グループの小計として機能します。
* **列合計 (Column Total):** 列の総計。ピボット列の値を集計します。
* **親列合計 (Parent Column Total):** 親列の総計。グルーピング内の行合計の集計に相当します。ピボットテーブルの各列グループの小計として機能します。

スクリーンショットでは、`East`と`West`の各行は、地域内のすべての州の合計を計算する親行合計を示しています。これら2つの親行合計は小計であり、合計されてピボットテーブルの総計が計算されます。月レベルの`Total`列にも列の小計があります。

計算列でピボットテーブルの合計を使用する例については、以下のチュートリアルを参照してください。
* [チュートリアル：ピボットテーブルの小計のパーセンテージを計算する](#tutorial-calculate-a-percentage-for-subtotals-in-a-pivot-table)
* [チュートリアル：行の小計のパーセンテージを計算する](#tutorial-calculate-a-percentage-for-row-subtotals)

##### **ピボットテーブルで合計を表示・非表示にする (Show and hide totals in a pivot table)**
特定のピボット行と列について、ピボットテーブルの合計を表示または非表示にすることを選択できます。ピボットテーブルでは、合計はデフォルトで表示されます。合計の表示は、ピボットテーブルが行を単一の列として表示するか、別々の列として表示するかによって異なります。

> 💡
> 合計は、ピボットテーブルに合計やカウントなどの集計値が含まれている場合に利用できます。

* **総計を非表示にする (Hide grand totals)**
    ピボットテーブルのすべての総計を非表示または削除するには、以下を実行します。
    1.  ワークブックのカスタマイズを開始するか、編集用に開きます。
    2.  変更したいピボットテーブルを選択します。
    3.  サイドパネルで`Format`を選択し、`Totals`ヘッダーをクリックしてセクションを展開します。
    4.  `Grand Totals`で、トグルをオフにします。
<img width="1071" height="503" alt="7ca84e2-hide-all-grand-totals-pivot" src="https://github.com/user-attachments/assets/0da8d869-9d56-459f-804c-ad6bb1451b44" />

* **親行合計を非表示にする (Hide parent row totals)**
    行レベルの総計のみを非表示または削除するには、以下を実行します。
    1.  ピボットテーブルまたはエディタパネルで、列名の隣にある下矢印()を選択します。
    2.  ドロップダウンメニューで`Show totals`を選択し、チェックマークが消えるようにします。
<img width="1183" height="513" alt="0d87323-hide-column-grand-totals-pivot" src="https://github.com/user-attachments/assets/8c4c6146-c34c-445a-a5fe-b376fdb1e1b3" />

##### **小計を非表示にする (Hide subtotals)**
ピボットテーブルの小計を非表示または削除するには、以下を実行します。
1.  エディタパネルで、`Element format`を選択します。
2.  `Totals`を選択して、合計の書式設定セクションを開きます。
3.  `Subtotals`で、トグルをオフにします。
<img width="1041" height="437" alt="401bc93-hide-subtotals-column-view-pivot" src="https://github.com/user-attachments/assets/2b188739-11b8-4b55-9aad-8e40de33d092" />

列レベルの総計のみを非表示または削除するには、以下を実行します。
1.  ピボットテーブルまたはエディタパネルで、列名の隣にある下矢印()を選択します。この例では、`Quarter of Date`列です。
2.  ドロップダウンメニューで`Show totals`を選択し、チェックマークが消えるようにします。
3.  `Total`列がピボットテーブルから削除されます。
<img width="1183" height="513" alt="0d87323-hide-column-grand-totals-pivot" src="https://github.com/user-attachments/assets/502d3111-e1fc-4aef-9efa-d9ec86f6fd4b" />

##### **合計と小計をカスタマイズする (Customize totals and subtotals)**
グループ化されたテーブルとピボットテーブルの合計と小計の計算に使用される数式をカスタマイズすることで、より柔軟なレポートを構築します。異なる集計を設定するか、カスタム数式を記述してカスタム合計またはカスタム小計を設定します。集計数式をカスタマイズしなくても、合計と小計に使用される[ラベルをカスタマイズする](https://help.sigmacomputing.com/docs/pivot-table-totals-and-subtotals#customize-total-labels)こともできます。

* **小計の集計を変更する (Change aggregate of a subtotal)**
    ピボットテーブルまたはグループ化されたテーブルの小計の集計を変更するには（例えば、`Sum()`から`Avg()`へ）、以下を実行します。
    1.  調整したい合計が表示されていることを確認します。
    2.  合計を持つピボットテーブルまたはグループ化されたテーブルを選択します。
    3.  小計または合計について、合計の行または列を探して選択します。
    4.  以下のいずれかを実行します。<img width="675" height="703" alt="10f87fdd591832fc1e09e07ab7afdc89f329979309e8ecbde88ee826f8288f8f-cs-set-agg-menu" src="https://github.com/user-attachments/assets/8c556dc4-ed6a-4baf-b4c0-afb272b38f33" />

        * 合計の行または列の任意のセルを右クリックしてコンテキストメニューを開きます。<img width="1080" height="519" alt="f8f610d2db58346dbbe8fb2cec6f6d964f53120e5da55de8a64567445400ab81-cs-grouped-subtotal-avg" src="https://github.com/user-attachments/assets/897de9d1-7d5d-4611-8008-211f4906866f" />

        * 関連するピボット行、列、または上位レベルのテーブルグルーピング列について、下矢印()をクリックして列メニューを開きます。
    5.  `totals`を選択し、`Set aggregate`を選択して関連する集計関数を選択します。デフォルトは`Auto`（`Sum`）です。

* **小計または総計のカスタム数式を記述する (Write a custom formula for a subtotal or grand total)**
    小計または総計を計算するためにカスタム数式を記述するには、以下を実行します。
    1.  カスタマイズしたい合計の行または列を探します。
    2.  合計の行または列で、セルを選択して数式バーに数式を表示させます。
<img width="1102" height="675" alt="6ebec90d4074d31ab021d4e20e2d1e6b3d0b921feae468f0bfc73539d656479e-cs-pivot-formula" src="https://github.com/user-attachments/assets/5d7e4126-f186-49e5-8112-136aded2428b" />

    3.  数式バーで数式を更新します。
       例えば、各`Stadium Level`のすべての製品タイプの合計を計算しつつ、総計から最もパフォーマンスの低い製品タイプを除外するには、`Sum([Quantity])`を   `Sum([Quantity]) - Min([Sum of Quantity (Parent Row Total)])`に置き換えます。
> 📘
> あなたの数式は、トップレベルの値ではなく、集計された値に適用されなければなりません。そうしないと、非集計の結果が表示される可能性があります。

数式はすべての`Stadium Level`の総計で更新され、総計のラベルは`Custom grand total`に変わります。

[任意] 合計行のラベルを修正します。「[合計ラベルをカスタマイズする](https://help.sigmacomputing.com/docs/pivot-table-totals-and-subtotals#customize-total-labels)」を参照してください。
<img width="1104" height="677" alt="775fdf901c6924bd9520d12b6abe90ebb8b95e8ec0799047a199552c270792d6-cs-pivot-end" src="https://github.com/user-attachments/assets/b5a52c63-cab2-4e03-9510-8fb2a606ea53" />

##### **例：ピボットテーブルの総計をカスタマイズする (Example: Customize pivot table grand totals)**
例えば、野球場のさまざまなレベルでの特定の製品タイプと製品ラインの売上を示すピボットテーブルがある場合、特定のスタジアムレベルで最もパフォーマンスの低い製品タイプの売上を除外する数式に総計を設定して、特定のスタジアムレベルで特定の製品タイプの販売を停止した場合の全体的な売上にどのように影響するかを確認できます。


1.  ワークブックにピボットテーブルを追加し、`MLB_STADIUM_SALES_HANDS_ON_LAB`テーブルをデータソースとして使用します。
2.  ピボットテーブルを次のように構成します。
    * `Product Type`と`Product Line`列をピボット行として追加します。
    * `Stadium Level`列をピボット列として追加します。
    * `Sales Quantity`列をピボット値として追加します。これは自動的に`Sum of Sales Quantity`として集計されます。列の名前を`Total Sales Volume`に変更します。
    * ピボットテーブルの表示を`Display as separate columns`に設定します。
    > 📘
    > この例では、小計は青で、総計セルは茶色で条件付き書式を使用してハイライトされており、フィルターが表示される製品タイプの数を制限しています。<img width="1382" height="668" alt="776a16dee7e8cca360d4be551b4eb7ae42658626a7eecddf3835498949c03154-cs-pivot-start" src="https://github.com/user-attachments/assets/9b5d387a-e7e8-4e96-8c9f-2dbb9eb2f216" />

3.  各スタジアムレベルで最もパフォーマンスの低い製品ラインの売上を除外するカスタム数式に総計を変更するには、総計の行を探します。

    * 総計の列は、すべてのスタジアムレベルにわたる各製品ラインの総販売量を計算し、総計の行は、各スタジアムレベルのすべての製品タイプの総販売量を計算します。
4.  総計の行のセルを選択し、数式を`Sum([Sales Quantity])`から`Sum([Sales Quantity]) - Min([Total Sales Volume (Parent Row Total)])`に変更します。<img width="1102" height="675" alt="6ebec90d4074d31ab021d4e20e2d1e6b3d0b921feae468f0bfc73539d656479e-cs-pivot-formula" src="https://github.com/user-attachments/assets/4fa63e34-0249-47c4-9592-ba12982f2dd0" />

 行の総計値が更新され、ラベルが`Custom grand total`に更新されます。
<img width="1104" height="677" alt="775fdf901c6924bd9520d12b6abe90ebb8b95e8ec0799047a199552c270792d6-cs-pivot-end" src="https://github.com/user-attachments/assets/ed283e61-0b8b-4057-bda1-f34f71ac4656" />

##### **合計ラベルをカスタマイズする (Customize total labels)**
テーブルまたはピボットテーブルの小計または総計のラベルをカスタマイズできます。
1.  名前を変更したい合計ラベルをテーブルまたはピボットテーブルで探します。
2.  ラベルをダブルクリックして編集可能にし、新しいラベルを入力します。<img width="1038" height="447" alt="4daaa66fe8c0a4ccc641987e79970d9ca71d0e3898bc4cf8f18e27d658cf8d40-cs-rename-start" src="https://github.com/user-attachments/assets/2a53dbd6-6e8b-4c1e-adb9-b801a2dec63f" />

    > 📘
    > 小計のラベルを変更すると、そのレベルと値の組み合わせのすべての小計ラベルが変更されます。
3.  キーボードのenterを押すか、セルの外側をクリックして新しいラベルを保存します。
    > 💡
    > 合計または小計のデフォルトラベルに戻すには、既存のラベルを削除します。ラベルをダブルクリックして既存のラベルを削除し、enterを押して変更を保存します。
<img width="1041" height="446" alt="507f4cf608e62796334e474459ac631144cfdb458241fea2aff340d2f5c7bef1-cs-rename-end" src="https://github.com/user-attachments/assets/d14ef573-980c-4795-bc68-91f092e4adb0" />

##### **合計と小計をカスタマイズする際の制限事項 (Limitations when customizing totals and subtotals)**
名前が変更された小計と総計のラベルは、下流では更新されません。合計にカスタム数式を持つピボットテーブルまたはグループ化されたテーブルから作成された子テーブルは、元の列名を表示します。合計または小計の値を参照するサマリーメトリクスなどの数式は、代わりに元の列名を参照する必要があります。
* `<Values Column Name> (Parent Row Total)` ピボット行の小計用。
* `<Values Column Name> (Row Total)` ピボット行の総計用。
* `<Values Column Name> (Parent Column Total)` ピボット列の小計用。
* `<Values Column Name> (Column Total)` ピボット列の総計用。
* `<Values Column Name> (Grand Total)` ピボットテーブルまたはグループ化されたテーブルの行と列の両方の値の総計用。

カスタム小計数式の後、交差する合計が意味をなさない場合、小計が交差するセルは空白になることがあります。例えば、一方の小計が平均を計算し、もう一方の小計が最大値を計算する場合などです。
<img width="1170" height="458" alt="71b0b0ae9e9b875bdadc35c92de22376567acdab091cc2383c22ae323a6a23f9-cs-pivot-intersect" src="https://github.com/user-attachments/assets/ee0f82e1-591c-419a-b7e1-cbe0615a0d4c" />

##### **チュートリアル：ピボットテーブルの小計のパーセンテージを計算する**
この例では、特定の地域で販売された総ユニット数のパーセンテージを計算します。この例では、Sigmaサンプルデータベースに含まれる`PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA`テーブルを使用します。ピボット行に`Store Region`と`Store State`、集計値に`Sum of Quantity`を持つピボットテーブルから始めます。<img width="713" height="457" alt="2675ef2-tutorial-no-columns-start-small" src="https://github.com/user-attachments/assets/b341a64b-bea3-401e-b542-d64e06dea9c1" />

ピボットテーブルに新しい列を追加するには：
1.エディタパネルの`Values`ヘッダーで、プラス(+)をクリックします。
2.`Add New Column`を選択します。<img width="711" height="290" alt="d06ee9e-pivot-tutorial-add-new-column" src="https://github.com/user-attachments/assets/520095ba-a3d8-4197-ba05-06d3b2c03a4d" />

3.  新しい列の数式バーに、次のように入力します。
    `[Sum of Quantity (Row Total)] / [Sum of Quantity (Parent Row Total)]`<img width="1323" height="226" alt="1f5586f-pivot-tutorial-no-column-formula-bar" src="https://github.com/user-attachments/assets/1077cc62-b8f3-458f-a003-39e42bebb762" />

4.  `Enter`を押すか、チェックマークをクリックして数式を保存します。
5.  計算列をパーセンテージとして書式設定するには、ワークブックツールバーで`Format as percent`(%)をクリックします。
　　結果は以下のように表示されます。<img width="776" height="453" alt="a115575-pivot-tutorial-no-columns-end" src="https://github.com/user-attachments/assets/f754f2f9-4e6e-4475-97f8-da86ebdf08df" />

##### **チュートリアル：行の小計のパーセンテージを計算する**
このチュートリアルでは、地域と販売四半期ごとに分類された州の総小売売上高のパーセンテージを計算します。
ピボット行に`Store Region`と`Store State`、ピボット列に`Quarter of Date`に切り捨てられた`Date`、集計値に`Sum of Quantity`を持つピボットテーブルから始めます。<img width="1289" height="471" alt="48a9d03-pivot-tutorial-add-percent-column-before" src="https://github.com/user-attachments/assets/126d777e-9a1a-455a-bdd4-73734b154618" />

1.  エディタパネルの`Values`ヘッダーで、プラス(+)をクリックします。
2.  `Add New Column`を選択します。
3.  新しい列の数式バーに、次のように入力します。
    `[Sum of Quantity] / [Sum of Quantity (Parent Row Total)]`<img width="1295" height="343" alt="2935071-pivot-tutorial-with-column-formula-bar" src="https://github.com/user-attachments/assets/bcb44a71-bc9c-4a49-939a-c5627b8f5839" />

4.  `Enter`を押すか、チェックマークをクリックして数式を保存します。
5.  計算列をパーセンテージとして書式設定するには、ワークブックツールバーで`Format as percent`(%)をクリックします。
    果は以下のように表示されます。<img width="1653" height="528" alt="a05ebde-pivot-tutorial-result-with-column" src="https://github.com/user-attachments/assets/3cb9ad84-1c57-47a6-8e87-bf76c7754ae5" />

#### 4-4-5-3. ピボットテーブルの合計の書式設定 (Format pivot table totals)

[テーブルスタイル](https://help.sigmacomputing.com/docs/format-and-customize-a-table#customize-the-table-style-for-an-individual-element)を適用してテーブルまたはピボットテーブルのすべてのセルをカスタマイズすることに加えて、ピボットテーブルの合計をピボットテーブル内の他の値とは別に書式設定できます。
* このドキュメントで説明されているように、ピボットテーブルの小計と総計にユニークな書式を適用します。
* ツールバーを使用して、合計行と合計列の数値形式と外観を変更します。「[列と合計データの書式設定](https://help.sigmacomputing.com/docs/format-and-customize-a-table#format-column-and-totals-data)」を参照してください。
* 小計と総計に条件付き書式を適用します。「[条件付き書式の適用](https://help.sigmacomputing.com/docs/format-and-customize-a-table#apply-conditional-formatting-to-table-columns-and-cells)」を参照してください。

小計と総計を表示または非表示にするには、「[ピボットテーブルの合計と小計](https://help.sigmacomputing.com/docs/pivot-table-totals-and-subtotals)」を参照してください。

このドキュメントでは、ピボットテーブルの合計の書式設定オプションについて説明し、小計と総計を含む行と列の表示をカスタマイズする方法を解説します。

##### **ユーザー要件 (User requirements)**

ピボットテーブルの合計を書式設定する機能には、以下が必要です。
* `Explore workbooks`または`Create, edit, and publish workbooks`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがワークブックの所有者であるか、`Can explore`または`Can edit`の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

##### **ピボットテーブルの合計の書式設定オプション (Pivot table totals format options)**

* **小計 (Subtotals)**
    `Subtotals`ツールを使用すると、小計の行と列のフォントの太さ、フォントの色、および背景色をカスタマイズできます。
<img width="632" height="472" alt="subtotals" src="https://github.com/user-attachments/assets/1b8bc237-ed83-4b47-8efb-2b4fddaf9a90" />

* **総計 (Grand totals)**
    `Grand totals`ツールを使用すると、総計の行と列のフォントの太さ、フォントの色、および背景色をカスタマイズできます。
<img width="632" height="472" alt="grand-totals" src="https://github.com/user-attachments/assets/6edffab3-3242-4a90-9de1-61b3ad25c315" />

* **位置 (Position)**
    `Position`設定を使用すると、総計を最初または最後の列と行に移動できます。
First<img width="630" height="332" alt="position_first" src="https://github.com/user-attachments/assets/cecc994c-cbb5-45f4-bdc9-3750c09aff0d" />
Last<img width="630" height="332" alt="position_last" src="https://github.com/user-attachments/assets/1144f385-a140-4f9a-b560-452f9fb28545" />

##### **ピボットテーブルの合計を書式設定する (Format pivot table totals)**
1.  ワークブックを`Explore`または`Edit`モードで開きます。
2.  書式設定したいピボットテーブルを選択します。
3.  サイドナビゲーションで`Element format`を選択し、`Totals`ヘッダーをクリックしてセクションを展開します。<img width="1037" height="569" alt="element-format_totals" src="https://github.com/user-attachments/assets/056ef154-775b-4687-8bf3-6b42b39585e7" />

4.  `Subtotals`および`Grand totals`ツールを使用して、フォントの太さ、フォントの色、背景色をカスタマイズし、`Position`ドロップダウンでオプションを選択して総計の行と列の位置を制御します。<img width="1037" height="569" alt="element-format_totals_customize" src="https://github.com/user-attachments/assets/dc0ffed7-9d87-4d52-8a81-77649192a8e0" />


#### 4-4-5-4. 階層 (ベータ版) (Hierarchies (Beta))

> 🚩
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このページは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

階層（ヒエラルキー）を使用して、列をカテゴリ別にグループ化し、データの粒度の順序を定義します。

一般的な階層の例：
* **製品:** タイプ、ファミリー、名前
* **場所:** 大陸、国、地域、州、市
* **時間:** 年、月、週、日
* **分類学:** 界、門、綱、目、科、属、種

> 📘
> 階層はテーブル、ピボットテーブル、およびビジュアライゼーション要素で定義できますが、適用できるのはピボットテーブルのみです。

##### **階層を作成する (Create a hierarchy)**
以下のステップは、階層を作成する方法を説明します。

1.  ワークブックを`Edit`モードで開きます。
2.  階層を作成したい要素を選択します。階層はテーブルまたはピボットテーブルで作成できますが、使用できるのはピボットテーブルのみであることに注意してください。
3.  `Columns`メニューで、`+`アイコンをクリックし、`Manage hierarchies`を選択します。<img width="415" height="323" alt="5b313e0-2" src="https://github.com/user-attachments/assets/1d9b9410-959e-4346-8255-b4306a20da80" />

4.  `Manage hierarchies`モーダルで、`+ New hierarchy`をクリックし、階層のプロパティを定義します。
    * `Hierarchy name`フィールドに、階層を識別するための名前を入力します。
    * `Columns in hierarchy`セクションで、`Add column`をクリックして階層に列を追加します。<img width="602" height="396" alt="80bc313-4" src="https://github.com/user-attachments/assets/8de49853-60d9-4a64-9bf7-fb7e4d2dcacb" />

  階層に列を追加すると、この列はワークブックの`Columns`メニューで階層アイコンでラベル付けされます。アイコンにカーソルを合わせると、階層の詳細が表示されます。<img width="311" height="218" alt="ddee60f-5" src="https://github.com/user-attachments/assets/863a8711-e9c8-4c1a-b53d-08853d1a4821" />

5.  追加の階層を作成するには、`Manage hierarchies`モーダルで`+ New hierarchy`をクリックし、ステップ4を繰り返します。
<img width="602" height="396" alt="2fb3281-6" src="https://github.com/user-attachments/assets/7ce693e6-49b7-4a08-aac8-d717b37a621b" />

##### **階層を管理する (Manage a hierarchy)**
階層の名前の変更、列の並べ替え、新しい列の追加、既存の列の削除、または階層全体の削除ができます。

1.  `Manage hierarchies`モーダルで、更新したい階層を選択します。
2.  階層の名前を変更するには、`Hierarchy name`フィールドを編集します。
3.  列を並べ替えるには、`Columns in hierarchy`セクションに移動し、必要に応じて列名をドラッグ＆ドロップします。<img width="785" height="604" alt="e0b38f8-7" src="https://github.com/user-attachments/assets/574eb186-8c17-4886-a368-a79b40c3bd94" />

4.  新しい列を追加するには、`Columns in hierarchy`セクションに移動し、`Add column`をクリックします。
5.  階層から列を削除するには、`Columns in hierarchy`セクションで列名を探し、`Remove column`をクリックします。<img width="602" height="396" alt="8f144c9-8" src="https://github.com/user-attachments/assets/a78f17ba-7fe6-4e80-92ad-5da9df624279" />

6.  階層を削除するには、左パネルで階層名を探し、`Delete hierarchy`をクリックします。<img width="602" height="396" alt="90fdbbd-9" src="https://github.com/user-attachments/assets/a60cf592-9c0e-47ae-b6c0-235f8843ee9e" />


##### **階層の継承 (Hierarchy inheritance)**
子要素は、親要素で定義されたすべての階層を継承します。継承された階層は子要素から削除または変更することはできませんが、完全な編集権限を持つ新しい階層を追加することはできます。
`Manage hierarchies`モーダルで階層が選択されると、Sigmaはそれが親要素から継承されたものであるかどうかを示します。
<img width="600" height="398" alt="746220c-10" src="https://github.com/user-attachments/assets/2c26a3e9-c421-46fa-8095-c94554666936" />

##### **階層を使用する (Using hierarchies)**
以下のステップは、定義された階層をピボットテーブルで使用する方法を説明します。
1.  階層を持つピボット行を作成するには、`Pivot Rows`プロパティに移動し、`Add new column`をクリックします。
2.  `Add new column`メニューで、定義された階層を選択します。<img width="481" height="580" alt="ac7bab6-12" src="https://github.com/user-attachments/assets/a893b167-d033-46c9-b603-e907f2afc484" />

3.  階層をピボット値に適用するには、`Values`プロパティに移動し、`Add new column`をクリックします。
4.  `Add new column`メニューで、定義された階層を選択します。<img width="547" height="754" alt="d6a3910-13" src="https://github.com/user-attachments/assets/cc8aad02-eaf7-4eff-92da-0cd38bf0c3b7" />

結果のピボットテーブルは、構成された階層を示します。
<img width="799" height="392" alt="7bc59d0-14" src="https://github.com/user-attachments/assets/b243d0c5-f809-468f-9951-f17da219ff15" />

##### **制限事項 (Limitations)**
* 階層はピボットテーブルでのみ使用できます。
* 階層は単一のワークブック内に存在し、データセットや他のワークブックには渡されません。
* 階層を更新しても、Sigmaは現在それを使用しているピボットテーブルにそれらの変更を適用しません。

### 4-4-5-7. テーブルの転置 (ベータ版) (Transpose a table (Beta))

> 🚩
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このページは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

Sigmaは、テーブルを行から列へ、または列から行へ転置することをサポートしています。データを転置することは、個々のユースケースに応じてデータをピボットまたはアンピボットできるため、データ分析に役立ちます。

例えば、下のテーブルは駐車場の入出庫の記録を示しており、各行が各車の入庫日と出庫日を示しています。
すべての日付値が単一の行になるようにデータを整形するには、行から列への転置を実行でき、その結果、テーブルは次のように変換されます。
<img width="444" height="104" alt="5a2bfacbe27d0f3c2068919eac137242c52fdb6552bfa07cb4cb2f2f80bfe317-carexample" src="https://github.com/user-attachments/assets/02784fce-de92-48bd-98fd-a09bddac3e71" />

これは、特定のチャートタイプに合わせてデータを再形成したい場合（例えば、折れ線グラフには単一の列に方向付けられた日付値が必要な場合など）に特に役立ちます。
<img width="450" height="166" alt="d7193a2cc515a058a135b032b07360038eb6f1c9330ebf2642682cb43c9fc576-cartransposed" src="https://github.com/user-attachments/assets/a5b3e82f-6282-4131-872a-b7d729b1c31f" />

このドキュメントでは、データを[行から列へ](https://help.sigmacomputing.com/docs/transpose-a-table#transpose-row-to-columns)、または[列から行へ](https://help.sigmacomputing.com/docs/transpose-a-table#transpose-columns-to-rows)転置する方法を説明し、それぞれの例を含んでいます。

#### **システムとユーザーの要件 (System and user requirements)**
ワークブックの所有者であるか、ワークブックに対する`Can explore`または`Can edit`のアクセス権を付与されている必要があります。

#### **制限事項 (Limitations)**
* 入力テーブルの転置はサポートされていません。
* 計算列の転置はサポートされておらず、既存のフィルタリング、ソート、またはグルーピングは転置された出力に反映されません。これは、転置がワークブック内の要素ではなく、データプラットフォームのデータに対して実行されるためです。
* 行を列に転置する場合、単一の列から転置できるユニークな行の値は200個に制限され、最大200列になります。列を行に転置する場合、制限はありません。

#### **行を列に転置する (Transpose row to columns)**
テーブルの行を列に転置して、特定の列の値をテーブルの列ヘッダーとして使用できます。例えば、`Store Region`列の行を転置して、`Store Region`列の値（East, Midwest, Southなど）を列ヘッダーとして使用し、それらの地域の値の集計値を表示します。

行を列に転置するには：
1.  目的のテーブルから、`More`を選択します。
2.  `Element source`から、`Transpose`を選択します。
3.  `Transpose Table`モーダルで、`Row to column`を選択します。
4.  目的の`Column to transpose`を選択します。転置されると、この列のデータは、各ユニークな値が新しい列になるように再配置されます。
    > ❗️
    > 選択した列に200を超えるユニークな値がある場合、転置されたテーブルで200を超える列が生成されるため、エラーが表示されます。
5.  `Value column`を選択します。これは、`Aggregate`で選択した計算に使用される列です。
6.  希望する`Aggregate`メソッドを選択します。表示される集計メソッドは、選択された`Value column`のデータ型によって異なります。
7.  目的の`Output columns`の隣にあるチェックボックスを選択します。これらは転置された出力に含めたい列であり、転置における他の計算には影響しません。転置されたテーブルのプレビューは`Output preview`で利用できます。
    * 列を選択した順序が、テーブルに左から右へと表示される順序になります。
　  元のソーステーブルの残りのソース列は、転置をグループ化するために使用されます。
8.  `Submit`を選択します。

##### **例：勝敗数のカウント (Example: Counting games won and lost)**
例えば、チームがホームでプレイした野球の試合のテーブルがあり、各試合ごとに1行のデータと、対戦相手、結果、試合後のディビジョンランクの列があるとします。
チームが各ディビジョンランクで勝ったまたは負けた総試合数を計算したい場合、ディビジョンランクでテーブルを転置できます。
<img width="1476" height="798" alt="54ace8ffa9210d93d5ee36eb0e499a42879d3a6d8eaaa17eec7c20f481f91883-transpose1" src="https://github.com/user-attachments/assets/c51eaabc-b407-4fbe-aa81-ac12aefa0d0b" />

このカウントを取得するには：
1.  `Row to column`転置を選択します。
2.  `L`（敗戦）と`W`（勝利）を転置されたテーブルの列ヘッダーとして設定するには、`Win Loss`を`Column to transpose`として選択します。
3.  特定の対戦相手に対する勝利数または敗戦数を計算するには、`Opponent`を`Value Column`として選択します。
4.  nullでなく空でもない値の数を計算するには、`Aggregate`に`Count`を選択します。
5. `Division Rank`、`L`、`W`を`Output columns`として選択します。テーブルの出力は、残りの唯一のソース列であるため、自動的に`Division Rank`でグループ化されます。これにより、各ディビジョンランクでの勝敗の合計`Count`が集計されます。

1. 出力を`Start Time`のような別の列で追加的にグループ化したい場合があるかもしれません。これを行うには：
`Output columns`で、`Start Time`を選択します（既存の`Division Rank`、`L`、`W`の選択は維持します）。各試合の開始時刻について、転置は各ディビジョンランクでの勝敗数を表示します。すべての開始時刻が4つすべてのディビジョンランクを表示するわけではないことに注意してください。それらの時刻には勝敗が記録されていないためです。

2. [任意] 出力を理解しやすくするために、`Start Time`列を昇順でソートすることもできます。これにより、データはその日の最も早い試合から最も遅い試合へとソートされます。`Start Time`列で、右クリックまたは下矢印()をクリックして列メニューを開き、`Sort ascending`を選択します。ソートされると、出力は次のようになります。
<img width="629" height="509" alt="950116fb0cf84de188cdff2f32b9ebff80e898b3cde615dee8148973423a4def-sortedtranspose" src="https://github.com/user-attachments/assets/6f5aef6f-60d4-488b-b4b3-16271c754de0" />

各ディビジョンランクで、あなたのチームが勝利または敗北したユニークな対戦相手の数を知りたい場合もあるでしょう。これを取得するには：
`Aggregate`メソッドを`CountDistinct`に変更します。`CountDistinct`は、`Opponent`列内のユニークな値の数を提供します。この値は、チームが各ディビジョンランクで打ち負かした異なる対戦相手の数を表します。あなたの出力は次のようになります。<img width="480" height="192" alt="ac42dd3dc777fadc51f90e37a2622a8f1a5a9510d17c2ca5f3d5f3baaa076395-countdistinct" src="https://github.com/user-attachments/assets/f027f736-c131-4672-be56-5095aaaabed7" />

##### **列を行に転置する (Transpose columns to rows)**
1.  目的のテーブルから、`More`を選択します。
2.  `Element source`から、`Transpose`を選択します。
3.  `Transpose Table`モーダルで、`Column to row`を選択します。
4.  マージしたい`Columns to merge`を選択します。
5.  マージされた列の`Column label for merged columns`を入力します。このラベルは、マージされた列の以前のヘッダー値を含む新しい列の列ヘッダーです。
6.  値の`Column label for values`を入力します。これは、マージされた列の値を含む新しい列の列ヘッダーです。
7.  目的の`Output columns`の隣にあるチェックボックスを選択します。
8.  `Submit`を選択します。

##### **例：監査ログイベント時刻のマージ (Example: Merging audit log event times)**
例えば、監査ログイベントのテーブルがあるとします。各行は、コネクタID、テーブル名、テーブルへの書き込み開始/終了、同期開始/終了、およびユニークなテーブル同期キーなどの情報を持つ、ユニークなテーブル同期の詳細を示します。

すべてのテーブルイベントとそのタイムスタンプの行を持つテーブルが必要な場合、テーブルを転置してこれらの列をマージできます。この新しいテーブルを取得するには：
<img width="1301" height="797" alt="6a2f4de6ceef391b5d07e2c72041deb8c0172cb1faafa97cd7dad302961a40eb-transpose2" src="https://github.com/user-attachments/assets/17746c02-a0b2-46a7-a63d-4503fe5f4fcb" />

1.  `Column to row`転置を選択します。
2.  `Columns to merge`には、`Write to Table Start`, `Write to Table End`, `Sync Start`, `Sync End`を選択します。これらはすべて1つの列にマージされます。
3.  `Column label for merged columns`には、マージされた列の名前として`Event Type`を入力します。
4.  `Column label for values`には、`Timestamp`を入力します。
5.  テーブルに表示したい行を選択します：`Unique Table Sync Key`（どのテーブルにイベントがリンクされているかが明確になるように）、および新しい列である`Event type`と`Timestamp`。
6.  [任意] 出力を理解しやすくするために、`Unique Table Sync Key`列を昇順でソートすることもできます。これにより、各テーブルのイベントが順序付けられた行になります。テーブルを1つの列で昇順にソートするには、右クリックまたは下矢印()をクリックして列メニューを開き、`Sort ascending`を選択します。

#### **転置を元に戻す (Undo a transpose)**
転置を元に戻す最も効果的な方法は、要素のソースを元のデータソースに変更することです。詳細は、「[ワークブックまたは要素のデータソースを変更する](https://help.sigmacomputing.com/docs/change-the-data-source-for-a-workbook-or-element)」を参照してください。

### 4-6-1. カスタムSQLを記述する (Write custom SQL)

SQLエディタを使用してデータプラットフォームを探索する際、SQLクエリをプレビューし、SQLから直接ワークブック、データモデル、データセットを作成できます。

このドキュメントでは、以下の方法について説明します。
* [SQLからワークブックを作成する](#create-a-workbook-from-sql)
* [SQLワークブック要素を作成する](#create-a-sql-workbook-element)
* [既存のSigmaワークブック要素を参照する](#reference-existing-sigma-workbook-elements)
* 以下を含む[ショートカット](https://help.sigmacomputing.com/docs/write-custom-sql#shortcuts)を使用する：
    * SQLベースのワークブックデータ要素内で、並列表示のインラインSQLエディタに切り替える。
    * SQLクエリを自動フォーマットする。
    * SQLクエリ内で検索と置換を使用する。

#### **要件 (Requirements)**
* この機能を使用するには、`Write SQL`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* カスタムSQLを実行するには、接続全体に対する`Can use`[アクセス権](https://help.sigmacomputing.com/docs/data-permissions)が付与されている必要があります。「[Manage access to data and connections](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
* SQLエディタは、組織内の少なくとも一つの接続に対して接続レベルのアクセス権を持っている場合にのみ表示されます。

#### **SQLからワークブックを作成する (Create a workbook from SQL)**
SQLクエリからワークブックを作成するには、以下を実行します。
1.  **Sigmaホーム**を開きます。
2.  ナビゲーションパネルで`+ Create New`をクリックし、`Write SQL`を選択してSQLエディタを開きます。<img width="350" height="424" alt="012c84e6e4c0d1dc1ea78ae375c0eb9f3019feddc58c57d4e6de7a49dd835548-sql-create-new" src="https://github.com/user-attachments/assets/f0445fbf-166f-466f-a5d3-a810aa4d0662" />

3.  サイドパネルで`Select a Connection`をクリックし、クエリを実行したい接続を選択します。
4.  クエリエディタに、SQLクエリを入力します。Sigmaはガイドするためのオートコンプリート候補を提供します。
    > 💡
    > SQL内でワークブックのコントロールを参照するには、コントロールIDを中括弧で囲みます。「[Reference workbook controls](https://help.sigmacomputing.com/docs/reference-workbook-control-values-in-sql-statements)」を参照してください。<img width="1129" height="571" alt="771da6b1a1c971c1a9a8e7934cdb2943f6ac7965c03df86096a6b03f26da7ece-sql-better-exploration" src="https://github.com/user-attachments/assets/cac663ca-6df7-43e2-aeb3-c7bad933d077" />

5.  SQLクエリを実行するには、`Run`をクリックするか、キーボードショートカット `⌘` + `return` (Mac) または `ctrl` + `enter` (PC) を使用します。
6.  未公開のワークブック（探索）をワークブックとして保存するには、`Save As`をクリックします。
    > 💡
    > SQLクエリをデータモデルに変換するには、要素メニューを開くために`More`を選択し、次に`Advanced options` > `Create data model`を選択します。

#### **SQLワークブック要素を作成する (Create a SQL workbook element)**
既存のワークブックにSQL要素を追加して既存の分析を補完するには、以下を実行します。
1.  編集用にワークブックを開きます。
2.  要素追加バーで、追加したい要素のタイプを選択し、次に特定の要素タイプを選択します：`Data` > `Table`, `Data` > `Pivot Table`または`Chart`およびサポートされている任意のチャートタイプ。
3.  `Select source`モーダルで、下部にある`SQL`オプションを選択します。<img width="484" height="790" alt="eaa2b6d9b9907a45801a87a2faeece3e576f135fdea3cb9814076115a9eda805-sql-source-pick" src="https://github.com/user-attachments/assets/a1a7e8d3-ef1b-46f3-af5f-8a3947f16b4e" />

4.  クエリを実行したい接続を選択します。 ワークブックに要素が表示され、接続にクエリを実行するためのSELECTステートメントを入力するよう促されます。<img width="859" height="502" alt="8042db867cdd5489a2b8a5d29ce7cc49a37dc71b82018f4698b3cab45659080a-sql-autocomplete" src="https://github.com/user-attachments/assets/e44b8521-2536-4477-b010-92692d03da13" />

5.  クエリエディタに、カスタムSQLを入力します。Sigmaはガイドするためのオートコンプリート候補を提供します。<img width="859" height="502" alt="8042db867cdd5489a2b8a5d29ce7cc49a37dc71b82018f4698b3cab45659080a-sql-autocomplete" src="https://github.com/user-attachments/assets/85817eb0-033e-4e59-be72-b3bd833f3574" />

    > 💡
    > SQL内でワークブックのコントロールを参照するには、コントロールIDを中括弧で囲みます。「[Reference workbook controls](https://help.sigmacomputing.com/docs/reference-workbook-control-values-in-sql-statements)」を参照してください。

#### **システム関数でユーザー属性を参照する (Reference user attributes with system functions)**

現在のユーザーの属性を参照するには、SQLステートメントで`{{system::SystemFunction}}`構文を使用します。使用できるシステム関数のリストについては、「[システム関数](https://help.sigmacomputing.com/docs/system-functions)」を参照してください。

例えば、ワークブック内の`PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA`というタイトルのデータ要素で、`Customer Name`列が現在の（サインインしている）ユーザーの名前と一致するレコードをクエリするには、以下のようなSQLステートメントを記述します。
```sql
SELECT *
FROM sigma_element('PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA')
WHERE "Customer Name" = {{system::CurrentUserFullName}}
```
#### **ショートカット (Shortcuts)**
SigmaでSQLを扱いやすくするためのいくつかのショートカットが存在します。

##### **要素メニューでSQLエディタを切り替える (Toggle SQL editor in the element menu)**
ワークブックが公開されると、SQL要素は結果のみを表示します。ワークブックを編集または探索する際、SQLエディタを切り替えて、結果を生成するSQLクエリを表示できます。
`Toggle SQL Editor`をクリックして、データ要素とSQLクエリエディタを切り替えます。

##### **SQL要素を最大化する (Maximize the SQL element)**
ワークブックキャンバスでSQL要素を最大化し、長く複雑なSQLクエリを書きやすくするには、スペースバーを押すか、`Maximize element`をクリックして要素をフルスクリーンモードに展開します。

##### **SQLをフォーマットする (Format SQL)**
長いSQLテキストブロックを素早くフォーマットするには、`Format SQL`をクリックします。
![77596fe-formatsql](https://github.com/user-attachments/assets/4cdc2a54-e93e-4e14-8d2c-bab795dcb2e7)

##### **検索と置換 (Find and replace)**
SQLクエリ内で検索し、任意で検索語のインスタンスを置換するには、`Search SQL`をクリックするか、キーボードショートカット `⌘ + F` を使用します。
<img width="978" height="539" alt="020b488-Screenshot_2024-05-15_at_3 35 57_PM" src="https://github.com/user-attachments/assets/a475cda9-168b-4175-b85b-dab54589bbe8" />

##### **リネージビューからカスタムSQLにアクセスする (Access custom SQL from the lineage view)**
ワークブックまたはデータモデルのリネージビューからカスタムSQLを表示および編集します。クエリ全体をクリップボードにコピーするか、`Edit SQL`をクリックして要素のインラインSQLエディタに移動します。
リネージの操作に関する詳細は、「[View workbook and data model data lineage](https://help.sigmacomputing.com/docs/view-workbook-data-lineage)」を参照してください。
<img width="1133" height="710" alt="c5ab9c054a92da392aaa2554814f02e4b971ea3b16ef77665031ed5f2565c281-sql-lineage" src="https://github.com/user-attachments/assets/b4a80369-62df-4597-acc9-2e23c62eda64" />

##### **クエリ履歴を表示する (View the query history)**
SQLエディタを使用する際、現在の接続に対して最近実行されたクエリの履歴にアクセスできます。
この履歴にアクセスするには、サイドパネルの`DB`タブをクリックし、`History`タブを選択します。
特定のワークブックまたはデータモデルのすべての要素のクエリ履歴を表示するには、「[Examine workbook queries](https://help.sigmacomputing.com/docs/examine-workbook-queries)」を参照してください。<img width="263" height="222" alt="fe62cf3964dcfcaf8dea2f3a7fc27ff8aedb4e553c59df3647a35be57860ebd3-sql-qh" src="https://github.com/user-attachments/assets/279ab8c4-edd9-40a3-a37c-82816d02fe96" />


##### **テーブルプレビューを表示する (View table previews)**
クエリを記述する際、サイドパネルを使用してデータプラットフォーム内のテーブルを探索できます。特定のテーブルに移動し、`Preview`を選択してテーブルの列と行のプレビューを開き、そのテーブルを既存のSQLクエリに追加するかどうかを決定するのに役立てることができます。
特定のテーブルについて、`More`を選択し、`Place name in SQL`または`Place select statement in SQL`を選択して、SQLクエリで新しいテーブルを簡単に参照します。

#### **例 (Examples)**
より高度なカスタムSQLのケースについては、これらの例を参照してください。

##### **ユーザー属性に基づいて出力を変更する (Change output based on a user attribute)**
組織でユーザー属性が定義されている場合、属性を参照して、現在のユーザーのユーザー属性の値に基づいてSQLクエリから返される結果を制限できます。
例えば、Plugs Electronicsのサンプルデータについて、`store_region`ユーザー属性に基づいて現在のユーザーがアクセスできる店舗地域の結果のみを返します。
```sql
SELECT
  *
FROM
  EXAMPLES.PLUGS_ELECTRONICS.PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA
WHERE 
  {{system::CurrentUserAttributeText::store_region}} = STORE_REGION
```
別の例として、割り当てられたorganization_nameユーザー属性の値に基づいて、現在のユーザーが表示を許可されているcustomer_nameでフィルタリングされた結果を返します。

```sql
SELECT 
  * FROM 
  test.orders 
WHERE 
  customer_name = {{system::CurrentUserAttributeText::organization_name}}
```
関数構文の詳細については、「CurrentUserAttributeText」を参照してください。ユーザー属性と割り当ての詳細については、「User Attributes」を参照してください。

##### **特定の日付範囲コントロールの出力を返す (Return output for a specific date range control)**
日付列が日付範囲コントロールで指定された値と一致する場合にのみ行を返す例については、「Reference workbook control values in SQL statements」のサンプルSQLを参照してください。

##### **複数選択コントロールの値に応じて行を返す (Return rows depending on the value of a multi-select control)**
複数選択リストコントロールの値に応じて行を返す例については、「Reference workbook control values in SQL statements」のサンプルSQLを参照してください。

##### **スキーマテキストセレクタに基づいて行を返す (Return rows based on a schema text selector)**
有効な選択（接続されたCDW内のスキーマ）を持つ`schema-param`という単一選択またはテキストコントロールがあり、指定されたスキーマに`STATIONS`テーブルが存在する場合、以下のサンプルSQLは指定されたスキーマの`STATIONS`列からすべての列を返します。

```sql
SELECT *
FROM {{#raw schema-param}}.STATIONS
```
> 🚩
> `#raw`構成値を使用すると、行レベルのセキュリティがバイパスされ、セキュリティの脆弱性が生じる可能性があります。
> このパラメータを使用してテーブル、スキーマ、またはデータベース名を交換する場合、SQLで参照される列名は同一でなければなりません。
> 
### 4-7-2. SQLステートメントでワークブックのコントロール値を参照する (Reference workbook control values in SQL statements)

Sigmaで[SQLステートメントを記述する](https://help.sigmacomputing.com/docs/write-custom-sql)際、コントロールIDを中括弧で囲むことで、SQLステートメント内でコントロールの値を参照できます。
`{{my-control-id}}`

コントロールIDは、コントロールの`Settings`タブで見つけることができます。コントロールIDの詳細については、「[Reference control values in a formula](https://help.sigmacomputing.com/docs/reference-control-values-as-parameters)」を参照してください。

正確な構文は、コントロールの出力タイプによって異なります。
* **単一の値 (Single value)** (ほとんどのコントロールタイプ)
* **最小/最大値 (Min/max values)** (数値範囲または範囲スライダー)
* **開始/終了値 (Start/end values)** (日付範囲コントロール)
* **複数の値 (Multiple values)** (複数選択リストコントロール)

#### **制限と警告 (Limitations and warnings)**
* コントロールの値を変更した結果、異なるスキーマを持つテーブルにクエリを実行するステートメントになると、クエリは期待とは異なる列を生成し、エラーを引き起こします。
* `#raw`構成値を使用すると、ワークブックまたはワークシートで行レベルのセキュリティがバイパスされ、セキュリティの脆弱性が生じる可能性があります。

#### **SQLで単一値コントロールの出力を参照する (Reference single value control output in SQL)**
SQLステートメントで、特定のコントロールで選択または指定された値（出力）を参照できます。単一の値を出力するコントロールの場合、構文は以下の通りです。

* **サポートされるコントロールタイプ**
    Single select list, Text input, Text area, Number input, Date, Segmented, Drilldown, Slider, Checkbox, Switch, Top N

* **構文 (Syntax)**
    数式でコントロール値を参照するには、コントロールIDを二重中括弧で囲み、以下の構文を使用します。
    `{{New-Control-ID}}`

#### **SQLで数値範囲または範囲スライダーコントロールの値を参照する (Reference number range or range slider control values in SQL)**
SQLステートメントで、特定のコントロールで選択または指定された値を参照できます。数値の範囲を出力するコントロールの場合、構文は以下の通りです。

* **サポートされるコントロールタイプ**
    Number range, Range slider

* **構文 (Syntax)**
    最小値を取得するには、以下の構文を使用します。
    `{{Range-Control-ID}}:min`
    最大値を取得するには、以下の構文を使用します。
    `{{Range-Control-ID}}:max`

* **例 (Example)**
    コントロールIDが `slider-control-ID` のスライダーコントロールで選択された最小値と最大値の間の特定の数量を販売した製品について `PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA` をフィルタリングするには、以下のサンプルSQLを使用します。
    ```sql
    SELECT *
    from EXAMPLES.PLUGS_ELECTRONICS.PLUGS_ELECTRONICS_HANDS_ON_LAB_DATA
    where QUANTITY between {{slider-control-ID}}:min and {{slider-control-ID}}:max
    ```

#### **SQLで日付範囲コントロールの値を参照する (Reference date range control values in SQL)**
SQLステートメントで、特定のコントロールで選択または指定された値を参照できます。日付の範囲を出力するコントロールの場合、構文は以下の通りです。

* **サポートされるコントロールタイプ**
    Date range

* **構文 (Syntax)**
    特定のデータプラットフォームがコントロールをどのように解釈するかによって、正確な構文は接続ごとに異なる場合があります。
    例えば、カスタムSQLで日付範囲コントロールの開始日を抽出する場合：
    * **Snowflake**では、コントロールは`VARIANT`データ型なので、以下の構文を使用できます。
      `to_timestamp({{Date-Range-Control}}:start)`
    * **BigQuery**または**Databricks**では、コントロールは`STRUCT`データ型なので、以下の構文を使用できます。
      `{{Date-Range-Control}}.start`
    * **Amazon Redshift**では、コントロールは`SUPER`データ型なので、以下の構文を使用できます。
      `select date_range.start start from (select {{Date-Range-Control}} date_range)`
    * **PostgreSQL**では、コントロールは`JSONB`データ型なので、以下の構文を使用できます。
      `({{Date-Range-Control}}->>‘start’)::timestamptz`

    範囲の終了日を参照するには、`start`の代わりに`end`を参照します。

* **特定の日付範囲コントロールの出力を返す**
    Snowflakeで、日付列が日付範囲コントロールで指定された値と一致する場合にのみ行を返すには、以下のサンプルSQLを参照してください。
    ```sql
    SELECT * FROM table
    WHERE
    CASE WHEN date({{Date-Range-Control}}:start) IS NULL
    THEN DATE <= date({{Date-Range-Control}}:end)
    WHEN date({{Date-Range-Control}}:end) IS NULL
    THEN DATE >= date({{Date-Range-Control}}:start)
    ELSE DATE BETWEEN date({{Date-Range-Control}}:start) AND date({{Date-Range-Control}}:end)
    END
    ```
    このSQLは、`DATE`列が`Date-Range-Control`で指定された値と一致するすべての行を返します。

#### **SQLで複数選択リストから複数の値を参照する (Reference multiple values from a multi-select list in SQL)**
SQLステートメントで、特定のコントロールで選択または指定された値を参照できます。複数選択リストの値は、配列として出力されます。例：
`('apples','bananas','oranges')`

コントロール値が単一引用符付きで出力される場合、コントロールIDの前にキーワード `#raw` を付けることで、これらの引用符を削除できます。
`{{#raw my-control-id}}`
> 🚧
> `#raw`構成値を使用すると、ワークブックまたはワークシートで行レベルのセキュリティがバイパスされ、セキュリティの脆弱性が生じる可能性があります。

* **サポートされるコントロールタイプ**
    List values, Legend

* **構文 (Syntax)**
    特定のクラウドデータウェアハウス（CDW）が配列データ型をどのように解釈するかによって、正確な構文は接続ごとに異なる場合があります。
    * **Snowflake**については、公式Snowflakeドキュメントの`Semi-structured data types`内の`Array`を参照してください。
    * **Databricks**については、公式Databricksドキュメントの`ARRAY type`を参照してください。
    * **BigQuery**については、公式Google Cloud BigQueryドキュメントの`Work with arrays`を参照してください。
    * **Amazon Redshift**については、公式Amazon Redshiftデータベース開発者ガイドの`SUPER type`を参照してください。

    例：
    ```sql
    select
      *
    FROM
      APPLICATIONS.GOOGLE_ANALYTICS.EVENTS
    WHERE
      TRAFFIC_SOURCE IN {{TRAFFIC_SOURCE}}
    limit
      10
    ```
    より詳細な例については、「[Return rows depending on the value of a multi-select control](#return-rows-depending-on-the-value-of-a-multi-select-control)」を参照してください。

* **複数選択コントロールの値に応じて行を返す**
    `City`という複数選択コントロールがあり、Snowflake接続でこのSQLを実行する場合、以下のサンプルクエリは`CITY`列の値が`City`コントロールの選択リストに含まれるすべての行を返します。`City`コントロールで都市が選択されていない場合、すべての行が返されます。
    ```sql
    SELECT * FROM EXAMPLES.BIKES.STATIONS  WHERE  
    CASE WHEN  
    LEN(ARRAY_TO_STRING(ARRAY_CONSTRUCT{{City}},',') ) = 0  
    THEN True  
    ELSE CITY in {{City}} END
    ```
    さらなる例については、Sigmaコミュニティの記事「[Injecting multi-select parameters in Custom SQL](https://community.sigmacomputing.com/c/technical-deep-dives/injecting-multi-select-parameters-in-custom-sql-287)」を参照してください。
### 4-7-3. dbt Semantic Layer連携のクエリ (ベータ版) (Query a dbt Semantic Layer integration (Beta))

> 🚩
> このドキュメントはプライベートベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このドキュメントは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。
> この機能の限定テストグループへの参加に興味がある場合は、[サポートに連絡](https://help.sigmacomputing.com/hc/en-us/requests/new)するか、アカウントエグゼクティブにお問い合わせください。

Sigmaは[dbt Semantic Layer](https://docs.getdbt.com/docs/use-dbt-semantic-layer/dbt-semantic-layer)連携をサポートしており、事前定義されたdbtメトリクスをSigmaワークブックで活用して、アドホック分析、定期レポート、組織のダッシュボードを作成できます。このドキュメントでは、Sigmaでdbt Semantic Layerにクエリを実行する方法と、そのクエリフローの進行について説明します。

#### **システムとユーザー要件 (System and user requirements)**

* **Sigmaにて:**
    * この機能を使用するには、[カスタムSQLを記述する権限](https://help.sigmacomputing.com/docs/account-type-and-license-overview)が有効になっているアカウントタイプを割り当てられている必要があります。
    * 接続全体に対する`Can use`の[データ権限](https://help.sigmacomputing.com/docs/data-permissions)を持っている必要があります。「[データ権限の管理](https://help.sigmacomputing.com/docs/data-permissions)」を参照してください。
    * 接続で[書き込みアクセスが構成されている](https://help.sigmacomputing.com/docs/set-up-write-access)必要があります。
    * [dbt Semantic Layer連携が構成されている](https://help.sigmacomputing.com/docs/configure-a-dbt-semantic-layer-integration)必要があります。
* **dbtにて:**
    * dbtでセマンティックモデルとメトリクスが作成されている必要があります。dbtドキュメントの「[dbt Semantic Layer](https://docs.getdbt.com/docs/use-dbt-semantic-layer/dbt-semantic-layer)」を参照してください。

#### **Sigmaとdbt Semantic Layer間のクエリフロー (Query flow between Sigma and dbt Semantic Layer)**
<img width="452" height="313" alt="a27389833b9750670592f46eac51e63765d927b79320c47a63199a2ce52d61c2-dbt_query_flow_diagram" src="https://github.com/user-attachments/assets/c3eb4970-7437-425a-94be-9600c803830d" />
SigmaでSemantic Layerクエリを入力すると、Sigmaはクエリを中間表現にコンパイルし、クエリパラメータをdbt Semantic Layer [JDBC API](https://docs.getdbt.com/docs/use-dbt-semantic-layer/jdbc)に送信します。dbtは適切な方言でSQLステートメントをSigmaに返します。次に、Sigmaは接続されたデータベースに対してそのSQLを実行し、他のデータプラットフォームからのテーブルと同様のテーブルを出力します。これらのテーブルは、Sigmaの他のデータテーブルと同様に使用できます。ワークブックやデータモデルで再利用したり、データセットを作成して結合したり、ビジュアライゼーションを構築したりすることができます。

Semantic Layerクエリが実行されるたびに、Sigmaは最新の定義を要求するため、Semantic Layerに加えられた変更はSigmaに反映されます。

#### **dbt Semantic Layer連携にクエリを実行する (Query the dbt Semantic Layer Integration)**
Semantic Layerにクエリを実行するには、以下を実行します。
1.  ワークブックを`Explore`または`Edit`モードで開きます。
2.  `Add element`を選択し、次に`Table`、そして`Custom SQL`を選択します。
3.  クエリを入力します。クエリ構文については、dbtのドキュメント「[Querying the API for metric metadata](https://docs.getdbt.com/docs/use-dbt-semantic-layer/query-sl)」を参照してください。
4.  `Run`を選択します。

Semantic Layerクエリが実行されるたびに、Sigmaは最新の定義を要求するため、Semantic Layerに加えられた変更はSigmaに反映されます。新しいクエリが実行されない限り、Semantic Layerに加えられた変更は反映されません。

#### **Semantic Layerメトリクスを参照する (Reference Semantic Layer metrics)**
dbt内のメトリック名を括弧内に入れて、`{semantic_layer.metrics()}`というテンプレート構文を使用することで、セマンティックレイヤーのメトリクスを参照できます。さらなる構文ガイダンスについては、dbtのドキュメント「[Querying the API for metric metadata](https://docs.getdbt.com/docs/use-dbt-semantic-layer/query-sl)」を参照してください。

##### **例1：Sigmaワークブックでdbtメトリクスを表示し、グループ化する**
既存のdbtメトリクスをSigmaワークブックで表示し、複数のディメンションでグループ化できます。クエリ例は次のようになります。
```sql
SELECT * FROM
{{ semantic_layer.query(
    metrics = ['new_customers', 'transactions', 'revenue_usd'],
    group_by = [Dimension('metric_time').grain('month'), 'customer__customer_country']
)}}
```
このクエリは、サンプルのdbtデータ内の3つの既存メトリクス（'new_customers', 'transactions', 'revenue_usd'）を表示し、国と時間（月の間隔で分割）の両方でグループ化します。このクエリはSigmaで以下の結果を生成します。
<img width="562" height="297" alt="a8345e9fb7b7134ee95f66525a54da606d1707b1c9e7d061700e82d32de380b8-surface_dbt_metrics" src="https://github.com/user-attachments/assets/1cc8d339-65ec-4f3e-9032-46a682daf5f8" />

##### **例2：Semantic Layerメトリクスを閲覧する (Example 2: Browse Semantic Layer metrics)**
以下のカスタムSQLを実行することで、SigmaのSemantic Layerで利用可能なすべてのメトリクスのリストを取得できます。
```sql
select * from {{semantic_layer.metrics()}}
```
これにより、メトリクス名と追加詳細のテーブルが生成されます。例：
<img width="778" height="211" alt="320cc755f31e9a207047214bdcfe9ebcf26819ccb5ef45792cf9c13201a808b3-browse_metrics" src="https://github.com/user-attachments/assets/1d9a650d-add0-4d02-8adf-a88941b2110f" />

##### **例3：メトリックのすべてのディメンションと時間粒度をリストする (Example 3: List all dimensions and time grains for a metric)**
既存のdbtメトリックで利用可能なすべてのディメンションと時間粒度のリストを取得したい場合があります。例えば、'transactions'という名前の既存のdbtメトリックがある場合、クエリは次のようになります。
```sql
select * from {{semantic_layer.dimensions(metrics=['transactions'])}}
```
このSQLをSigmaで実行すると、以下の結果が生成されます。<img width="1174" height="451" alt="feb028759048b649aa18d4ec990c4560057eba158b90cb02f19d9c418872a476-list_dimensions" src="https://github.com/user-attachments/assets/9ed1b1c2-49a2-4b4b-94db-4d88a77aeaec" />

#### **制限事項 (Limitations)**
[ワークブックコントロール](https://help.sigmacomputing.com/docs/intro-to-control-elements)は、Semantic Layerクエリで参照できません。ワークブックコントロールを参照するクエリは、エラーメッセージを結果として返します。

### 4-7-4. Ask Sigmaで自然言語クエリを実行する (Ask natural language queries with Ask Sigma)

Ask Sigmaは、データに関する質問をしたり、AIが生成した応答と対話したりできる自然言語クエリ（NLQ）インターフェースです。データから事実情報を抽出したり、チャートを生成する質問をしたりして、それをさらにワークブックで探索することができます。

> 🚩
> AI機能の使用は、以下の[免責事項](https://help.sigmacomputing.com/docs/ai-feature-disclaimer)の対象となります。

#### **システムとユーザー要件 (System and user requirements)**
Ask Sigmaを使用するには、以下が必要です。
* あなたの組織でAIプロバイダーが構成されている必要があります。「[Configure an AI provider](https://help.sigmacomputing.com/docs/configure-an-ai-provider)」を参照してください。
* `Use Ask Sigma`権限が有効になっているアカウントタイプを割り当てられている必要があります。詳細は「[Account type and license overview](https://help.sigmacomputing.com/docs/account-type-and-license-overview)」を参照してください。
* Ask Sigmaからワークブックに分析を移動するには、`Create, edit, and publish workbooks`権限が有効になっているアカウントタイプを割り当てられている必要があります。詳細は「[Account type and license overview](https://help.sigmacomputing.com/docs/account-type-and-license-overview)」を参照してください。

#### **制限事項 (Limitations)**
* Ask SigmaはJoin（結合）を実行できません。Ask Sigmaはデータに関する質問に答えるために単一のデータソースを選択し、複数のテーブル、データモデル、またはメトリクスからのデータを組み合わせることはできません。
* Ask Sigmaは、管理者がAIモデルで利用可能にしたデータプラットフォーム内のデータソースに基づいてのみ、データに関する質問に答えることができます。「[Select data sources to make available to Ask Sigma](https://help.sigmacomputing.com/docs/select-data-sources-to-make-available-to-ask-sigma-beta)」を参照してください。
* データモデルのタグ付けされたバージョンは、Ask Sigmaでは利用できません。
* Ask Sigmaを独自のポータルやサイトに埋め込みたい場合は、セキュアな埋め込みURLをJWTで署名する必要があります。「[Embed Ask Sigma (Beta)](https://help.sigmacomputing.com/docs/embed-ask-sigma)」を参照してください。

#### **データソースを検索する (Search data sources)**
Ask Sigmaは、管理者がAsk Sigmaで利用可能にすることを選択したデータソースにのみアクセスできます。あなたは、自分がアクセスできるデータソースを検索し、データカタログでどれが利用可能かを確認できます。

利用可能なデータソースを検索するには：
1.  Sigmaホームから、左のナビゲーションで`Ask Sigma`をクリックします。このオプションが表示されない場合は、上記の「[System and user requirements](#system-and-user-requirements)」を参照してください。
2.  `All data sources`をクリックし、テーブル、データモデル要素、またはデータセットの名前の全部または一部を入力して、それがAsk Sigmaで利用可能かどうかを確認します。
    Sigmaは、あなたが使用する権限を持つすべての一致するテーブル、データモデル要素、およびデータセットを返します。それぞれに、Ask Sigmaで利用可能かどうかのインジケータが表示されます。
    > 📘
    > あなたの管理者は、Ask Sigmaによってクエリされるソースを構成します。
    > Sigmaの他の場所で適用されるすべてのデータ権限は、Ask Sigmaでも適用されます。例えば、管理者がデータソースに行レベルのセキュリティまたは列レベルのセキュリティを構
    成している場合、Ask Sigmaはそれらの制限を尊重します。データモデルの場合、その要素が利用可能なソースとして表示されるためには、公開バージョンへのアクセス権が必要です。<img width="448" height="594" alt="04ef9e20359ae68209f680bfcf0d129fa92a47d7dbb7bea2c7224d16a3b28fa9-ask_sigma_highlighted_datasource" src="https://github.com/user-attachments/assets/63af48cc-8837-428a-b31f-49dd22b053c4" />

    Ask Sigmaで利用可能にしたいソースが現在利用できない場合は、Sigmaの管理者に通知してください。Sigmaの管理者は、Ask Sigmaで利用可能にするデータソースを選択します。「[Select data sources to make available to ask Sigma (Beta)](https://help.sigmacomputing.com/docs/select-data-sources-to-make-available-to-ask-sigma-beta)」を参照してください。

#### **Ask Sigmaで自然言語クエリを実行する (Ask natural language queries with Ask Sigma)**
Ask Sigmaを使用してデータに関する質問をするには：
1.  Sigmaホームから、左のナビゲーションで`Ask Sigma`をクリックします。
2.  画面の左上にあるボックスに質問を入力します。
3.  Ask Sigmaはあなたの質問を解釈し、あなたがアクセスできるデータソースを検索し、質問に答えるのに最適だと判断したソースを選択します。Ask Sigmaは、意味的関連性、データ有効性メタデータ、およびデータソースの使用状況を使用して、あなたが閲覧権限を持つデータソースの中から最適なデータソースを選択します。
4.  Ask Sigmaは回答を提供し、回答を決定するために使用したステップバイステップの決定ロジックを表示します。<img width="1704" height="881" alt="bb9a8365374dd9439e3a18d44020c4a1bccfd010cb45cc3a65f64440d3d0e2aa-answer-view" src="https://github.com/user-attachments/assets/1717442e-6823-4768-af88-69a877c18f62" />

5.  [任意] ステップをスクロールするか、サイドパネルで特定のステップを選択して決定ロジックを調査し、必要であればAsk Sigmaが行った選択を修正します。![15cc5b9bbf09d013dea95e85eee6d2fa751c2619a3dfc90330f5780d021cab61-scroll-back-through-steps](https://github.com/user-attachments/assets/25c8af66-7b20-4152-b37f-560854af40b5)

6.  [任意] 任意のステップで、`Open in workbook`をクリックして、分析のその時点から[探索（exploration）](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations)を開始します。

#### **関連チャートで探索を続ける (ベータ版) (Continue exploring with related charts (Beta))**
> 🚩
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このドキュメントは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

最初の回答から、提供された分析の探索を続けることができます。Ask Sigmaは、関連データを分析する道筋を提供するために、主要な回答の下に関連チャートを提示します。

あなたは以下のことができます。
* 回答チャートまたは任意の関連チャートの`View underlying data`をクリックする。
* 関連チャートをクリックして詳細ビューを表示し、さらに関連チャートを取得する。
* 任意のステップ、回答、または関連チャートのチェックボックスをオンにし、`Open in workbook`をクリックして、[探索](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations)でデータをさらに分析する。![5fe428f47a8e2725047e543272cd175e2684c893e7ce7fd6c26efe29ccd64aa7-keep-exploring](https://github.com/user-attachments/assets/68553c22-2bf7-43b5-a13b-9c59c713fd50)

#### **Ask Sigmaのトラブルシューティング (Troubleshoot Ask Sigma)**
失敗したAsk Sigmaクエリについて技術サポートに相談する必要がある場合は、Ask Sigmaの左下隅にある`Download debug`をクリックして、サポートチームに提供できるようにしてください。デバッグファイルには、あなたの質問のテキストとデータソースに関するメタデータが含まれており、Ask Sigmaがクエリを解決するために取ったステップのトラブルシューティングに役立ちます。

### 5-1-1. ワークブックとデータモデルのデータリネージを表示する (View workbook and data model data lineage)

データリネージ（系譜）とは、ワークブックまたはデータモデル内のデータ要素間の祖先と関係を指します。すべてのワークブックとデータモデルには**リネージグラフ**が含まれており、ドキュメント内の関係と依存関係を確認・操作することができます。

データリネージのユースケースには、以下のようなものがあります。
* データ要素への変更が子要素にどのように影響するかを判断する
* 予期しないデータのソースを特定する
* 未使用または冗長な要素を削除するために既存のワークブックをクリーンアップする
* データおよび/または権限エラーのソースを診断する
* マテリアライゼーションスケジュールの依存関係を特定する

このドキュメントでは、ワークブックまたはデータモデルのデータリネージを表示し、操作する方法について説明します。

#### **要件 (Requirements)**

データリネージを表示するには、ワークブックまたはデータモデルに対する`Can Edit`[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)が必要です。

#### **ワークブックまたはデータモデルのデータリネージを表示する (View data lineage for a workbook or data model)**

1.  ドキュメントヘッダーの`Edit`をクリックして、編集用にドキュメントを開きます。
2.  `(Lineage)`を選択して、ワークブックまたはデータモデルのデータリネージを開きます。
    > 💡
    > 特定の要素の要素ツールバーからリネージを開くこともできます。
    > 1.  要素ツールバーで、`More`を選択します。
    > 2.  メニューで、`View lineage`を選択します。
    > ドキュメントのデータリネージが、その要素がハイライトされた状態で開きます。

データリネージグラフでは、以下のいずれかを実行できます。
* `+`および`-`オプションを使用してズームインおよびズームアウトする。
* ブラウザウィンドウのビューにリネージグラフを合わせる。
* `Show controls`チェックボックスを選択して、コントロール要素を表示または非表示にする。
* カーソルで掴んでドラッグして、グラフ内を移動する。
* クリックしてドラッグすることで、グラフ内の要素を再編成する。要素の位置に加えた変更は、データリネージを閉じるとリセットされます。
* [特定の要素またはページにリネージビューをフォーカスする](#focus-your-lineage-view-on-a-specific-element-or-page)。
* [データリネージから要素を開く](#open-an-element-from-data-lineage)。

#### **特定の要素またはページにリネージビューをフォーカスする (Focus your lineage view on a specific element or page)**

* **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ドキュメントヘッダーの`Edit`をクリックします。

1.  `(Lineage)`を選択して、ワークブックまたはデータモデルのデータリネージを開きます。
2.  グラフの上部で、要素を検索するか、ドロップダウンメニューを開いてワークブックまたはデータモデル内の特定のページを選択します。
3.  メニューからページを選択すると、そのページの要素のみが表示されます。

#### **データリネージから要素を開く (Open an element from data lineage)**

* **始める前に:** このアクションは編集モードでのみ利用可能です。編集を開始するには、ドキュメントヘッダーの`Edit`をクリックします。

1.  `(Lineage)`を選択して、ワークブックまたはデータモデルのデータリネージを開きます。
2.  リネージグラフで要素を選択します。
3.  要素の詳細で、`View element`を選択します。

### 5-1-2. ワークブックまたは要素のデータソースを変更する (Change the data source for a workbook or element)

ワークブック全体または特定のデータ要素で使用されるデータソースを変更することができます。

例えば、実験や計算の作成中に本番データベースへの負荷を軽減するために、テストデータ接続からのデータソースでワークブックを構築することがあります。チームや組織とワークブックを公開・共有する準備ができたら、ワークブックで使用されているテストデータソースを本番データソースに置き換えることができます。

また、バージョンタグに基づいて、ワークブックやデータモデルのデータソースを自動的に変更または交換することもできます。「[Swap the source of a tagged version](https://help.sigmacomputing.com/docs/add-version-tags#swap-the-source-of-a-tagged-version)」を参照してください。

#### **要件 (Requirements)**
* 変更したい接続に対する`Can use`[アクセス権](https://help.sigmacomputing.com/docs/data-permissions)が付与されている必要があります。
* ワークブックに対する`Can edit`または`Can explore`のアクセス権が必要です。

#### **ワークブックのデータソースを交換する (Swap the data source for a workbook)**
ワークブック内のすべての要素のデータソースを交換するには（例えば、テストデータウェアハウス接続から本番データウェアハウス接続に変更するなど）、以下を実行します。

1.  ワークブックを`Edit`または`Explore`モードで開きます。
2.  ワークブックメニュー から、`Swap data sources…`を選択します。
3.  `Swap Data Sources Overview`モーダルで、自動選択された`Matching Connection`を確認します。必要に応じて、選択された接続を更新します。
4.  ワークブック内の各要素の`Matching Data Sources`を確認します。いずれかのデータソースに`No Match`がある場合は、`Match Manually`を選択して、一致するデータソースがない各要素に対して異なるデータソースを選択します。
5.  手動マッチページで、要素によって使用されるデータソースを選択し、`Select Source`をクリックします。
6.  新しいデータソースを検索または参照し、`Select`をクリックします。
7.  マッチングが必要な次のデータソースを選択し、これらのステップを繰り返します。
8.  一致しないすべてのデータソースが新しいデータソースにマッチングされた後、`Swap`を選択します。
9.  手動でマッチングする必要があるデータソースがない場合は、`Swap Now`を選択します。

ワークブックは新しいデータソースを使用するように更新されます。一致するデータソースがない要素はエラーを表示します。

> 🚩
> ワークブックに入力テーブルまたはカスタムSQL要素が含まれている場合、それらの要素のデータソースと接続は交換されません。代わりに、新しい接続をデータソースとして要素を再作成する必要があります。
> * **入力テーブルの場合、** 新しい接続で入力テーブルを作成し、古い入力テーブルから新しいものへデータをコピー＆ペーストします。
> * **カスタムSQL要素の場合、** 新しいSQL要素を作成し、新しいデータ接続に対して同等のSQLを記述します。

#### **要素のデータソースを変更する (Change the data source for an element)**
特定の要素に使用されるデータソースを変更することもできます。例えば、Snowflakeデータベースにビューを作成し、Sigmaのテーブル要素をSnowflake接続のベーステーブルの代わりにそのビューを使用するように更新したい場合、ソースを交換できます。

> 🚩
> 入力テーブルまたは接続されたデータウェアハウスを直接クエリするSQLを使用する要素のデータソースは変更できません。SQL要素のソースを変更すると、その要素はもはやSQLを使用しなくなります。

##### **要素のデータソースを交換する (Swap the data source for an element)**
`Edit`または`Explore`モードで要素を選択した後、データソースを変更できます。
1.  ワークブックキャンバスから、`More` > `Element source` > `Change source`を選択します。または、エディタパネルの`Properties`タブで、データソースの名前を探し、 > `Change source`を選択します。
2.  要素の新しいデータソースを検索または参照します。
3.  [任意] データソースをプレビューして特定の列を選択し、`Add`をクリックします。
4.  データソースを選択して、データソースの変更を完了します。

データ要素は更新されます。要素に新しいデータソースに存在しない列を参照する計算列が含まれている場合、その計算列は「unknown column」と表示されます。

##### **テーブル要素で使用されるテーブルを置き換える (Replace the table used by a table element)**
テーブルまたはピボットテーブル要素で使用されるテーブルを別のテーブルに置き換えたい場合は、以下を実行します。
1.  ワークブックキャンバスから、`More` > `Element source` > `Replace table`を選択します。または、エディタパネルの`Properties`タブで、データソースの名前を探し、 > `Replace table`を選択します。
2.  要素の新しいテーブルを検索または参照します。
3.  選択した列を確認し、任意で不要な列の隣にあるチェックボックスの選択を解除します。
4.  `Add`をクリックします。

データ要素は更新されます。テーブルに新しいテーブルに存在しない列を参照する計算列が含まれている場合、その計算列は「unknown column」と表示されます。

### 5-1-3. ワークブックの更新オプションを管理する (Manage workbook refresh options)

Sigmaは、個人がワークブックを開くか更新するたびに、ワークブックのデータを更新します。ユーザーの操作なしで画面に表示されるワークブックなど、設定されたスケジュールでワークブックのデータを更新したい場合は、カスタムの更新スケジュールを設定できます。

データ要素は個別に更新することもできますが、自動スケジュールでは更新できません。

> 🚩
> Sigmaはデータを保存しません。すべての更新は、ウェアハウス内のデータに再度クエリを実行します。自動更新を設定すると、接続に負荷がかかり、多額のウェアハウスコストが発生する可能性があります。

#### **要件 (Requirements)**

更新スケジュールを設定するには、個々のワークブックに対する`Can Edit`[アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)と、`Set workbook data refresh`権限が有効になっているアカウントタイプを割り当てられている必要があります。

ワークブックがホストアプリケーションに埋め込まれている場合、カスタム更新スケジュールを埋め込みコンテンツに適用するには、セキュアな埋め込みがJSON Web Tokens (JWTs)で認証されている必要があります。「[Create an embed API with JSON Web Tokens (Beta)](https://help.sigmacomputing.com/docs/example-embed-api-and-url#create-an-embed-api-with-json-web-tokens)」を参照してください。

#### **更新スケジュールを設定する (Set up a refresh schedule)**

ワークブックの更新スケジュールを設定するには、以下を実行します。
1.  ワークブックヘッダーの更新ボタンの右側にあるキャレット() `More options`をクリックします。
2.  `Data refresh`を選択します。
3.  `Data refresh settings`モーダルが開きます。
4.  `Refresh schedule`で、`Enable`トグルをオンにします。
5.  `Query data every`フィールドを調整して、ワークブックを更新する頻度を指定します。例えば、10分ごとなど。
6.  [任意] 更新スケジュールを特定の時間枠に制限するには、`Between`フィールドに時間を入力します。Sigmaは、更新スケジュールが有効であるべきかを評価するために、ブラウザのタイムゾーンを使用します。
7.  `Save`をクリックします。

#### **個々のデータ要素を更新する (Refresh individual data elements)**

個々のデータ要素のデータを手動で更新できます。
1.  データ要素を選択します。
2.  要素のツールバーで、`More`をクリックします。
3.  `Refresh data`をクリックします。
4.  要素内のデータが更新されます。

### 5-1-4. ワークブックのローカライゼーションを管理する (Manage workbook localization)

ローカライゼーションにより、ワークブックの編集者はカスタムワークブックのテキストを他の言語に翻訳できます。翻訳はワークブックのプレビューと埋め込みビューに適用されます。

管理者は、Sigma組織内のすべてのワークブックに適用される組織レベルの翻訳を作成することもできます。管理者によって管理される組織レベルの翻訳ファイルの詳細については、「[組織の翻訳ファイルを管理する](https://help.sigmacomputing.com/docs/manage-organization-translation-files)」を参照してください。

#### **要件 (Requirements)**
ワークブックの翻訳を管理するには、`Can edit`の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)が付与されている必要があります。
> 📘
> ワークブックのプレビューまたは埋め込みビューのURLと有効なロケール定義を持つ任意のユーザーが、翻訳されたワークブックを閲覧できます。

#### **サポートされている言語とロケール (Supported languages and locales)**
Sigmaは以下の言語とロケールをサポートしています。
| 言語 | ロケール |
| :--- | :--- |
| Chinese (Simplified) | zh-cn |
| Chinese (Traditional) | zh-tw |
| English (United States) | en |
| English (Australia) | en-au |
| English (Canada) | en-ca |
| English (Ireland) | en-ie |
| English (United Kingdom) | en-gb |
| French | fr |
| French (Canada) | fr-ca |
| German | de |
| Italian | it |
| Japanese | ja |
| Korean | ko-kr |
| Polish | pl |
| Portuguese | pt |
| Portuguese (Brazil) | pt-br |
| Russian | ru |
| Spanish | es |
| Spanish (Mexico) | es-mx |
| Swedish | sv-se |
| Thai | th |

#### **ワークブックの翻訳を作成する (Create a workbook translation)**
ワークブックの設定メニューからアクセスできる`Manage locales`パネルを使用して、ワークブックのロケールと翻訳を管理します。

1.  ワークブックを`Edit`モードで開きます。
2.  ワークブックの左サイドバーにある設定アイコン()をクリックして、ワークブックの設定パネルを開きます。
3.  `Manage locales`をクリックします。
4.  新しい言語を追加するには、`Available locales`の隣にあるプラスアイコン(+)をクリックします。
5.  ドロップダウンメニューから言語を選択します。
    > 📘
    > このステップを完了してワークブックのロケールを作成すると、すべての標準Sigmaテキスト（メニューラベル、モーダルテキストなど）の翻訳が有効になります。ワークブックのカスタムテキストを翻訳するには、この手順の残りを完了してください。
6.  ワークブック内のカスタムテキストの翻訳を追加するには、その他アイコン()をクリックし、jsonファイルをダウンロードします。

| オプション | 内容 | いつ使うか |
| :--- | :--- | :--- |
| **Download** | このオプションは、組織レベルの翻訳ファイルが存在しない場合に表示されます。結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。 | 管理者が組織全体に適用される翻訳を定義していない場合に、カスタムテキストの翻訳を定義するためにこのオプションを選択します。 |
| **Download untranslated strings** | 結果のjsonファイルには、組織レベルの翻訳ファイルのキーと一致しない、ワークブック内のカスタム文字列のキーと値のペアのみが含まれます。 | 組織レベルで定義されている値を上書きしたくない場合に、このオプションを選択します。 |
| **Download all strings** | 結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。 | このワークブックのカスタム文字列に適用されるすべての翻訳を確認したい場合、または組織レベルの翻訳をこのワークブック用に異なる翻訳で上書きしたい場合に、このオプションを選択します。|

7.  ダウンロードしたファイルを開きます。
8.  `.json`ファイルには、キーと値のペアのリストが含まれています。
    値を適切な翻訳に更新します。
    > 🚩
    > どのキーも編集しないでください。
9. ファイルを編集して保存します。ファイル名は変更しないでください。
10. Sigmaに戻ります。`Upload`をクリックし、更新した`.json`ファイルを選択します。
11. プレビューアイコン()をクリックして、翻訳されたテキストでワークブックのプレビューを開きます。

#### **ワークブックの翻訳を更新する (Update a workbook translation)**
#### **ワークブックの翻訳を更新する (Update a workbook translation)**
ワークブックにテキストの変更を公開するたびに、新しいまたは変更されたテキスト文字列の新しい翻訳を含むロケールの`.json`ファイルをダウンロードして再アップロードする必要があります。新しく追加された文字列は、jsonファイルの末尾に表示されます。

管理者がその言語の組織全体の翻訳ファイルを作成している場合は、未翻訳の文字列のみをダウンロードするか、すべての文字列をダウンロードするかを選択する必要があります。

| オプション | 内容 | いつ使うか |
| :--- | :--- | :--- |
| **Download (ダウンロード)** | このオプションは、組織レベルの翻訳ファイルが存在しない場合に表示されます。結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。 | 管理者が組織全体に適用される翻訳を定義していない場合に、カスタムテキストの翻訳を定義するためにこのオプションを選択します。 |
| **Download untranslated strings (未翻訳の文字列をダウンロード)** | 結果のjsonファイルには、組織レベルの翻訳ファイルのキーと一致しない、ワークブック内のカスタム文字列のキーと値のペアのみが含まれます。言い換えれば、組織レベルで翻訳が既に存在する場合、そのキーと値のペアはこのファイルでは省略されます。組織レベルのファイルで翻訳されていないキーは、このワークブックで定義された翻訳（もしあれば）を表示するか、まだ翻訳が提供されていない場合は英語の値を表示します。 | 組織レベルで定義されている値を上書きしたくない場合に、このオプションを選択します。 |
| **Download all strings (すべての文字列をダウンロード)** | 結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。組織レベルのファイルでのみ翻訳されているキーは、管理者がそのファイルで定義した値を表示します。組織レベルのファイルで翻訳されていないキーは、このワークブックで定義された翻訳（もしあれば）を表示するか、まだ翻訳が提供されていない場合は英語の値を表示します。組織レベルのファイルとワークブックレベルのファイルの両方で翻訳されているキーは、このワークブックで定義された翻訳を表示します。 | このワークブックのカスタム文字列に適用されるすべての翻訳を確認したい場合、または組織レベルの翻訳をこのワークブック用に異なる翻訳で上書きしたい場合に、このオプションを選択します。|

#### **言語のカスタム翻訳を追加する (Add a custom translation for a language)**

特定の言語に対して複数のユニークな翻訳を維持することができます。言語のカスタム翻訳を追加すると、例えば、埋め込みダッシュボードの異なる消費者に対して、ワークブック内の文字列を異なる方法で翻訳できます。

言語のカスタム翻訳を追加すると、カスタム翻訳ファイルがベース言語ファイルの**代わり**に使用されます。ベース言語ファイルに加えてカスタムの翻訳セットを適用するには、ベース言語ファイルをカスタム言語ファイルに複製してください。

1.  ワークブックを`Edit`モードで開きます。
2.  ワークブックの左サイドバーにある設定アイコン()をクリックして、ワークブックの設定パネルを開きます。
3.  `Manage locales`をクリックします。
4.  `Available locales`の隣にあるプラスアイコン(+)をクリックします。
5.  ドロップダウンメニューで、`Add custom translations`を選択します。
6.  カスタム翻訳ファイルの名前を入力します。
    > 🚩
    > 管理者が定義した組織レベルのカスタム翻訳セットをこの言語で継承したい場合は、ここで管理者が組織レベルの翻訳ファイルを作成した際に使用したのと同じ名前を使用する必要があります。管理者にファイルの名前を尋ねてください。
7.  `Base language`を設定して、すべての標準Sigmaテキスト（メニューラベル、モーダルテキストなど）に使用する言語を指定します。
8.  `Add`をクリックします。
9.  利用可能なロケールのリストで、追加したカスタム言語バリアントを見つけます。
    > 📘
    > 組織レベルの言語バリアントが存在し、カスタム言語バリアントファイルに同じ名前を使用した場合、組織レベルのファイルはグレーで表示されます。
10. ワークブック内のカスタムテキストの翻訳を追加するには、その他アイコン()をクリックし、jsonファイルをダウンロードします。

| オプション | 内容 | いつ使うか |
| :--- | :--- | :--- |
| **Download (ダウンロード)** | このオプションは、組織レベルの翻訳ファイルが存在しない場合に表示されます。結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。 | 管理者が組織全体に適用される翻訳を定義していない場合に、カスタムテキストの翻訳を定義するためにこのオプションを選択します。 |
| **Download untranslated strings (未翻訳の文字列をダウンロード)** | 結果のjsonファイルには、組織レベルの翻訳ファイルのキーと一致しない、ワークブック内のカスタム文字列のキーと値のペアのみが含まれます。 | 組織レベルで定義されている値を上書きしたくない場合に、このオプションを選択します。 |
| **Download all strings (すべての文字列をダウンロード)** | 結果のjsonファイルには、ワークブック内のカスタム文字列のすべてのキーと値のペアが含まれます。組織レベルのファイルでのみ翻訳されているキーは、管理者がそのファイルで定義した値を表示します。このワークブックレベルのファイルで翻訳されているキーは、このワークブックで既に定義されている翻訳（もしあれば）を表示するか、まだ翻訳が提供されていない場合は英語の値を表示します。組織レベルのファイルとワークブックレベルのファイルの両方で翻訳されているキーは、このワークブックで定義された翻訳を表示します。 | このワークブックのカスタム文字列に適用されるすべての翻訳を確認したい場合、または組織レベルの翻訳をこのワークブック用に異なる翻訳で上書きしたい場合に、このオプションを選択します。|

11. ダウンロードしたファイルを開きます。
12. `.json`ファイルには、キーと値のペアのリストが含まれています。
13. 値を適切な翻訳に更新します。
    > 🚩
    > どのキーも編集しないでください。
14. ファイルを編集して保存します。ファイル名は変更しないでください。
15. Sigmaに戻ります。`Upload`をクリックし、更新した`.json`ファイルを選択します。
16. プレビューアイコン()をクリックして、翻訳されたテキストでワークブックのプレビューを開きます。

カスタム翻訳は、管理者によって作成された組織レベルのファイルから継承できます。「[組織の翻訳ファイルを管理する](https://help.sigmacomputing.com/docs/manage-organization-translation-files)」を参照してください。

#### **翻訳ファイルでマークダウンと動的テキストを使用する (Use markdown and dynamic text in a translation file)**

JSONの値にマークダウンと動的テキストを使用して、リッチテキストをサポートできます。

値の一部として動的テキストを生成するには、以下の構文を使用します。 `[={formula-id}]`

他のリッチテキストにはマークダウン構文を使用します。

| 表示 | マークダウンバージョン |
| :--- | :--- |
| I love **bold** text. | `I love **bold** text.` |
| *Italics* are great too. | `*Italics* are great too.` |
| Click this [link](https://help.sigmacomputing.com). | `Click this [link](https://help.sigmacomputing.com).` |
| * Bullet points<br>* Make bulleted lists | `* Bullet points`<br>`* Make bulleted lists` |
| 1. Numbers<br>2. Make numbered lists | `1. Numbers`<br>`2. Make numbered lists` |

#### **埋め込みまたはプレビューにロケールと翻訳を適用する (Apply locales and translations to embeds or previews)**
埋め込みまたはプレビューにロケールを適用するには、埋め込みまたはワークブックプレビューのURLに `:lng=<your-locale>` を追加します。ロケールを適用すると、メニューラベルやモーダルテキストなどの標準Sigmaテキストが、ロケールに関連付けられた言語に翻訳されます。そのロケールに翻訳ファイルが定義されている場合、ロケールを適用すると、ワークブック内のカスタムテキストも定義された翻訳で翻訳されます。
言語のカスタム翻訳バリアントを適用する場合は、`:lng_variant=<variant+name>` も追加します。名前の特殊文字にはURLエンコーディングを使用してください。

* **埋め込みAPIコードの例:**
    ```javascript
    // 注：ローカライゼーションの値は大文字と小文字を区別します
    searchParams += '&:lng=fr-ca';
    ```
* **カスタム翻訳バリアントの埋め込みAPIコードの例:**
    ```javascript
    // 注：ローカライゼーションの値は大文字と小文字を区別します
    searchParams += '&:lng=it&:lng_variant=Custom+Italian';
    ```
* **埋め込みURLの例:**
    `https://app.sigmacomputing.com/my-company/workbook/My-Workbook-2PG8oM9uFxNLyzxAukJfBrL?:embed=true&:lng=fr-ca`
* **カスタム翻訳バリアントの埋め込みURLの例:**
    `https://app.sigmacomputing.com/my-company/workbook/My-Workbook-2PG8oM9uFxNLyzxAukJfBrL?:embed=true&:lng=it&:lng_variant=Custom+Italian`
> 💡
> ロケールを適用するために翻訳ファイルは必須ではありません。
> 翻訳ファイルが定義されていなくても、上記のパラメータを使用して埋め込みやプレビューにロケールを適用し、メニューラベルやモーダルテキストなどの標準Sigmaテキストを別の言語で表示することができます。

#### **現在の制限事項 (Current limitations)**
* 自動生成されたデータ要素名（例：Sum of Cost by Year of Date）は、Sigmaが生成する.jsonファイルには含まれません。翻訳を定義する前に、すべてのデータ要素を手動で命名してください。
* 探索モードはサポートされていません。
* 数値と日付のフォーマットはサポートされていません。

### 5-1-5. ワークブックのページの可視性を管理する (Manage workbook page visibility)

デフォルトでは、ワークブックのページは、ワークブックを閲覧、探索、または編集する権限を持つすべてのユーザーに表示されます。個々のページの可視性を変更して、特定のワークブックのコンテンツの閲覧を制限することができます。

このドキュメントでは、Sigmaのページの可視性オプションについて説明し、特定のページの可視性をカスタマイズする方法を解説します。

#### **ユーザー要件 (User requirements)**
ワークブックのページの可視性を管理する機能には、以下が必要です。
* `Create, edit, and publish workbooks`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがワークブックの所有者であるか、`Can edit`の[ワークブック権限](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

#### **ページの可視性を理解する (Understanding page visibility)**
ページの可視性はセキュリティ機能ではありません。データへのアクセスを制限する必要がある場合は、「[Dataset Row-Level Security](https://help.sigmacomputing.com/docs/set-up-row-level-security)」を参照してください。
> 📘
> ワークブック内の少なくとも1つのページには、ページの可視性制限が適用されていない状態である必要があります。
> 🚧
> ページの可視性設定は、`View`および`Explore`モードでのみ適用されます。ワークブックの所有者および特定のワークブックに対する`Can edit`権限を付与された任意のユーザーは、ページの可視性設定に関わらず、`Edit`モードですべてのページにアクセスできます。
> 🚧
> `Save As`権限を持つユーザーがワークブックのコピーを保存すると、元のワークブックのページの可視性設定に関わらず、コピーにはすべてのページが表示されます。

##### **ページの可視性アイコン (Page visibility icons)**
ページタブには、現在のページの可視性設定を示すアイコンが表示されます。

| アイコン | 説明 |
| :--- | :--- |
| (アイコンなし) | ページがすべてのユーザーに表示されることを示します。|
| (アイコン) | ページが選択されたユーザーまたはチームにのみ表示されることを示します。|
| (アイコン) | ページがすべてのユーザーから非表示になっていることを示します。|

##### **ワークブックのバージョンとセキュアな埋め込みでのページの可視性 (Page visibility in workbook versions and secure embeds)**
* **タグ付きバージョン (Tagged versions)**
    タグ付きのワークブックバージョンは、タグが適用されたときにワークブックに保存されたページの可視性設定を継承します。したがって、あるバージョンではユーザーがページにアクセスでき、別のバージョンでは同じユーザーから非表示にすることができます。
* **セキュアな埋め込み (Secure embeds)**
    セキュアな埋め込みでのページの可視性は、チーム設定によって決定されます。ページは、ユーザーの割り当てられたチームに表示されている場合（`Show page to all users`または`Only show to select users or teams`を介して）にのみ、埋め込みユーザーに表示されます。
    > 🚧
    > セキュアな埋め込みユーザーが埋め込まれたワークブックのコピーを保存すると、元のワークブックのページの可視性設定に関わらず、コピーにはすべてのページが表示されます。

#### **ページを非表示または再表示する (Hide or unhide a page)**
`Hide page`および`Unhide page`オプションを使用して、すべてのユーザーに対するページの可視性を迅速に更新します。
1.  ワークブックを`Edit`モードで開きます。
2.  カスタマイズしたいページのタブを探します。
3.  タブのキャレット()をクリックしてページメニューを開き、利用可能なオプションを選択します。
    * **Hide page:** `View`または`Explore`モードでワークブックにアクセスするすべてのユーザーからページを非表示にします。ページが現在すべてのユーザーに表示されている場合に利用可能です。
    * **Unhide page:** 任意のモードでワークブックにアクセスするすべてのユーザーにページを表示します。ページが現在すべてまたは選択されたユーザーとチームから非表示になっている場合に利用可能です。

#### **ページの可視性をカスタマイズする (Customize page visibility)**
`Customize page visibility`オプションを使用して、すべてのユーザーまたは特定のユーザーとチームに対するページの可視性を更新します。
1.  ワークブックを`Edit`モードで開きます。
2.  カスタマイズしたいページのタブを探します。
3.  タブのキャレット()をクリックしてページメニューを開き、`Customize page visibility`を選択します。
4.  `Customize Page Visibility`モーダルで、ページの可視性を構成します。
    a. `Page visibility setting`フィールドをクリックし、ドロップダウンからオプションを選択します。
        * **Hide page from all users:** `View`または`Explore`モードでワークブックにアクセスするすべてのユーザーからページを非表示にします。
        * **Show page to all users (default):** 任意のモードでワークブックにアクセスするすべてのユーザーにページを表示します。
        * **Only show to select users or teams:** 選択されたユーザーとチームにのみページを表示します。`View`または`Explore`モードでワークブックにアクセスする残りのユーザーからはページを非表示にします。
    b. ステップ4aで`Only show to select users or teams`を選択した場合は、`Select users`フィールドを使用して、該当するユーザーとチームを検索して選択します。
    c. `Save`をクリックして、ページの可視性の変更を適用します。

### 5-1-6. ドキュメントにショートカットを追加する (Add shortcuts to documents)

複数の場所にドキュメントへのリンクを保存したい場合は、ショートカットを追加できます。

ショートカットを使用して、特定のデータソースをソースピッカーで見つけやすくしたり、主要なワークブックやデータモデルへのアクセスを容易にするためにドキュメントを整理したりします。

例えば、「Sales」ワークスペースにある「Quarterly Sales Targets」ワークブックへのショートカットを、個人の「My Documents」フォルダに追加して、そのワークブックに簡単にアクセスできるようにすることができます。

別の例として、「Marketing」ワークスペースに「Google Analytics」データモデル（またはデータウェアハウステーブル）へのショートカットを追加できます。次にMarketingワークスペースの誰かがワークブックに新しい要素を追加しようとするとき、その標準的なデータモデルが簡単に見つかります。

#### **サポートされているショートカットドキュメント (Supported shortcut documents)**
以下のファイル、フォルダ、その他のオブジェクトへのリンクを、Sigmaのワークスペースまたはフォルダにショートカットとして保存できます。
* ワークブック
* フォルダ（「My Documents」を除く）
* ワークスペース
* データモデル（データモデル内の可視要素を含む）
* データセット
* データウェアハウスのテーブル、ビュー、スキーマ、カタログ、データベース

ショートカットへのショートカットを追加することはできず、「My Documents」フォルダへのショートカットを別のフォルダやワークスペースに追加することもできません。

#### **ショートカットの権限 (Shortcut permissions)**
ドキュメントにショートカットを追加するには、あなたが所有者であるか、そのドキュメントに対する`Can Explore`または`Can Edit`の権限を持っている必要があります。

ワークブック、フォルダ、ワークスペース、データモデル、またはデータセットへのショートカットを作成しても、そのファイルやフォルダへの権限は変更されません。フォルダやワークスペースへのアクセス権を持つ誰もがショートカットを閲覧できますが、ドキュメント（ワークスペース、ワークブック、フォルダ、データモデル、データセット）へのアクセス権を付与されたユーザーのみが、そのドキュメントを開くことができます。

#### **ドキュメントにショートカットを追加する (Add a shortcut to a document)**
サポートされているドキュメントへのショートカットを、別のフォルダまたはワークスペースに追加できます。バージョンタグが付いたワークブック、データモデル、またはデータセットにショートカットを追加することはできません。

1.  ショートカットを追加したいドキュメントを含む親フォルダまたはワークスペースを開きます。例えば、「My Documents」フォルダ内のサブフォルダへのショートカットを追加するには、「My Documents」を開きます。
2.  `More` > `Add shortcut…`を選択します。
3.  ショートカットを追加したいフォルダまたはワークスペースを検索または参照し、`Add`をクリックします。
4.  ドキュメントへのショートカットが、そのフォルダまたはワークスペースで利用可能になります。

ワークブック、データモデル、またはデータセットを表示中にショートカットを追加することもできます。
1.  ヘッダーで、ワークブック、データモデル、またはデータセットのタイトルの隣にある下矢印()を選択して、ドキュメントメニューを開きます。
2.  `File` > `Add shortcut…`を選択します。
3.  ショートカットを追加したいフォルダまたはワークスペースを検索または参照し、`Add`をクリックします。
    ワークブックへのショートカットが、そのフォルダまたはワークスペースで利用可能になります。

#### **データウェアハウスオブジェクトにショートカットを追加する (Add a shortcut to a data warehouse object)**
データウェアハウス内のテーブル、ビュー、スキーマ、カタログ、またはデータベースにショートカットを追加するには：
1.  Sigmaホームから、`Connections`を選択します。
2.  接続を選択し、ショートカットを追加したいオブジェクトを検索または参照します。
3.  オブジェクトにカーソルを合わせ、`More` > `Add shortcut…`を選択します。
4.  ショートカットを追加したいフォルダまたはワークスペースを検索または参照し、`Add`をクリックします。
5.  オブジェクトへのショートカットが、そのフォルダまたはワークスペースで利用可能になります。

その後、データソースを追加する際に、そのショートカットを使用してデータベースオブジェクトをより簡単に見つけることができます。

削除されたドキュメントへのショートカットがある場合、そのショートカットを削除するように促されます。ショートカットをクリックすると、もしアクセス権があれば、削除されたドキュメントを復元するように促されます。

### 5-2-1. テンプレートからワークブックを作成する (Create workbooks from templates)

テンプレートは、迅速かつ一貫性をもって新しいワークブックを構築できる、再利用可能なワークブック構造です。

このドキュメントでは、既存のテンプレートにアクセスし、それらを使用して新しいワークブックを作成する方法について説明します。テンプレートに関する詳細は、「[テンプレートの作成と編集](https://help.sigmacomputing.com/docs/create-and-edit-templates)」および「[テンプレートの共有](https://help.sigmacomputing.com/docs/share-templates)」を参照してください。

#### **要件 (Requirements)**

既存のテンプレートにアクセスし、それを使用して新しいワークブックを作成する機能には、以下が必要です。
* `Can create, edit, and publish workbooks`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたの組織のユーザーによって作成されたテンプレート（`Templates` > `Internal`内）にアクセスするには、あなたがテンプレートの所有者であるか、`Can use`または`Can edit`のテンプレート権限を付与されている必要があります。
* Sigmaテンプレートやあなたの組織と共有されている他のテンプレート（`Templates` > `External`内）にアクセスするには、`Internal`メンバータイプを割り当てられている必要があります。ゲストユーザーは外部テンプレートにアクセスできません。

#### **テンプレートからワークブックを作成する (Create a workbook from a template)**

1.  ホームページの左側ナビゲーションパネルから`Templates`ギャラリーページを開きます。
2.  探索したいテンプレートをクリックします。
3.  テンプレート化されたワークブックが開きます。
4.  テーブル、ビジュアライゼーション、コントロールなど、そのインタラクティブな要素のいずれかをクリックしてテンプレートを探索します。あなたの変更は、テンプレート自体には影響しません。
5.  [任意] テンプレートから編集可能で公開可能なワークブックを作成するには、テンプレートのヘッダーで`Save As`をクリックします。

#### **ワークブックテンプレートであなたのデータを使用する（ソースを交換する）(Use your data in a workbook template (swap sources))**

* **前提条件:** 交換したいデータはSigmaで利用可能である必要があります。

ワークブックテンプレートに独自のデータを注入するには：
1.  ホームページの左側ナビゲーションパネルから`Templates`ギャラリーページを開きます。
2.  使用したいテンプレートをクリックします。
3.  テンプレート化されたワークブックが開きます。
4.  ワークブックが[サンプルデータ](https://help.sigmacomputing.com/docs/sample-connection)上に構築されている場合、ページ上部にポップアップが表示されます。
5.  `Swap now`をクリックします。
6.  これにより、`Swap Data Sources`ページが開きます。
7.  Sigmaは、テンプレートの期待されるデータとあなたのデータを自動的に照合しようと試みます。
8.  しかし、これを上書きすることも、Sigmaが見つけられないソースを手動で選択する必要がある場合もあります。
    * [任意] 一致したソースを置き換えるには、`REPLACE WITH`の下にあるソースの隣の編集()ボタンをクリックします。次に、モーダルから新しいソースを選択します。
9.  テンプレートが追加のソースを必要とする場合は、左端のパネル`ALL SOURCES IN USE`から各ソースの一致を確認します。
10. 準備ができたら、`Swap`をクリックします。
11. ワークブックを探索して、あなたのデータが正しく表示されることを確認します。
12. テンプレートから編集可能で公開可能なワークブックを作成するには、テンプレートのヘッダーで`Save As`をクリックします。

ワークブックはソースの交換もサポートしています。ワークブックにデータを交換し始めるには、ワークブックを編集モードで開き、ヘッダーメニューを開いて`Swap data sources`をクリックします。

### 5-2-2. ワークブックテンプレートの作成と編集 (Create and edit workbook templates)

ワークブック[テンプレート](https://help.sigmacomputing.com/docs/get-started-with-workbook-templates)を使用すると、ユーザーは[ワークブック](https://help.sigmacomputing.com/docs/workbooks-overview)の構造をテンプレート化して共有し、迅速かつ一貫性のある再利用が可能になります。

#### **要件 (Requirements)**

テンプレートを作成および編集する機能には、以下が必要です。
* 既存のワークブックから新しいテンプレートを作成するには、`Create, edit, and publish workbooks`権限を持つ[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられ、既存のワークブックに対する表示アクセス権を持っている必要があります。
* 既存のテンプレートを編集するには、あなたがテンプレートの所有者であるか、`Can edit`のテンプレート権限を付与されている必要があります。

#### **新しいテンプレートを作成する (Create a new template)**

1.  テンプレートの基として使用したいワークブックを開きます。
2.  ドキュメントメニューから、`File` > `Save as template`を選択します。
3.  `Template Name`を入力します。
4.  [任意] テンプレートを共有したい場合は、組織のメンバーまたはチームの名前を入力し、ドロップダウンから希望の権限を選択します。
5.  `Save`をクリックします。新しいテンプレートにリダイレクトされます。

#### **既存のテンプレートを編集する (Edit an existing template)**

1.  ホームページから`Templates`を選択します。
2.  編集したいテンプレートを見つけ、`More` > `Open`を選択します。
3.  テンプレートのヘッダーで、`Edit`を選択します。
4.  変更を加えます。
5.  テンプレートのヘッダーで、`Publish`をクリックして変更を保存します。

### 5-3. ワークブックのライフサイクル

#### 5-3-1. ワークブックのライフサイクル：探索、ドラフト、公開 (Workbook lifecycle: explore, draft, and publish)

ワークブックは、アドホックなデータ探索と複雑な長期レポーティングの両方をサポートします。共同作業が可能なインターフェースと、データ操作への視覚的なアプローチにより、組織内の誰もがライブデータとリアルタイムの共同作業にアクセスできるようになります。この記事では、データ探索から公開、バージョン履歴までの、ワークブックのライフサイクルの基本を紹介します。

##### **アドホックなデータ探索 (Ad hoc data exploration)**
新規の、保存されていないワークブックは「探索（explorations）」とも呼ばれます。探索は、将来の使用のために作業を保存することなく、データを探索して次に進みたい場合のアドホック分析に最適です。
探索を公開済みワークブックとして保存するには、探索のヘッダーにある`Save as`をクリックします。
「[Ad hoc data exploration](https://help.sigmacomputing.com/docs/ad-hoc-data-explorations)」を参照してください。

##### **ワークブックのモード：編集、探索、表示 (Workbook modes: Edit, Explore, and View)**
公開済みのワークブックは、編集、探索、表示の3つの異なるモードでアクセスできます。特定のワークブックでアクセスできるモードは、その個々のワークブックに対してあなたに付与された権限に依存します。「[Workbook modes overview](https://help.sigmacomputing.com/docs/workbook-modes-overview)」を参照してください。

##### **ドラフトと公開 (Drafts and publishing)**
ワークブックに加えられた編集は、共有されたライブドラフトとして自動的に保存されます。複数の編集者が単一のドラフトでリアルタイムに共同作業できます。すべてのアクティブな編集者は、現在編集モードにいる他のユーザーのリストと、それぞれが選択している要素を見ることができます。
`Publish`をクリックすると、ライブドラフト上のすべての編集者によってドラフトされた変更を含む、ワークブックへのすべてのドラフトされた変更が公開されます。
「[Edit, draft, and publish a workbook](https://help.sigmacomputing.com/docs/draft-and-publish-a-workbook)」を参照してください。

##### **バージョン履歴 (Version history)**
Sigmaは、公開されたワークブックのバージョンとそれに関連する変更の履歴を保存します。これをバージョン履歴と呼びます。バージョン履歴には、ワークブックヘッダーにあるバージョンメニューからアクセスします。
「[Workbook versions and version history](https://help.sigmacomputing.com/docs/document-versions-and-version-history)」を参照してください。

### 5-3-2. ドキュメントバッジの表示と管理 (View and manage document badges)

ワークブックとデータモデルに認定バッジ（推奨、警告、非推奨）を設定して、ドキュメントのステータス、品質、信頼性を反映させます。

例えば、以下のようにデータモデルのライフサイクルの段階を示すためにバッジを使用します。
* **Endorsed (推奨):** データモデルは検証済みで信頼でき、品質基準を満たしています。
* **Warning (警告):** データモデルは古い、不完全、またはレビュー中です。
* **Deprecated (非推奨):** データモデルは廃止されたか、もはやメンテナンスされていません。

このドキュメントでは、ワークブックとデータモデルでバッジを表示、設定、削除する方法について説明します。データセットとデータベーステーブルに認定バッジを追加する方法については、「[データセットの作成と管理](https://help.sigmacomputing.com/docs/create-and-manage-datasets)」および「[データカタログのレビューと管理](https://help.sigmacomputing.com/docs/review-and-manage-your-data-catalog)」を参照してください。

#### **ユーザー要件 (User requirements)**
バッジを設定または削除する機能には、以下が必要です。
* `Manage all badges`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたがドキュメントの所有者であるか、任意の[ドキュメント権限](https://help.sigmacomputing.com/docs/folder-and-document-permissions)を付与されている必要があります。

バッジは、ドキュメントへのアクセス権を付与された任意のユーザーに表示されます。

#### **既存のバッジを表示する (View existing badges)**
ホームページから、または個々のワークブックからバッジを表示できます。
* **ホームページ:** ホームページから、`My documents`を選択します。最近アクセスしたドキュメントのうち、どのドキュメントにバッジが割り当てられているかを確認できます。
* **ワークブック内:** バッジはドキュメントメニュー（ワークブックの名前の隣）に表示されます。

#### **バッジを設定する (Set a badge)**
1.  バッジを割り当てたいドキュメントを開きます。
2.  ヘッダーで、ドキュメント名をクリックし、メニューから`File` > `Set badge`を選択します。
3.  `Set badge`モーダルで、ドキュメントに適用するバッジを選択し、次にバッジに関するメモを追加します（任意）。<img width="442" height="343" alt="93c323bcf1da34cef10cde8bd6e76f778618ef5b53c983e1d0d87519ba259f8f-image" src="https://github.com/user-attachments/assets/d31efc12-341e-45b3-bc80-25c4134f7484" />

4.  `Add`（現在バッジが設定されていない場合）または`Update`（既存のバッジを置き換える場合）をクリックしてバッジを設定します。

#### **バッジを削除する (Delete a badge)**
1.  削除したいバッジがあるドキュメントを開きます。
2.  ヘッダーで、ドキュメント名をクリックし、メニューから`File` > `Set badge`を選択します。
3.  `Set badge`モーダルで、`Delete`をクリックしてドキュメントからバッジを削除します。

### 5-3-3. ワークブックのバージョンとバージョン履歴 (Workbook versions and version history)

ワークブックにはバージョンがあります。デフォルトのバージョンは「Published」と「Draft」で、「タグ付きバージョン」と呼ばれる新しいカスタムバージョンを追加することもできます。バージョンタグ付けの詳細については、「[ワークブックとデータモデルにバージョンタグを追加する](https://help.sigmacomputing.com/docs/add-version-tags)」を参照してください。ワークブックの編集と公開の詳細については、「[ワークブックの編集、ドラフト、公開](https://help.sigmacomputing.com/docs/draft-and-publish-a-workbook)」を参照してください。

ワークブックのバージョン履歴には、以前に公開されたすべてのワークブックのバージョンのリストと、保留中のドラフトの変更が含まれています。各公開バージョンには、編集履歴と呼ばれる変更の詳細なリストが含まれています。バージョンと編集履歴を使用して、ドラフトされた変更を確認したり、古い公開バージョンと比較または元に戻したり、チームの誰が特定の編集または一連の変更を行ったかを特定したり、特定のバージョンタグでタグ付けされたバージョンを特定したりできます。ワークブックのバージョン履歴の保持期間に制限はありません。

#### **要件 (Requirements)**
* 編集履歴や現在のドラフトへの編集を含むワークブックのバージョン履歴は、ワークブックに対する`Can Edit`権限を持つユーザーのみが利用できます。
* ワークブックの古いバージョンや変更を復元できるのは、`Can Edit`権限を持つユーザーのみです。
* 2022年12月13日より前に行われた変更については、編集履歴は利用できません。2022年12月13日以降、ライブ編集が有効になっているすべての組織では、編集履歴で編集が追跡されます。ライブ編集が有効になる前に行われた編集は、追跡されません。詳細は、「[ワークブックでのライブ編集による共同作業](https://help.sigmacomputing.com/docs/collaborate-with-live-edit-in-workbooks)」を参照してください。

#### **ワークブックのバージョンについて (About workbook versions)**
ワークブックを開くと、現在のバージョンがワークブックヘッダーに表示されます。
* 公開済みのワークブックを表示している場合、バージョンは`PUBLISHED`です。
* タグ付きバージョンを表示している場合、バージョンタグの名前が表示されます。
* 編集のためにワークブックを開くと、バージョンは`DRAFT`です。

ワークブックは、以下のいずれかのバージョンを持つことができます。
* **Draft (ドラフト):** ワークブックを編集中は、ドラフトモードになり、変更はあなたと現在ワークブックを編集している他の人にのみ表示されます。
* **Published (公開済み):** ワークブックへの表示または探索アクセス権を持つ他の人が変更を見られるようにするには、それを公開します。
* **Tagged (タグ付き):** 特定のユーザーまたは特定の目的のためにワークブックの読み取り専用バージョンを利用可能にしたい場合は、特定のワークブックバージョンにタグを適用できます。例えば、「Development」や「Production」としてワークブックにタグを付けることができます。「[ワークブックとデータモデルにバージョンタグを追加する](https://help.sigmacomputing.com/docs/add-version-tags)」を参照してください。

ワークブックのバージョンのライフサイクルに関する詳細は、「[ワークブックの編集、ドラフト、公開](https://help.sigmacomputing.com/docs/draft-and-publish-a-workbook)」を参照してください。

#### **ワークブックのバージョン履歴を開く (Open version history for a workbook)**
ワークブックに変更を加えると、その変更はバージョン履歴に表示されます。バージョンを公開すると、バージョン履歴が更新されます。
バージョン履歴を表示するには、ワークブックに対する`Can Edit`権限が必要です。

1.  ワークブックを開きます。
2.  ドキュメント名の隣にあるキャレット()をクリックし、`Version history`を選択します。現在のバージョンの名前を選択し、`View version history`を選択することもできます。<img width="1370" height="790" alt="0194740807d15b795f80246ff4cf6000479c03ef296cb63e279a8a87db693814-workbook-vh-open" src="https://github.com/user-attachments/assets/97e12193-3881-404a-8fcf-266565a381d7" />

3.  バージョン履歴パネルが開き、最新バージョンとその変更が表示されます。以前に公開されたバージョンは以下にリストされ、現在公開されているバージョンに対応するバージョンには`Current`というラベルが付いています。 バージョンタイムスタンプの隣にあるシェブロンをクリックして特定のバージョンの詳細な編集履歴を確認するか、特定のバージョンまたは変更を選択してその時点でのワークブックを表示します。<img width="1371" height="577" alt="0ca6cd62dd323090a666c58d665ec54fa14bd8eb46e4941adacb35d485b18b06-selected-change-vh" src="https://github.com/user-attachments/assets/9d51bff1-5490-45b8-b95f-6dd7eafcf7c1" />

4.  ワークブックの最新バージョンに戻るには、`Go back to latest version`を選択します。
5.  バージョン履歴パネルを閉じるには、`X`をクリックします。

#### **ドラフトを以前の変更またはバージョンに復元する (Restore a draft to a previous change or version)**
ワークブックを以前に公開されたバージョンに戻すか、ワークブックのバージョン履歴の特定の変更に戻すには、以前の変更またはバージョンをドラフトとして復元します。以前のバージョンを復元する前に行われた変更は、バージョン履歴に残ります。
バージョン履歴の以前のバージョンまたは変更を復元するには、ワークブックに対する`Can Edit`権限が必要です。

* **ドラフトを以前に公開されたバージョンに復元する**
    ドラフトを以前に公開されたバージョンに復元するには、以下を実行します。
    1.  ワークブックのバージョン履歴を開きます。
    2.  復元したい以前に公開されたバージョンを探します。
    3.  `More`をクリックし、`Restore version as draft`を選択します。
    4.  変更は、リストされたバージョンのタイムスタンプとともに`Restored version from`としてバージョン履歴に表示されます。
    5.  必要に応じて他の変更を行うか、`Publish`をクリックして変更を公開します。

* **バージョン履歴の以前の変更に戻す**
    ワークブックのドラフトを、バージョンまたはドラフトの編集履歴の特定の変更に復元できます。
    > 🚧
    > ワークブックに入力テーブルが含まれており、バージョン履歴の以前の変更にワークブックを復元した場合、入力テーブルの内容はその時点には復元されず、代わりに最新の変更が反映されます。
    > 代わりに、特定の変更に最も近い公開バージョンを復元し、その後で特定の変更を復元することができます。
    ドラフトを編集履歴の以前の変更に戻すには、以下を実行します。
    1.  ワークブックのバージョン履歴を開きます。
    2.  ドラフトを戻したい変更が含まれるバージョンを探します。
    3.  必要に応じて、バージョンの編集履歴を展開し、その変更を探して選択します。
    4.  ワークブックヘッダーで、`Restore version as draft`を選択します。
    5.  変更は`Restored from autosaved draft`としてバージョン履歴に表示されます。
    6.  必要に応じて他の変更を行うか、`Publish`をクリックして変更を公開します。

#### **以前に公開されたバージョンを操作する (Work with previously published versions)**
ワークブックのバージョン履歴を確認する際、以前に公開されたバージョンに対していくつかのアクションを実行できます。`More`を選択して、以下のいずれかを実行します。
* **Restore version as draft:** バージョンをドラフトとして復元します。「[ドラフトを以前に公開されたバージョンに復元する](#restore-a-draft-to-a-previously-published-version)」を参照してください。
* **Edit name and description:** バージョンの名前と説明を変更します。デフォルトでは、バージョンはタイムスタンプでリストされます。
* **Save as new workbook:** バージョンを新しいワークブックとして保存します。
* **Copy link:** 以前のワークブックバージョンへのリンクをコピーします。ワークブックへのアクセス権を持つユーザーのみがリンクを表示できます。
* **Set a tag on the version:** バージョンにタグを設定します。「[ワークブックとデータモデルにバージョンタグを追加する](https://help.sigmacomputing.com/docs/add-version-tags)」を参照してください。

### 5-3-4. ワークブックとデータモデルにバージョンタグを追加する (Add version tags to workbooks and data models)

> 🚩
> データモデルのバージョンタグ付けはパブリックベータ機能であり、迅速で反復的な変更の対象となります。そのため、最新の製品バージョンはこのドキュメントの内容と異なる場合があります。詳細は、「[Beta features](https://help.sigmacomputing.com/docs/beta-features)」を参照してください。
> ワークブックのバージョンタグ付けは一般的に利用可能です。

ワークブックまたはデータモデルのバージョンにタグを追加して、そのドキュメントバージョンの読み取り専用ビューを作成します。その後、タグ付きバージョンを別のチームと共有して彼ら専用にしたり、タグ付きバージョンのワークブックをアプリケーションに埋め込んだり、タグ付きバージョンを使用してバージョン管理を行う開発ライフサイクルを実装したりできます。

ワークブックまたはデータモデルのバージョンにタグを付けると、タグ付きバージョンに影響を与えることなく、典型的なドラフトと公開のワークフローでソースドキュメントの反復作業を続けることができます。詳細は、「[Version tagging workflow](#version-tagging-workflow)」を参照してください。

ワークブックまたはデータモデルの複数のバージョンにタグを付けることができますが、同じタグでドキュメントの複数のバージョンにタグを付けることはできません。

管理者は、承認フローを必要とする保護されたタグの作成を含む、バージョンタグの作成と管理ができます。「[Create and manage version tags](https://help.sigmacomputing.com/docs/create-and-manage-version-tags)」を参照してください。

#### **バージョンタグ付けのワークフロー (Version tagging workflow)**
すべてのワークブックとデータモデルには、公開バージョンとドラフトがあります。ドキュメントに加えられたすべての変更は、[バージョン履歴](https://help.sigmacomputing.com/docs/document-versions-and-version-history)で表示できます。

特定のドキュメントバージョンにタグを付けて、そのドキュメントバージョンのステータスについて何かを示すことができます。例えば、ワークブックのバージョンにタグを付けて、内容の正確性をレビューする必要があること、または本番環境で使用する準備ができていることを示します。
<img width="1759" height="1344" alt="4be75c3ec3cb8eaefd59cade127457cb1258bb6afa73e321f0aa15e50a019c95-version-tag-workflow" src="https://github.com/user-attachments/assets/48cd4525-a2af-400f-b282-51adff62f8bb" />

データモデルにもタグを付け、同様のワークフローを使用して、テスト用または本番用に特定のデータモデルバージョンにタグを付けられます。

タグ付きバージョンがレビューされている間、ドラフトの反復作業を続けることができます。ドラフトまたは公開バージョンに加えられた変更は、タグ付きバージョンには影響しません。詳細は、「[Make changes to a tagged workbook version](#make-changes-to-a-tagged-workbook-version)」を参照してください。
<img width="1375" height="890" alt="6d1aa5d397ed3e77e4b4c358aba2e9e35d18a529aed6b3f1faeffa61e457880a-draft-publish-tag-workflow" src="https://github.com/user-attachments/assets/aec8133a-8631-4bae-a98d-f3db452e6385" />

##### **バージョンタグ付けがデータセットとデータモデルに与える影響 (How version tagging affects datasets and data models)**
データセットをデータソースとして使用するワークブックバージョンにタグを付けると、使用中のデータセットバージョンのコピーが作成され、タグ付きワークブックバージョンで使用されます。タグ付きワークブックバージョンに関連付けられたデータセットは、元のデータセットに変更が加えられても更新されなくなり、ワークブックバージョンがタグ付けされたときに使用されていたデータセットのバージョンが事実上凍結されます。データソース自体は、バージョンタグによって何ら影響を受けません。
<img width="3728" height="2664" alt="4dac999-vt-diagram-dataset" src="https://github.com/user-attachments/assets/e26ce890-aec5-474b-99c5-511642ca76e6" />

データモデルをデータソースとして使用するワークブックは、動作が異なります。データモデルをデータソースとして使用するワークブックバージョンにタグを付けると、ワークブックバージョンはタグ付けされますが、データモデルバージョンはタグ付けされません。新しい列の追加や既存の列のデータ型の変更など、データモデルに加えられた将来の変更は、そのデータモデルに依存するワークブックのバージョンと同期されます。
<img width="3728" height="2664" alt="841bfca-vt-diagram-data-model" src="https://github.com/user-attachments/assets/37455837-ff10-4cf4-95f3-c890752613ae" />

タグ付きバージョンのワークブックのデータソースとして使用されるデータモデルを「凍結」したい場合は、データモデルとワークブックの両方にタグを付け、タグ付きバージョンのワークブックのデータソースとしてタグ付きデータモデルを使用できます。「[Swap the source of a tagged workbook version](#swap-the-source-of-a-tagged-workbook-version)」を参照してください。

##### **タグ付きワークブックバージョンの埋め込み (Embedding tagged workbook versions)**
ワークブックを埋め込む場合、バージョンタグを使用して環境間でコンテンツをプロモートする管理ができます。例えば、「test」と「production」タグを使用して変更を管理し、本番で使用されるバージョンを保護します。その後、埋め込みでタグ付きバージョンへの直接リンクを使用できます。「[タグ付きバージョンのワークブックへのリンク](#link-to-a-tagged-version-of-a-workbook)」を参照してください。

バージョンタグのワークフローとタグ付きバージョンのワークブックへのアクセス制限に関する詳細は、「[タグ付きワークブックバージョンに変更を加える](#make-changes-to-a-tagged-workbook-version)」および「[ドキュメントのタグ付きバージョンを共有する](https://help.sigmacomputing.com/docs/share-a-workbook#share-tagged-versions-of-a-document)」を参照してください。

タグの作成と、リクエスト承認フローを強制するためのタグの保護に関する詳細は、「[バージョンタグの作成と管理](https://help.sigmacomputing.com/docs/create-and-manage-version-tags)」を参照してください。

Sigmaでのバージョンタグ付けを、開発ワークフローに既に統合されているソース管理プラットフォームと統合したい場合は、Sigma REST APIを使用できます。レシピについては、「[QuickStart - Embedding 08: Version Tagging](https://help.sigmacomputing.com/docs/quickstart-embedding-08-version-tagging)」を参照してください。

##### **バージョンタグ付けとマテリアライゼーション (Version tagging and materialization)**
マテリアライズされたデータソースに依存するワークブックのバージョンにタグを付けると、タグ付きバージョンはマテリアライズされたデータソースを使用しない場合があります。

* **マテリアライズされたデータセット:** マテリアライズされたデータセットは、タグ付きバージョンのワークブックでは使用されません。代わりに、タグ付きバージョンのワークブックは、タグが適用されたときに作成されたデータセットのコピーに依存します。
* **マテリアライズされたデータモデル:** タグ付きバージョンのワークブックのソースを交換する場合など、タグ付きバージョンのデータモデルを使用しない限り、マテリアライズされたデータモデルが使用されます。データモデルのタグ付きバージョンはマテリアライズできません。

| オブジェクト | マテリアライズされたバージョンは使用されるか？ | 詳細 |
| :--- | :--- | :--- |
| **データセット** | マテリアライズされたバージョンは使用されない | タグ付きバージョンのワークブックは、元のデータセットの代わりにデータセットのコピーを使用します。 |
| **データモデル** | マテリアライズされたバージョンは使用される | タグ付きバージョンのワークブックはデータモデルを使用し、データモデルに加えられた変更と同期を保ち、マテリアライズされた結果を使用します。 |
| **タグ付きデータモデル** | マテリアライズされたバージョンは使用されない | タグ付きバージョンのワークブックは、タグ付きバージョンのデータモデルを使用します。これは現時点ではマテリアライズできません。 |

マテリアライゼーションの詳細については、「[Materialization](https://help.sigmacomputing.com/docs/about-materialization)」を参照してください。

#### **ワークブックまたはデータモデルのバージョンにタグを付ける (Tag a workbook or data model version)**

ワークブックまたはデータモデルのバージョンにタグを付けることができます。ドキュメントにタグを付けると、そのドキュメントの読み取り専用バージョンが作成され、それを他の人と共有したり埋め込んだりできます。
> 🚧
> データモデルのタグ付きバージョンは、Ask Sigmaでは利用できません。管理者がAsk Sigmaで利用可能なデータソースにデータモデルを含めることを選択した場合、そのデータモデルの公開バージョンのみが利用可能であり、公開バージョンにアクセスできるユーザーのみがそのデータモデルを参照するAsk Sigmaからの回答を受け取ることができます。詳細は、「[組織のAI機能を構成する](https://help.sigmacomputing.com/docs/configure-ai-features-for-your-organization)」を参照してください。

##### **ユーザー要件 (User requirements)**
ドキュメントバージョンにタグを付けるには、以下が真である必要があります。
* ドキュメントに対する`Can Edit`[権限](https://help.sigmacomputing.com/docs/share-a-workbook)が付与されている。
* `Apply Tag`および`Create, edit, and publish workbooks`権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)が割り当てられている。

一部のタグは保護されており、ドキュメントに設定するには追加の権限が必要です。保護されたタグを設定するには、Adminアカウントタイプを割り当てられているか、保護されたタグを設定するアクセス権が付与されている必要があります。アクセス権がない場合は、タグの追加をリクエストできます。「[バージョンタグの作成と管理](https://help.sigmacomputing.com/docs/create-and-manage-version-tags)」を参照してください。

##### **ドキュメントにタグを設定する (Set a tag on a document)**
ドキュメントにタグを設定するには、以下の手順に従います。
1.  ドキュメントを開き、タグを付けたいバージョンを探します。
    * **ドキュメントの最新公開バージョンにタグを付けるには：**
        a. ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
        b. `Versions` > `Tag this version`を選択します。ドキュメントがドラフト状態で未公開の編集がある場合は、代わりに`Tag latest published version`と表示されます。
    * **ドキュメントの特定のバージョンにタグを付けるには：**
        a. ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
        b. `Versions` > `Version history`を選択し、タグを付けたいバージョンを探します。
        c. `More` > `Set tag on this version`をクリックします。
    `Set tag on version`モーダルが表示されます。
2.  `Choose tag`で、タグを選択します。
    適用する権限がない保護されたタグを選択した場合、タグの承認者にリクエストを送信するよう促されます。
    * a.`Request reason`に、保護されたタグをドキュメントに適用したい理由を正当化するためのメッセージをメールリクエストに含めて入力します。
    * b. `Request tag on version`をクリックします。
    * Sigmaはリクエストを承認できるユーザーにメールを送信します。
3.  [任意] タグ付きバージョンのドキュメントが異なるデータソースを使用するようにしたい場合は、`Swap sources of the tagged version`のチェックボックスを選択します。例えば、タグ付きバージョンに異なる接続、データベースまたはカタログ、テーブル、データモデル、またはデータセットを使用します。「[タグ付きバージョンのソースを交換する](#swap-the-source-of-a-tagged-workbook-version)」を参照してください。
    > 📘
    > ドキュメントに入力テーブルまたはCSVアップロードから作成されたテーブルが含まれている場合、このオプションを選択しないでください。これらの要素は接続間で移行できません。
4.  [任意] タグ付きバージョンのドキュメントへのアクセス権しか持たないユーザーが、デフォルトでタグ付きバージョンを開くようにしたい場合は、`Set this tag as default`のチェックボックスを選択します。「[ドキュメントのデフォルトバージョンタグを設定する](#set-a-default-version-tag-for-a-document)」を参照してください。
5.  バージョンタグ付きワークブックの場合、ワークブックで使用されているデータソースへの`Can view`アクセス権を付与したい場合は、`Allow user to use data sources when they "Save as"`のチェックボックスを選択します。このチェックボックスが選択されていない場合、ユーザーはデータなしでワークブックのタグ付きバージョンにアクセスします。
6.  `Set tag`をクリックします。
> 🚩
> ワークブックに入力テーブルが含まれている場合、タグ付きバージョンのワークブックには、ソースワークブックの入力テーブルとは別の空の入力テーブルのコピーが含まれます。ソースワークブックの入力テーブルに存在するデータをバージョンタグ付きバージョンに含めたい場合は、以下の手順が必要です：
> 1. 入力テーブルのデータ入力権限を、表示/探索モードで公開バージョンのみ編集可能に変更します。
> 2. バージョンタグを適用します。
> 3. 空のテーブルに手動でデータをコピー＆ペーストします。
> データモデルバージョンの一つの入力テーブルからタグ付きデータモデルバージョンにデータを移行したい場合、データモデルの公開バージョンの入力テーブルにデータを追加できないため、この回避策は利用できません。

#### **ドキュメントのデフォルトバージョンタグを設定する (Set a default version tag for a document)**

ワークブックまたはデータモデルにタグを適用する際、そのタグをデフォルトとして設定できます。デフォルトタグは、公開バージョンへのアクセス権がないユーザーに対して、デフォルトで表示されるドキュメントのバージョンを決定します。ユーザーが公開バージョンへのアクセス権を持っている場合、公開バージョンがデフォルトタグよりも優先されます。

> 📘
> ユーザーがドキュメントの公開バージョンにアクセスできず、デフォルトのバージョンタグが設定されていない場合、ドキュメントはユーザーがアクセスできる最新作成のタグ付きバージョンをロードします。

ドキュメントに対する`Can edit`アクセス権を持つ任意のユーザーが、タグをデフォルトとして設定できます。
1.  ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
2.  `Versions` > `Version history`を選択します。
3.  デフォルトとして設定したいタグ付きバージョンを探し、`More`を選択します。
4.  `Set tag as default`をクリックします。

タグをデフォルトから削除し、別のデフォルトタグに置き換えない場合は、以下の手順に従います。
1.  ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
2.  `Versions` > `Version history`を選択します。
3.  デフォルトバージョンタグの隣にある`More`を選択します。
4.  `Remove as default`をクリックします。

#### **ドキュメントバージョンからタグを削除する (Remove a tag from a document version)**

ワークブックまたはデータモデルのバージョンからタグを削除すると、バージョンはバージョン履歴から引き続きアクセス可能ですが、タグ付きバージョンへのアクセス権しか持たない人はドキュメントへのアクセスを失います。

> 💡
> 間違ったドキュメントバージョンにタグを付けた場合や、タグ付きバージョンへのアクセスのみを持つユーザーのアクセスを制限したい場合にタグを削除することがあります。タグ付きバージョンを更新したい場合は、このドキュメントの「[タグ付きワークブックバージョンに変更を加える](https://help.sigmacomputing.com/docs/add-version-tags#make-changes-to-a-tagged-workbook-version)」を参照してください。

ドキュメントバージョンからタグを削除するには：
1.  ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
2.  `Versions` > `Version history`を選択します。
    > 💡
    > 各バージョンの詳細な変更を折りたたむには、最新バージョンの隣にある下矢印を選択します。
3.  タグ付きバージョンを探し、`More` > `Remove this tag`を選択します。
4.  タグを削除すると、タグ付きバージョンがキャンバスに表示されます。

#### **タグ付きワークブックバージョンのソースを交換する (Swap the source of a tagged workbook version)**
> 📘
> ワークブックに複数のデータソースからの要素が含まれている場合、タグ付きワークブックバージョンのソースを交換することはできません。

タグ付きワークブックバージョンのソースを交換するには、例えば「testing」とタグ付けされたワークブックにテストデータ接続を使用し、「production」とタグ付けされたワークブックに本番データ接続に交換するなど、以下の手順に従います。手順は、ワークブックがデータソースとしてデータモデルを使用しているかどうかによって異なります。
* [タグ付きワークブックバージョンで使用されるデータモデルソースを交換する](#swap-the-data-model-source-used-by-a-tagged-workbook-version)
* [タグ付きワークブックバージョンで使用されるデータセットまたは接続ソースを交換する](#swap-the-dataset-or-connection-source-used-by-a-tagged-workbook-version)

ワークブックのデータソースの変更に関する詳細は、「[ワークブックまたは要素のデータソースを変更する](https://help.sigmacomputing.com/docs/change-the-data-source-for-a-workbook-or-element)」を参照してください。

##### **タグ付きワークブックバージョンで使用されるデータモデルソースを交換する (Swap the data model source used by a tagged workbook version)**
ワークブックがデータソースとしてデータモデルを使用しており、タグ付きワークブックバージョンが公開バージョンとは異なるデータソースを使用するようにしたい場合は、まずデータモデルにタグを付けてタグ付きデータモデルのソースを交換し、次にワークブックにタグを付けてタグ付きデータモデルをソースとして使用します。
ワークブックがデータソースとして使用するデータモデルが、別のデータモデルに基づいている場合は、そのソースデータモデルにもタグを付けます。
> 💡
> データソースで使用される接続を交換する場合、ワークブックバージョンではなくデータモデルバージョンにタグを付けてソースを交換すると、データソースへのアクセスをより簡単に管理および制御できます。

* **データモデルにタグを付けてソースを交換する**
    1.  編集のためにデータモデルを開き、タグを付けるバージョンを選択します。
    2.  `Set tag on version`モーダルが表示されます。
    3.  `Choose tag`で、データモデルに適用するタグを選択します。ワークブックで使用する予定の同じタグを選択します。
    4.  `Swap sources of the tagged version`のチェックボックスを選択します。
    5.  `Set tag`をクリックします。
    6.  `Swap sources`モーダルで、`Sources of tagged data model`に、タグ付きバージョンで使用する新しいデータソースを選択します。代わりにデータベースまたはカタログ、スキーマ、またはテーブルを変更したい場合は、現在のオブジェクト名にカーソルを合わせ、`Select`をクリックして別のオブジェクトを選択し、`Confirm`をクリックします。
    7.  `Swap and tag`を選択します。

* **ワークブックにタグを付けて、ソースをタグ付きデータモデルに交換する**
    1.  編集のためにワークブックを開き、タグを付けるバージョンを選択します。
    2.  `Set tag on version`モーダルが表示されます。
    3.  `Choose tag`で、ワークブックバージョンに適用するタグを選択します。
    4.  `Swap sources of the tagged version`のチェックボックスを選択します。
    5.  `Set tag`をクリックします。
    6.  `Swap sources`モーダルで、`Sources of tagged workbook`についてドロップダウンメニューを開き、対応するタグ付きバージョンのデータモデルを選択します。
        > 📘
        > ワークブックに複数のデータソースが含まれている場合、各データソースのソースを交換するオプションが表示されます。
    7.  `Swap and tag`を選択します。

##### **タグ付きワークブックバージョンで使用されるデータセットまたは接続ソースを交換する (Swap the dataset or connection source used by a tagged workbook version)**
タグ付きワークブックバージョンに異なる接続パス、データベース、またはスキーマを選択するには、以下を実行します。
1.  編集のためにワークブックを開き、タグを付けるバージョンを選択します。
2.  `Set tag on version`モーダルが表示されます。
3.  `Choose tag`で、ワークブックバージョンに適用するタグを選択します。
4.  `Swap sources of the tagged version`のチェックボックスを選択し、`Set tag`をクリックします。
5.  `Swap sources`モーダルで、`Sources of tagged data model`に、タグ付きバージョンで使用する新しいデータソースを選択します。
6.  `Swap and tag`をクリックします。
タグ付きバージョンのワークブックは、新しい接続を使用するように更新されます。ワークブックがデータセットを使用している場合、新しい接続上にデータセットのコピーが作成されます。


#### **タグ付きワークブックバージョンに変更を加える (Make changes to a tagged workbook version)**

タグ付きバージョンのワークブックに変更を加えたい場合は、まずタグ付きバージョンをドラフトに戻し、変更を加え、変更を公開し、バージョンに再度タグを付ける必要があります。

例えば、「testing」タグでワークブックバージョンにタグを付けた後、本番環境で使用する準備ができたことを示すために「production」タグでワークブックにタグを付ける開発ライフサイクルに従う場合、「testing」タグで反復作業を行いたい場合があります。

「testing」タグ付きバージョンのワークブックを更新するには、以下を実行します。
1.  編集のためにワークブックを開きます。
2.  ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
3.  `Versions` > `Version history`を選択します。
4.  タグ付きバージョンを探し、関連するバージョンの日付を選択して開きます。
5.  そのバージョンについて、`More` > `Restore version as draft`を選択します。
6.  ドラフトで希望の変更を加えます。
7.  変更が終わったら、変更を公開します。
8.  ドキュメントメニューを開き、`Versions` > `Version history`を選択して、バージョン履歴を再度開きます。
9.  バージョン履歴には、`Restored version from <date>`という項目が表示され、そのバージョンの上にさらなる変更がリストされます。
10. 変更を含む最新の公開バージョンについて、`More > Set tag on this version`を選択します。
11. 最新バージョンにタグが付けられ、内容が一致するように更新されます。以前にタグ付けされたバージョンは、グレーアウトされたバージョンタグでリストされます。
    > 📘
    > 以前のバージョンからtestingタグを削除しないでください。そうすると、そのタグ付きバージョンのワークブックへのアクセス権しか持たない人はアクセスを失います。異なるバージョンに再度タグを付けると、共有は維持されます。
12. 保存して作業を続けたい他の変更があった場合は、タグ付きバージョンを最新のドラフトとして復元する前のバージョンに戻り、`More > Restore version as draft`を選択します。

#### **タグ付きバージョンを別のタグに更新する (Update a tagged version to use another tag)**
例えば、「staging」バージョンタグから「production」バージョンタグにタグ付きワークブックバージョンを昇格させたい場合は、以下を実行します。
1.  編集のためにワークブックを開きます。
2.  ドキュメント名の隣にある下矢印()をクリックしてドキュメントメニューを開きます。
3.  `Versions`を選択し、表示したいタグ（例：「Staging」）を選択します。
    タグ付きバージョンが開きます。
4.  ドキュメントメニューを開き、`Versions` > `Tag this version`を選択します。
    `Set tag on version`モーダルが開きます。
5.  モーダルで、関連オプションを選択し、`Set tag`を選択します。
    「Production」タグがバージョンに追加されます。
6.  次に、バージョンから「Staging」タグを削除します。ドキュメントメニューを開き、`Versions` > `Version history`を選択します。
7. バージョン履歴で、「Staging」タグが適用されているバージョンを探し、`More` > `Remove this tag`を選択します。
8. モーダルで、このタグ付きバージョンへのアクセス権のみが付与されているユーザー、またはタグ付きバージョンへのリンクを使用する埋め込みが、タグを削除した後にアクセスを失うことを承認し、`Remove`を選択します。
   バージョンは、現在のタグが「Production」、以前のタグが「Staging」として表示されます。

#### **バージョンタグを使用してフォルダへのアクセスを制限する (Restrict access to a folder using a version tag)**
バージョンタグを使用してドキュメントへのアクセスを管理する場合、ワークスペースまたはフォルダを設定してアクセスをより簡単に管理できます。
ワークスペースまたはフォルダをユーザーまたはチームと共有し、それらのユーザーまたはチームに特定のタグへのアクセス権を付与できます。そうすると、そのワークスペースまたはフォルダ内のワークブックまたはデータモデルは、それらのユーザーまたはチームがアクセスできるようにするために、そのタグが適用されている必要があります。

例えば、5つの地域をカバーする営業組織がある場合、各地域にワークスペースを作成し、各営業チームにその地域のタグを持つワークスペースへの`Can explore`アクセス権を付与できます。
そうすると、ワークスペース内のすべてのドキュメントには、対応するタグ付きバージョンが必要です。この例では、Sales US-Eastワークスペース内のすべてのワークブックには、Sales US-Eastチームのメンバーがワークブックの`East`バージョンを表示および探索できるように、`East`とタグ付けされたバージョンが必要です。

ワークスペースでチームメンバーに`Can contribute`や`Can manage`などの昇格された権限を付与すると、それらのチームメンバーはワークスペース内のドキュメントのすべてのバージョンにアクセスできます。
ワークスペースおよびフォルダレベルで設定された権限は、ワークスペースまたはフォルダ内のワークブックおよびドキュメントに継承されます。詳細は、「[フォルダを共有する](https://help.sigmacomputing.com/docs/share-a-folder)」を参照してください。

#### **タグ付きバージョンのワークブックへのリンク (Link to a tagged version of a workbook)**
タグ付きバージョンのワークブックに直接リンクしたい場合（例えば、タグ付きバージョンのワークブックを埋め込むなど）、URLでタグ名を参照します。
例えば、ワークブックに`staging`タグを追加した場合、`staging`でタグ付けされたワークブックバージョンのURLには以下が含まれます。
`/workbook/My-Workbook-{workbook_id}/tag/staging`

埋め込みにも同じ構成が適用されます。`staging`タグはURLに追加されます。
`/embed/{embed_id}/tag/staging`

他のURLパラメータと同様に、スペースや特殊文字を含むバージョンタグ名はエンコードされます。例えば、「Staging Copy」という名前のバージョンタグの場合は`staging%20copy`となります。「[Embed URL parameters](https://help.sigmacomputing.com/docs/embed-url-parameters)」を参照してください。

### 5-4. マテリアライゼーション

#### 5-4-1-1. マテリアライゼーションについて (About materialization)

> 🚩
> データモデル内のデータ要素とデータセットのマテリアライゼーションは、一般的に利用可能です。
> ワークブック内のデータ要素のマテリアライゼーションは、パブリックベータです。
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このドキュメントは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

マテリアライゼーションは、レポートの速度とパフォーマンスを向上させます。データモデル、ワークブック、およびデータセットに対してマテリアライゼーションを設定できます。

##### **マテリアライゼーションについて (About materialization)**
データ要素間の複雑な結合や、カーディナリティが高く複数のグルーピングレベルと計算列を持つデータセットなど、コストのかかる、または長時間実行されるクエリを使用するデータソースがある場合、マテリアライゼーションを設定することでクエリのパフォーマンスが向上し、コンピューティングコストの削減に役立ちます。

マテリアライゼーションは、データセットまたはデータ要素のコピーをテーブルとして、または場合によっては動的テーブルとして、あなたのウェアハウスに書き戻します。マテリアライズされたデータは、Sigmaサービスによって管理されるスキーマ内のクラウドデータウェアハウスに、すべての書き戻しデータに使用されるのと同じデータベースまたはカタログとスキーマに保存されます。マテリアライズされたテーブルは、先頭に `t_mat` または `T_ID` が付くか、末尾に `_MAT` が付き、Sigmaの接続エクスプローラーには表示されません。

##### **マテリアライゼーションが使用されるとき (When materialization is used)**
マテリアライゼーションを使用する要素を表示または操作すると、Sigmaのクエリコンパイラは自動的かつ透過的に最新のマテリアライゼーションを使用します。あなたのクラウドデータウェアハウスはクエリを再計算しません。
ワークブックページのコントロールがマテリアライズされた要素を対象としている場合、コントロールの値を変更するとライブデータにクエリが実行されます。代わりに、コントロールをワークブックまたはデータモデルの子要素を対象にしてください。「[マテリアライゼーションのベストプラクティス](#best-practices-for-materialization)」を参照してください。
ワークブックまたはデータモデルのマテリアライズされたデータセットまたはマテリアライズされた要素を編集すると、マテリアライズされたデータは使用されず、正確な結果を保証するために基盤となるデータにクエリが実行されます。

##### **データモデルとワークブックのマテリアライゼーションとデータセットのマテリアライゼーションの比較**
ワークブックとデータモデルのマテリアライズされたデータ要素は、マテリアライズされたデータセットとはいくつかの違いがあります。
* データセットを公開すると、変更がマテリアライゼーションの正確さに影響しない場合でも、マテリアライゼーションが実行されます。マテリアライズされた要素を持つワークブックまたはデータモデルを公開すると、公開された変更がマテリアライゼーションに影響する場合にのみ、マテリアライゼーションが実行されます。
* データセットに複数のグルーピングレベルが含まれている場合、1つのグルーピングレベルしかマテリアライズできません。ワークブックまたはデータモデルのデータ要素に複数のグルーピングレベルが含まれている場合、各グルーピングレベルをマテリアライズできます。
* ワークブックとデータモデルのデータ要素の未使用のマテリアライゼーションは、自動的に一時停止できます。未使用のデータセットのマテリアライゼーションは自動的に一時停止できません。詳細は「[マテリアライゼーションの管理](https://help.sigmacomputing.com/docs/manage-materializations)」を参照してください。
* Snowflake接続でマテリアライゼーションを使用する場合、ワークブックとデータモデルのマテリアライズされたデータ要素は一時テーブルを使用します。一時テーブルの詳細については、Snowflakeドキュメントの「[Working with Temporary and Transient Tables](https://docs.snowflake.com/en/user-guide/tables-temp-transient)」を参照してください。

##### **動的テーブルによる増分マテリアライゼーション (Incremental materialization with dynamic tables)**
デフォルトでは、マテリアライゼーションは毎回新しいテーブルを作成します。Snowflake接続でマテリアライゼーションを使用する場合、代わりにマテリアライゼーションに動的テーブルを使用するように接続を構成できます。多くの場合、動的テーブルは増分更新を可能にし、つまり、マテリアライゼーションが実行されると、変更されたデータのみが更新されます。

マテリアライゼーションに動的テーブルを使用するには：
1.  マテリアライゼーションに動的テーブルを使用するように接続を構成します。「[Connect to Snowflake](https://help.sigmacomputing.com/docs/connect-to-snowflake)」の「書き込みアクセスを構成する」を参照してください。
2.  マテリアライゼーションに使用される動的テーブルを構築するためにクエリされる可能性のあるデータベーステーブルで、変更追跡を有効にします。Snowflakeドキュメントの動的テーブル作成に関する「[Enable change tracking](https://docs.snowflake.com/en/user-guide/dynamic-tables-creating#enabling-change-tracking-on-underlying-objects)」を参照してください。

これらのステップを完了すると、マテリアライゼーションは動的テーブルを使用し、利用可能であれば増分リフレッシュを使用します。増分リフレッシュが利用できない場合は、完全なリフレッシュが実行されます。動的テーブルが利用できないかサポートされていない場合は、テーブルが使用されます。要素のマテリアライゼーション履歴を確認して、どの方法が使用されたかを確認できます。「[マテリアライズされたデータ要素のステータスを確認する](https://help.sigmacomputing.com/docs/schedule-materialization-for-a-data-model-or-workbook#review-the-status-of-a-materialized-data-element)」を参照してください。

増分リフレッシュが使用されない場合や、動的テーブルが使用されない場合についての詳細は、Snowflakeドキュメントの「[Known limitations for dynamic tables](https://docs.snowflake.com/en/user-guide/dynamic-tables-limitations)」を参照してください。

既存のマテリアライゼーションスケジュールは、次回のスケジュールされた実行の一部として動的テーブルを使用しようとします。ワークブックとデータモデルのデータ要素のみが、動的テーブルによる増分マテリアライゼーションを使用できます。マテリアライズされたデータセットは動的テーブルを使用しません。

##### **マテリアライゼーションのベストプラクティス (Best practices for materialization)**
* マテリアライゼーションをスケジュールする際は、データの更新時間を考慮してください。データウェアハウスのデータがスケジュールで更新される場合、Sigmaのマテリアライゼーションスケジュールがそのデータ更新の完了後に開始するようにしてください。
* データが使用されないと予想されるときにマテリアライゼーションが実行されるようにスケジュールし、ユーザーがデータにアクセスする前に完了させます。必要であれば、マテリアライゼーションに使用する専用のコンピューティングリソースを作成します。例えば、マテリアライゼーションをゆっくり実行するが、リソースの使用量が少ない小さなコンピューティングリソースを作成します。
* 上流の要素をマテリアライズする場合、下流のマテリアライズされた要素のマテリアライゼーションスケジュールが、上流の要素のマテリアライゼーションの完了後に開始するようにしてください。
* データ構造の変更が将来のマテリアライゼーションの失敗を引き起こさないように、データモデルまたはデータセットを設定する際には、[マテリアライゼーションの制限](#materialization-limitations)を考慮してください。
* マテリアライズされたデータソースと要素の子要素にコントロールを対象として、信頼性の高いインタラクションと出力を確保します。
* 長時間実行されるクエリのタイムアウト制限を考慮してください。マテリアライゼーションクエリは、[接続で構成されたSigmaのクエリタイムアウト](https://help.sigmacomputing.com/docs/manage-workbook-refresh-options#set-a-query-id-cache-duration)を使用せず、代わりにデータプラットフォームで使用されるコンピューティングリソースで定義された設定（例えば、Snowflakeの仮想ウェアハウスのクエリタイムアウト設定など）を使用します。

##### **マテリアライゼーションの制限 (Materialization limitations)**
一部のデータ構造はマテリアライズできません。[行レベルのセキュリティ](https://help.sigmacomputing.com/docs/set-up-row-level-security)を持つデータセットなど、一つ以上の[システム関数](https://help.sigmacomputing.com/docs/system-functions)を使用する列がデータに含まれている場合、マテリアライゼーションは実行に失敗します。

マテリアライゼーションは実行時のデータの固定出力を反映するため、一部のデータ構造は予期しない結果を生むことがあります。
* データセットが[パラメータ](https://help.sigmacomputing.com/docs/create-and-manage-dataset-parameters)を使用する場合、マテリアライゼーションはパラメータの初期値を使用して実行されます。パラメータへの将来の変更は影響しません。
* ワークブックまたはデータモデルのデータ要素が一つ以上の[コントロール](https://help.sigmacomputing.com/docs/intro-to-control-elements)の対象となっている場合、マテリアライゼーションはコントロールの初期値を使用して実行されます。マテリアライゼーション後、コントロールを使用してマテリアライズされたデータ要素と対話すると、マテリアライズされたデータは使用されず、代わりにクエリが実行されて最新のデータが取得されます。代わりに、コントロールを子要素を対象にしてください。

ワークブックやデータモデルのデータ要素は、ルックアップ、[結合](https://help.sigmacomputing.com/docs/join-data-in-workbooks)、リレーションシップなどで他のデータ要素を参照していてもマテリアライズできますが、ソースデータ要素の一つがマテリアライズできない場合を除きます。
データセットは、ルックアップ、リンク、または[結合](https://help.sigmacomputing.com/docs/join-data)などで他のデータセットを参照していてもマテリアライズできますが、ソースデータセットの一つがマテリアライズできない場合を除きます。
OAuth認証を使用してデータプラットフォームに接続している場合、ワークブックやデータモデルのデータ要素はマテリアライズできますが、データセットはマテリアライズできません。

##### **マテリアライゼーションを設定する (Set up materialization)**
データモデルやワークブックの要素、またはデータセットにマテリアライゼーションを設定するには：
* [データモデルまたはワークブックのマテリアライゼーションをスケジュールする](https://help.sigmacomputing.com/docs/schedule-materialization-for-a-data-model-or-workbook)
* [データセットのマテリアライゼーションをスケジュールする](https://help.sigmacomputing.com/docs/dataset-materialization-api)
* 
#### 5-4-1-2. データモデルまたはワークブックのマテリアライゼーションをスケジュールする (ベータ版)

> 🚩
> データモデル内のデータ要素のマテリアライゼーションは一般的に利用可能です。
> ワークブック内のデータ要素のマテリアライゼーションはパブリックベータです。
> このドキュメントはパブリックベータ機能について説明しており、現在作成中です。この通知およびSigmaサービス内の機能に対応するベータフラグが削除されるまで、このドキュメントは公開されたドキュメントの一部とは見なされません。他のベータ機能と同様、以下で説明する機能は、迅速で反復的な変更の対象となります。Sigmaサービスでの最新の体験は、このドキュメントの内容と異なる場合があります。
> ベータ機能は、[ベータ機能](https://help.sigmacomputing.com/docs/beta-features)の免責事項の対象となります。

マテリアライゼーションをスケジュールすることにより、ワークブックまたはデータモデル内のデータ要素をマテリアライズします。構成したマテリアライゼーションスケジュールは、下流の要素のデータの鮮度に影響します。制限事項やベストプラクティスを含む詳細については、「[マテリアライゼーションについて](https://help.sigmacomputing.com/docs/about-materialization)」を参照してください。データモデルがバージョンタグを使用している場合は、「[バージョンタグ付きデータモデルのマテリアライゼーションをスケジュールする](https://help.sigmacomputing.com/docs/schedule-materialization-for-a-version-tagged-data-model)」を参照してください。

##### **要件 (Requirements)**
* 接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。
* データモデルでマテリアライゼーションをスケジュールするには、`Schedule materializations`および`Create, edit, and publish datasets`権限が有効になっているアカウントタイプを割り当てられている必要があります。
* ワークブックでマテリアライゼーションをスケジュールするには、`Schedule materializations`および`Create, edit, and publish workbooks`権限が有効になっているアカウントタイプを割り当てられている必要があります。
* ワークブックまたはデータモデルに対する`Can Edit`アクセス権が必要です。

##### **データ要素のマテリアライゼーションスケジュールを作成する (Create a data element materialization schedule)**
ワークブックまたはデータモデル内の特定のデータ要素をマテリアライズできます。
> 📘
> データ要素は1つのマテリアライゼーションスケジュールしか持てませんが、1つのスケジュールで複数の要素をマテリアライズするように作成できます。

1.  編集のためにデータモデルまたはワークブックを開きます。
2.  マテリアライズしたい要素を探し、`More`をクリックして要素メニューを開きます。
3.  `Advanced options` > `Schedule materialization...`を選択します。
4.  `Materialization schedules`モーダルで、データ要素をマテリアライズするスケジュールを設定します。
    * (任意) `Daily`のドロップダウンを選択し、`Weekly`, `Monthly`, または`Custom`を選択します。
        * `Daily`の場合、`Once a day`または`Multiple times`を選択します。
        * `Weekly`の場合、マテリアライゼーションジョブを実行する曜日を選択し、`Once a day`または`Multiple times`を選択します。
        * `Monthly`の場合、マテリアライゼーションジョブを実行する月の日と時刻を選択します。
        * `Custom`の場合、cron構文を使用してスケジュールを指定します。
    * `Multiple times`を選択した場合は、頻度を指定します。例えば、午前9時から午後6時までの間、毎時15分に2時間ごとなど。
    * (任意) ドロップダウンメニューを使用して、デフォルトのスケジュールタイムゾーンを調整します。
    > 📘
    > 要素に複数のグルーピングレベルが含まれている場合、マテリアライズするグルーピングレベルを選択します。Sigmaは選択されたグルーピングレベルとその上位のすべてのレベルをマテリアライズします。グループ化された要素の最も粒度の細かいレベル（All source columns）をマテリアライズすることは、しばしば不要でコストがかかる可能性があります。
5.  `Save schedules`をクリックします。
マテリアライゼーションの実行は、ワークブックの最新の公開バージョンを使用して直ちに開始されます。
> 🚩
> データプラットフォームへの認証にOAuthを使用する場合、マテリアライゼーションジョブはマテリアライゼーションをスケジュールしたユーザーとして実行されます。代わりにサービスアカウントを使用してマテリアライゼーションを実行するには、ワークブックをサービスアカウントとして実行します。「[Run a workbook with service account credentials](https://help.sigmacomputing.com/docs/run-a-workbook-with-service-account-credentials)」を参照してください。

##### **依存マテリアライゼーションスケジュールを設定する (Set up a dependent materialization schedule)**
親要素と子要素の両方をマテリアライズする場合、子要素に対して依存マテリアライゼーションスケジュールを設定できます。依存マテリアライゼーションスケジュールでは、一つ以上の子要素のマテリアライゼーションは、親要素のマテリアライゼーションが正常に完了した後に実行されます。依存マテリアライゼーションは、子要素のデータが親要素で利用可能な最新のデータを反映することを保証するのに役立ちます。

親要素は、同じワークブック、データモデル、またはデータモデルをまたいで、複数のレベル上流にある場合があります。親要素と子要素を特定するには、ワークブックまたはデータモデルの[データリネージ](https://help.sigmacomputing.com/docs/view-workbook-data-lineage)を確認してください。

依存マテリアライゼーションスケジュールを設定するには、以下を実行します。
1.  編集のためにデータモデルまたはワークブックを開きます。
2.  マテリアライズしたい子要素を探し、`More`をクリックして要素メニューを開きます。
3.  `Advanced options > Schedule materialization...`を選択します。
4.  `Materialization schedules`モーダルが、選択した要素のドラフトスケジュールと共に開きます。
5.  `Frequency`セクションの`Select a run time`で、オプションを選択します。
    * 子要素を親要素のマテリアライゼーションが正常に終了した後にのみマテリアライズするには、`After selected parent schedule finishes`を選択し、ドロップダウンメニューで関連する親スケジュールを選択します。
    * 親要素のマテリアライゼーションスケジュールとは別に、子要素を独自のスケジュールでマテリアライズするには、`Manual Time`を選択し、頻度を指定します。
6.  [任意] 同じスケジュールで複数の要素をマテリアライズしたい場合は、`+ Add element`を選択し、別の要素を選択します。
7.  `Save schedules`を選択します。
保存後、依存スケジュールは親スケジュールと同じスケジュールの一部として表示されます。親スケジュールが一時停止または失敗した場合、依存スケジュールも一時停止または失敗します。
> 📘
> 親要素のマテリアライゼーションスケジュールが削除された場合、依存スケジュールは親要素に設定された頻度と一致するように更新されます。

##### **マテリアライズされたデータ要素のステータスを確認する (Review the status of a materialized data element)**
マテリアライゼーションのステータスはいくつかの場所で確認できます。
* ワークブックまたはデータモデルでデータ要素を表示すると、要素メニューにマテリアライゼーションのステータスが表示されます。
* データ要素のリネージを確認すると、マテリアライゼーションのステータスが表示されます。

データ要素のマテリアライゼーション履歴を確認するには：
1.  編集のためにデータモデルまたはワークブックを開きます。
2.  マテリアライズしたい要素を探し、`More`をクリックして要素メニューを開きます。
3.  `Advanced options` > `Schedule materialization...`を選択します。
4.  `Materialization schedules`モーダルで、`History`を選択します。
5.  ワークブックまたはデータモデル内のすべての要素のマテリアライゼーション履歴を確認します。
    * マテリアライゼーションのステータスを確認します。失敗したマテリアライゼーションについては、エラーメッセージをコピーできます。
    * マテリアライゼーションの開始時刻と実行時間を確認します。
    * 総行数と総バイト数でマテリアライズされたデータの量を確認します。
    * `More`を選択して要素を直ちにマテリアライズするか、その要素をマテリアライズするスケジュールに移動します。

##### **スケジュールされたマテリアライゼーションを実行する (Run a scheduled materialization for a data element)**
スケジュールされたマテリアライゼーションを持つデータ要素を直ちにマテリアライズするには：
1.  マテリアライズされたデータ要素を選択します。
2.  メニューで、`View materialization info` ()を選択します。
    * このオプションが利用できない場合、要素はマテリアライズされていません。「[データ要素のマテリアライゼーションスケジュールを作成する](https://help.sigmacomputing.com/docs/schedule-materialization-for-a-data-model-or-workbook#create-a-data-element-materialization-schedule)」を参照してください。
3.  表示されるメニューで、`Materialize now`をクリックします。
マテリアライゼーションの実行は、ワークブックの最新の公開バージョンを使用して直ちに開始されます。

また、スケジュールからデータ要素のマテリアライゼーションを実行することもできます。例えば、同じスケジュール内のすべてまたは複数の要素のマテリアライゼーションを直ちに実行したい場合などです。
1.  マテリアライズされたデータ要素を選択します。
2.  `More`をクリックして要素メニューを開きます。
3.  `Advanced options` > `Schedule materialization...`を選択します。
4.  `Materialization schedules`モーダルで、スケジュール内の要素を確認し、直ちにマテリアライズするものを選択します。
    * スケジュール内のすべての要素をマテリアライズするには、ヘッダー行で`More` > `Materialize all now`を選択します。
    * スケジュール内の個々の要素をマテリアライズするには、要素の行を探し、`More` > `Materialize now`を選択します。
マテリアライゼーションの実行は、ワークブックの最新の公開バージョンを使用して直ちに開始されます。

##### **マテリアライゼーションスケジュールを管理する (Manage the materialization schedule for a data element)**
マテリアライゼーションスケジュールを変更して、マテリアライズの頻度やどの要素がマテリアライズされるかを変更できます。また、スケジュールから一つ以上の要素を削除したり、スケジュール全体を削除したりすることもできます。要素またはスケジュール全体を削除すると、関連するテーブルは24時間以内にデータプラットフォームから削除されます。

1.  編集のためにデータモデルまたはワークブックを開きます。
2.  マテリアライズしたい要素を探し、`More`をクリックして要素メニューを開きます。
3.  `Advanced options` > `Schedule materialization...`を選択します。
4.  `Materialization schedules`モーダルで、希望の変更を加えます。
    * スケジュールの頻度を修正する。
    * スケジュールから要素を削除する。要素の行を探し、`More` > `Remove element`を選択します。
    * `Delete schedule`を選択してスケジュールを削除する。

管理者として、追加のマテリアライゼーション機能を管理するには、「[マテリアライゼーションの管理](https://help.sigmacomputing.com/docs/manage-materializations)」を参照してください。

#### 5-4-1-3. データセットのマテリアライゼーションをスケジュールする (Schedule materialization for a dataset)

マテリアライゼーションをスケジュールすることにより、データセットをマテリアライズします。構成したマテリアライゼーションスケジュールは、下流の要素のデータの鮮度に影響します。制限事項やベストプラクティスを含む詳細については、「[マテリアライゼーションについて](https://help.sigmacomputing.com/docs/about-materialization)」を参照してください。

##### **要件 (Requirements)**
* 接続で[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている必要があります。
* データセットでマテリアライゼーションをスケジュールするには、`Schedule materializations`および`Create, edit, and publish datasets`権限が有効になっているアカウントタイプを割り当てられている必要があります。
* データセットに対する`Can Edit`アクセス権が必要です。

##### **データセットのマテリアライゼーションスケジュールを作成する (Create a materialization schedule for a dataset)**
データセットをマテリアライズするには：
1.  マテリアライズしたいデータセットを開きます。
2.  `Materialization`タブを選択し、`Create Schedule`をクリックします。
3.  `Add Materialization Schedule`モーダルで、マテリアライズされたデータを更新するためのスケジュールを定義します。
4.  `Save`をクリックします。
データの最初のマテリアライゼーションは直ちに開始されます。

##### **データセットのマテリアライゼーションのステータスを確認する (Review the status of a dataset materialization)**
データセットがマテリアライズされている場合、データセットのヘッダーでマテリアライゼーションのステータスを確認できます。
1.  データセットヘッダーで、情報アイコン()をクリックしてデータセット情報を開きます。
2.  `Materialization`セクションで、ステータスを確認します。最終更新日や次回更新日などの詳細を表示するには、ステータスにカーソルを合わせます。

Adminアカウントタイプを割り当てられたユーザーは、いつでも`Materialization`タブからマテリアライゼーションのステータスと履歴を表示できます。「[Manage materializations](https://help.sigmacomputing.com/docs/manage-materializations)」を参照してください。

##### **データセットのマテリアライゼーションジョブを実行する (Run a materialization job for a dataset)**
スケジュールされたマテリアライゼーションを手動で実行するには、以下を実行します。
1.  データセットを開き、`Materialization`タブを選択します。
2.  `Schedule`セクションで、`Run Now`をクリックします。

##### **データセットのマテリアライゼーションスケジュールを修正する (Modify a dataset materialization schedule)**
データセットのマテリアライゼーションスケジュールに変更を加えるには：
1.  データセットを開き、`Materialization`タブを選択します。
2.  `Schedule`セクションで、`More` > `Edit Schedule`をクリックします。
3.  新しいスケジュールを定義します。
4.  `Save`をクリックします。
マテリアライゼーションスケジュールは直ちに変更されます。次のマテリアライゼーションは、次のスケジュールされた時刻に行われます。

##### **データセットのマテリアライゼーションスケジュールを削除する (Delete a dataset materialization schedule)**
データセットのマテリアライゼーションスケジュールを削除し、マテリアライズされたデータを接続されたデータプラットフォームから削除するには：
1.  データセットを開き、`Materialization`タブを選択します。
2.  `Schedule`セクションで、`More` > `Remove Schedule`をクリックします。
3.  表示される確認画面で、`Remove`を選択します。
Sigmaは自動的にウェアハウスからマテリアライズされたテーブルを削除します。テーブルが削除されるまで最大24時間かかることがあります。

#### 5-4-1-4. バージョンタグ付きデータモデルのマテリアライゼーションをスケジュールする (Schedule materialization for a version-tagged data model)

一つ以上のタグ付きバージョンを持つデータモデルがある場合、データモデルの各バージョンに対して[マテリアライゼーション](https://help.sigmacomputing.com/docs/about-materialization)スケジュールを設定できます。例えば、「testing」と「production」のタグ付きバージョンのデータモデルがある場合、各タグのデータ要素に対してマテリアライゼーションをスケジュールでき、これにより、そのタグ付きバージョンのデータモデルに依存する下流の要素のパフォーマンスを向上させることができます。

バージョンタグ付きデータモデルの要素のマテリアライゼーションをスケジュールする際には、[マテリアライゼーションのベストプラクティス](https://help.sigmacomputing.com/docs/about-materialization#best-practices-for-materialization)が引き続き適用されます。マテリアライゼーションのスケジューリングに関する詳細は、「[データモデルまたはワークブックのマテリアライゼーションをスケジュールする](https://help.sigmacomputing.com/docs/schedule-materialization-for-a-data-model-or-workbook)」を参照してください。

##### **要件 (Requirements)**
* この機能を使用するには、[データをマテリアライズする権限](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を持つアカウントタイプを割り当てられている必要があります。
* データ要素をマテリアライズするには、データソースの接続で書き込みアクセスが有効になっている必要があります。

##### **タグ付きデータモデルのマテリアライゼーションをスケジュールする (Schedule materialization for a tagged data model)**
少なくとも一つのタグ付きバージョンを持つデータモデルについて、タグ付きバージョンの一つ以上のデータ要素のマテリアライゼーションをスケジュールします。データモデルの異なるタグ付きバージョン間で同じデータ要素のマテリアライゼーションをスケジュールしたい場合は、各タグ付きバージョンに対してスケジュールを作成します。

1.  データモデルを開きます。
2.  ドキュメントヘッダーで、更新データボタンの隣にある`More options` > `Materialization schedule...`をクリックします。
3.  `Materialization`モーダルで、`+ New schedule`をクリックします。マテリアライゼーションスケジュールがない場合は、`Add schedule`をクリックします。
    > 💡
    > 代わりに既存のスケジュールを複製するには、複製したいスケジュールを探し、`More` > `Duplicate schedule`を選択します。
4.  `Version`で、 を選択してバージョンを修正し、ドロップダウンでスケジュールを適用するバージョンタグを選択します。
5.  `Elements`で、スケジュールにデータ要素を追加します。公開バージョンまたはデータモデルの別のタグ付きバージョンでマテリアライズされているのと同じ要素をタグ付きバージョンでマテリアライズするには、`+ Add element`を選択し、`Copy elements from schedule of other versions`を選択します。
6.  スケジュールの頻度を設定します。
    * (任意) `Daily`のドロップダウンを選択し、`Weekly`, `Monthly`, または`Custom`を選択します。
    * `Daily`の場合、`Once a day`または`Multiple times`を選択します。
    * `Weekly`の場合、マテリアライゼーションジョブを実行する曜日を選択し、`Once a day`または`Multiple times`を選択します。
    * `Monthly`の場合、マテリアライゼーションジョブを実行する月の日と時刻を選択します。
    * `Custom`の場合、cron構文を使用してスケジュールを指定します。
    * `Multiple times`を選択した場合は、頻度を指定します。
    * (任意) ドロップダウンメニューを使用して、デフォルトのスケジュールタイムゾーンを調整します。
7.  スケジュールを保存します。

> 📘
> タグをデータモデルの新しいバージョンに昇格させる（例えば、古いバージョンのデータモデルから最新の公開バージョンにタグを移動するなど）と、新しいマテリアライゼーションの実行が開始されます。新しくタグ付けされたバージョンのマテリアライゼーションが実行されている間は、以前にタグ付けされたバージョンのデータモデルのマテリアライズされたデータが使用されます。

#### 5-4-2-1. パフォーマンス向上のためのベストプラクティス (Best practices for improved performance)

このドキュメントでは、パフォーマンスに関連するいくつかのベストプラクティスを集めて、検討のために提供します。

##### **データセットを使用してクエリ負荷を削減する (Use datasets to reduce query loads)**
Sigmaはデータセットを使用して、データ定義を一元化し、ワークブックにソースデータを提供します。データセットの使用に関する詳細は、「[Data modeling In Sigma](https://help.sigmacomputing.com/docs/datasets)」および「[Data modeling tutorial](https://help.sigmacomputing.com/docs/tutorial-data-modeling-with-datasets)」を参照してください。

データセットレベルでフィルターを使用することにより、ワークブックのクエリで返される不要なデータの量を削減します。フィルターは、制限しすぎることなく無関係なデータを削減します。最も関連性の高いデータのみを表示することで、インサイト発見のプロセスがはるかに速くなります。マテリアライゼーションと組み合わせると、クエリの実行も速くなります。

* **データセットの時間範囲フィルター (Dataset time range filters)**
    相対日付フィルターを使用して、Sigmaのクエリが特定の時間範囲のデータのみを返すようにします。詳細は、「[Add relative date filters](https://help.sigmacomputing.com/docs/dataset-filters#add-relative-date-filters)」および「[Dataset filters](https://help.sigmacomputing.com/docs/dataset-filters)」を参照してください。
* **データセットパラメータ (Dataset parameters)**
    データセットパラメータを作成し、ワークシートで使用して、データが必要なものだけにフィルタリングされるようにします。詳細は、「[Dataset parameters](https://help.sigmacomputing.com/docs/dataset-parameters)」を参照してください。

##### **データセットとワークブック要素をマテリアライズしてコンピューティングコストを削減する (Materialize datasets and workbook elements to reduce compute costs)**
マテリアライゼーションを使用すると、データセットとワークブック要素をテーブルとしてウェアハウスに書き戻すことができ、これによりコンピューティングコストを削減できます。マテリアライゼーションは、データウェアハウスがデータセットを要素または下流のSigma分析で使用する際に再計算を回避できるようにすることで、クエリのパフォーマンスを向上させます。詳細は、「[Materialization](https://help.sigmacomputing.com/docs/about-materialization)」を参照してください。

##### **CDWでクエリキャッシュを使用する (Use a query cache in the CDW)**
一部のクラウドデータウェアハウス（CDW）には、Sigmaが追加のコンピューティングコストを発生させることなくクエリ結果を取得するために使用できるクエリ結果キャッシュがあります。これにより、パフォーマンスが向上します。詳細は、「[Set a cache duration](https://help.sigmacomputing.com/docs/set-a-cache-duration)」を参照してください。

##### **ワークブックのパフォーマンスを向上させるためのその他のヒント (More tips for improving workbook performance)**
過剰な結合、繰り返されるロジック、未使用のデータ、フィルターの過負荷は、ワークブックを遅くする可能性があります。パフォーマンスのヒントについては、Sigmaコミュニティの「[How to improve workbook performance](https://community.sigmacomputing.com/dashboards-and-workbooks/how-to-improve-workbook-performance-224)」を参照してください。

#### 5-4-2-2. ウェアハウスビューの作成と管理 (Create and manage warehouse views)

ウェアハウスビューは、あなたのデータプラットフォームに保存される仮想テーブルです。テーブル、ピボットテーブル、入力テーブル、およびチャートからウェアハウスビューを作成し、Sigmaまたはあなたのデータエコシステム内の他の任意のアプリケーションを使用してそれらにクエリを実行できます。ウェアハウスビューはクエリを簡素化し、関連性のある最新のデータサブセットをデータプラットフォームから直接取得することを可能にします。

このドキュメントでは、ワークブックとデータモデルでウェアハウスビューを作成および管理する方法について説明します。管理者ポータルの `Warehouse Views` ページに関する情報については、「[Review warehouse view details](https://help.sigmacomputing.com/docs/review-warehouse-view-details)」を参照してください。

> 📘
> この機能は、すべてのデータプラットフォーム接続でサポートされているわけではありません。あなたの接続がサポートしているかを確認するには、「[Supported data platforms and feature compatibility](https://help.sigmacomputing.com/docs/region-and-feature-support)」を参照してください。

##### **システムとユーザー要件 (System and user requirements)**
ウェアハウスビューを作成および管理する機能には、以下が必要です。
* 要素のデータソースは、[書き込みアクセス](https://help.sigmacomputing.com/docs/set-up-write-access)が有効になっている接続からデータを取得する必要があります。
* `Create warehouse views` 権限が有効になっている[アカウントタイプ](https://help.sigmacomputing.com/docs/account-type-and-license-overview)を割り当てられている必要があります。
* あなたはワークブックまたはデータモデルの所有者であるか、そのワークブックまたはデータモデルに対する `Can edit` [アクセス権](https://help.sigmacomputing.com/docs/share-a-workbook)を付与されている必要があります。

##### **ウェアハウスビューについて (About warehouse views)**
データベーステーブルにデータを保存する代わりに、ウェアハウスビューは、Sigmaの個々のデータ要素または入力テーブルによって定義された特定のクエリロジックを表現するSQLステートメントを保存します。

ウェアハウスビューを作成すると、あなたのデータプラットフォームとSigmaの間にライブリンクが確立されます。ビューはデータ要素または入力テーブルを信頼できる唯一の情報源（source of truth）として参照し、要素の基盤となるデータの最新バージョンを反映するように自動的に更新されます。

ウェアハウスビューはデータプラットフォームに直接クエリを実行するため、マテリアライゼーションとは動作が異なります。しかし、マテリアライズされた要素からウェアハウスビューを作成することもでき、その場合、ビューは要素のマテリアライズされた基盤となるデータテーブルにクエリを実行します。

##### **ウェアハウスビューについて (About warehouse views)**
データベーステーブルにデータを保存する代わりに、ウェアハウスビューは、Sigmaの個々のデータ要素または入力テーブルによって定義された特定のクエリロジックを表現するSQLステートメントを保存します。

ウェアハウスビューを作成すると、あなたのデータプラットフォームとSigmaの間にライブリンクが確立されます。ビューはデータ要素または入力テーブルを信頼できる唯一の情報源（source of truth）として参照し、要素の基盤となるデータの最新バージョンを反映するように自動的に更新されます。

ウェアハウスビューはデータプラットフォームに直接クエリを実行するため、マテリアライゼーションとは動作が異なります。しかし、マテリアライズされた要素からウェアハウスビューを作成することもでき、その場合、ビューは要素のマテリアライズされた基盤となるデータテーブルにクエリを実行します。

##### **ウェアハウスビューの考慮事項 (Warehouse view considerations)**
ウェアハウスビューを作成する際には、以下の制限と制約を考慮してください。
* ウェアハウスビューは、ドキュメントの公開バージョンから作成されます。データモデルまたはワークブックのタグ付きバージョンからウェアハウスビューを作成することはできません。ワークブックのカスタムビューと保存済みビューもサポートされていません。ドラフトでウェアハウスビューが作成された場合、以下のいずれかの結果となります。
    * 要素がドラフトにのみ存在する場合、Sigmaはワークブックまたはデータモデルが公開され、要素が公開バージョンに存在するときにビューを作成します。
    * 要素が公開バージョンに存在するが、ドラフトに未保存の変更が含まれている場合、Sigmaは要素の公開バージョンに基づいてビューを作成します。これはドラフトのデータと一致しない可能性があります。
    * 要素が公開バージョンに存在し、ドラフトに未保存の変更がない場合、Sigmaは要素の公開バージョンに基づいてビューを作成します。これはドラフトのデータと一致します。
* 以下の動的な条件はサポートされていません。
    * **要素内でパラメータとして参照されるコントロール値:** コントロール値は、クエリがユーザー入力に依存するため、要素のSQLステートメントで明示的に定義されません。
    * **相対日付フィルター:** 相対日付フィルター（`Last`, `Next`, `Current`など）は、要素のSQLステートメントで明示的に定義できない現在の日付基準に依存します。
* グループ化されたテーブルからウェアハウスビューを作成する場合、ウェアハウスビューに使用するグルーピングレベルを定義することはできません。
* データ要素に[列レベルのセキュリティ](https://help.sigmacomputing.com/docs/column-level-security)が含まれている場合、ウェアハウスビューを作成することはできません。
* データ要素が[転置](https://help.sigmacomputing.com/docs/transpose-a-table)されている場合、ウェアハウスビューを作成することはできません。

##### **ビューを作成する (Create a view)**
ウェアハウスビューを作成するには、以下を実行します。
1.  公開済みのワークブックまたはデータモデルを開き、ウェアハウスビューを作成したい要素を探します。
2.  要素ツールバーで、`More` をクリックして要素メニューを開き、`Advanced options` > `Create warehouse view` を選択します。
3.  `Create Warehouse View` モーダルで、Sigmaはビューの名前を自動生成します。必要に応じて名前を編集し、`Create` をクリックします。この名前は、データプラットフォームにビューを保存する際にも使用されます。

Sigmaはビューが正常に作成されると通知します。また、要素ツールバーでステータスをプレビューしたり、`View warehouse view info` をクリックしてビューの詳細を確認したりすることもできます。
> 📘
> Sigmaがビューを作成した後、要素に適用されたフィルターやその他の変更は、ワークブックが再公開されたときにのみビューに保存されます。

要素ごとに作成できるウェアハウスビューは1つだけです。同じデータの複数のビューを作成する必要がある場合は、要素を複製し、必要に応じてデータを調整して、別のウェアハウスビューを作成できます。

Sigmaはビューが正常に作成されると通知します。また、要素ツールバーでステータスをプレビューしたり、`View warehouse view info` をクリックしてビューの詳細を確認したりすることもできます。
> 📘
> Sigmaがビューを作成した後、要素に適用されたフィルターやその他の変更は、ワークブックが再公開されたときにのみビューに保存されます。

要素ごとに作成できるウェアハウスビューは1つだけです。同じデータの複数のビューを作成する必要がある場合は、要素を複製し、必要に応じてデータを調整して、別のウェアハウスビューを作成できます。

##### **ビューの名前を変更する (Rename a view)**
ウェアハウスビューの名前を変更するには、以下を実行します。
1.  ワークブックまたはデータモデルを開き、名前を変更したいウェアハウスビューに関連付けられた要素を探します。
2.  要素ツールバーで、`More`をクリックして要素メニューを開き、`Advanced options` > `Manage warehouse view`を選択します。
3.  `Manage Warehouse View`モーダルで、`Name`フィールドに新しい名前を入力し、`Update`をクリックします。
     ウェアハウスビューの名前とパスが更新されます。

要素ツールバーでウェアハウスビューの更新ステータスをプレビューするか、`View warehouse view info`をクリックしてビューの詳細を確認できます。「[ウェアハウスビューのステータス](#warehouse-view-statuses)」を参照してください。
##### **ビューを削除する (Delete a view)**
ウェアハウスビューを削除するには、以下を実行します。
1.  ワークブックまたはデータモデルを開き、削除したいウェアハウスビューに関連付けられた要素を探します。
2.  要素ツールバーで、`More` > `Advanced options` > `Manage warehouse view` を選択します。
3.  `Manage Warehouse View` モーダルで、`Delete` をクリックします。
4.  `Confirm Delete` モーダルで、`Delete` をクリックします。

##### **ウェアハウスビューのステータス (Warehouse view statuses)**
ウェアハウスビューには以下のステータスが適用されます。

| ステータス | 説明 |
| :--- | :--- |
| **Pending** | Sigmaはワークブックが公開されるとビューを作成または更新します。|
| **Successful** | Sigmaはビューの作成または更新に成功しました。|
| **In Progress** | Sigmaは現在ビューを作成または更新中です。|
| **Failed** | ビューの作成または更新ができませんでした。失敗ステータスの原因を表示するには、ウェアハウスビュー詳細で`Failed`ステータスインジケータにカーソルを合わせます。|

##### **トラブルシューティング (Troubleshooting)**
特定の要素に対してウェアハウスビューを作成できない場合は、以下のいずれかが真であるかを確認してください。
* 現在、探索（exploration）で作業している。ウェアハウスビューを作成する前に、探索をワークブックとして保存する必要があります。
* 別のウェアハウスビューをソースとするデータ要素または入力テーブルに対してウェアハウスビューを作成しようとしている。ビューは他のビューをクエリできません。
* 要素データが[コントロール値をパラメータとして参照している](https://help.sigmacomputing.com/docs/reference-workbook-control-values-in-sql-statements)。
* 要素タイプが現在ウェアハウスビューをサポートしていない。

### 5-5. クエリの調査

#### 5-5-1. ワークブックとデータモデルのクエリを調査する (Examine workbook and data model queries)

ワークブックまたはデータモデルを開くと、Sigmaは最適化されたSQLクエリを生成・実行し、接続されたデータプラットフォームからデータを取得します。クエリ結果は、安全にあなたのウェブブラウザに返されます。

ワークブックまたはデータモデルの**クエリ履歴**を開くことで、ブラウザセッション中に実行されたクエリの構文やその他の詳細を確認できます。データセットのクエリ履歴に関する詳細は、「[データセットのクエリを調査する](https://help.sigmacomputing.com/docs/examine-dataset-queries)」を参照してください。

**クエリ履歴**は、ユーザーセッション中にワークブックから実行された最近のクエリの概要を表示し、クエリのランタイムや現在のステータスを含みます。個々のクエリをさらに深く掘り下げて、基盤となるSQLを表示したり、トラブルシューティングのためのリクエストIDを収集したり、エラーを調査したりすることができます。

##### **最近のクエリを表示する (View recent queries)**
クエリ履歴は、既存のセッション中にワークブックまたはデータモデルから実行された最近のクエリを表示します。ドキュメントの個々のクエリのリストは、各クエリの詳細を自動的に表示します。

1.  ドキュメントヘッダーで、更新データボタンの隣にある`More options`をクリックします。
2.  `Query history`を選択します。

##### **ブラウザの計算を表示する (View browser calculations)**
一部のクエリはデータプラットフォームから結果を返し、その他はデータプラットフォームの結果キャッシュから、さらに他の結果はブラウザキャッシュから返されます。
デフォルトでは、ブラウザで実行された計算はデータプラットフォームに送信されないため、クエリ履歴から非表示になっています。ブラウザの計算履歴を表示するには、以下を実行します。

1.  ドキュメントヘッダーで、更新データボタンの隣にある`More options`をクリックします。
2.  `Query history`を選択します。
3.  `Query history`モーダルの上部で、`View browser calculations`トグルをオンにします。
4.  `Execution Path`列で`Browser`エントリを確認します。

##### **個々のクエリ詳細を表示する (View individual query details)**
生成されたSQL、完全な実行時間、トラブルシューティング用のリクエストIDなど、個々のクエリの詳細を表示するには、以下を実行します。
1.  ドキュメントヘッダーで、更新データボタンの隣にある`More options`をクリックします。
2.  `Query history`を選択します。
3.  調査したいクエリを選択します。Sigmaは選択されたクエリの詳細を表示します。
    * 要素名を選択して、クエリが実行されたデータ要素を開きます。
    * 実行時間と期間を確認します。
    * 生成されたSQLを表示およびコピーします。
    * 失敗したクエリの場合、エラーメッセージを確認します。
    * トラブルシューティングの際にSigmaサポートと共有するためのリクエストIDをコピーします。

##### **クエリを一時停止および再開する (Pause and resume queries)**
データプラットフォームに対して自動的にクエリを実行せずにドキュメントに変更を加えるには、クエリを一時停止します。
1.  ドキュメントヘッダーで、更新データボタンの隣にある`More options`をクリックします。
2.  `Pause queries`を選択します。
クエリを一時停止した後にクエリの実行を再開するには、`Resume queries`を選択します。

##### **クエリ履歴のリファレンス (Query history reference)**
ステータス、実行時間、リクエストタイプ、および実行パスの詳細については、以下のセクションを参照してください。

* **クエリステータスタイプ (Query status types)**

| ステータス | 詳細 |
| :--- | :--- |
| **Completed** | クエリは正常に実行されました。|
| **Running** | クエリは現在実行中です。デフォルトでは、Sigmaはクエリのタイムアウトを120秒（2分）に設定しています。 |
| **Errored** | クエリ実行中にエラーが発生しました。行を選択してクエリ詳細とエラーメッセージを表示します。 |
| **Paused** | ドキュメント上のクエリは一時停止しています。クエリの実行を再開して最新データを取得するには、ドキュメントヘッダーの`Refresh queries`をクリックします。 |
| **Canceled** | クエリはキャンセルされました。これは、クエリが終了する前に別のドキュメントタブに切り替えた場合や、クエリが終了する前にドキュメントに変更が加えられた場合に発生する可能性があります。 |

* **クエリ実行時間 (Query run time)**
    正常に完了したクエリとタイムアウトしたクエリに対して、詳細なクエリ実行時間の内訳が利用可能です。クエリの実行時間は、ネットワークトラフィック、キューの遅延、またはデータプラットフォームの処理時間によって変動する可能性があります。実行時間の内訳により、クエリが遅延したかどうか、どの段階で遅延したかを確認できます。

    実行時間は3つの部分に分かれています。
    * **Queue duration (キュー期間):** クエリがデータプラットフォームに送信される前にSigmaのキューで待機する時間。特定のデータプラットフォームでは、Sigmaキューはデータプラットフォームに送信される同時リクエストの数を制限するために使用されます。
    * **Sigma runtime (Sigmaランタイム):** キューの期間とデータプラットフォームの時間を除く、Sigmaがクエリを処理するのにかかる時間。失敗したクエリやキャンセルされたクエリは、クエリがデータプラットフォームのタイムアウトにより失敗した場合でも、すべての実行時間をSigmaに帰属させます。
    * **Warehouse runtime (ウェアハウスランタイム):** Sigmaがデータプラットフォームにリクエストを送信してから応答を受け取るまでの時間。これは、おおよそデータプラットフォームがクエリの実行に費やした時間と同等です。
    * **Result fetch time (結果取得時間):** Sigmaがデータプラットフォームから結果を取得するのにかかる時間。
    * **Details unavailable (詳細利用不可):** PDFダウンロードなどの一部のエクスポートクエリでは、実行時間の内訳詳細は利用できません。

    未完了のクエリやダウンロード/エクスポートリクエストは、詳細な実行時間の内訳を表示しません。
    特定のクエリの実行時間（例えば、キューイング時間が著しく長いなど）に懸念がある場合は、Sigmaサポートにお問い合わせください。

* **クエリリクエストタイプ (Query request types)**
    Sigmaは、異なるタイプの情報を取得するために、データプラットフォームに対して異なるタイプの最適化されたクエリを作成します。
    ドキュメントのクエリ履歴を調査する際、以下のようなリクエストタイプが表示されることがあります。

| リクエストタイプ | 詳細 |
| :--- | :--- |
| **Data Prefetch Query** | 表示されているデータ要素によって使用されるデータソースを取得します。<br>例えば、10個の表示されているKPI要素のデータを取得するために10個の個別のクエリを実行する代わりに、1つのクエリを実行してデータソースを取得します。|
| **<Element name> <Element type>**<br>例：<br>EVENTS Visualization: bar | 要素のデータを取得します。|
| **SQL Preview** | データモデルの概要を表示するために使用されるデータを取得します。|
| **Filter Top Values** | 列の詳細を表示する際や、データ要素のリストフィルターを開く際など、トップの値を取得します。|
| **<Element name> Count Rows** | 列の詳細を取得する際や、データモデルの概要で折りたたまれた要素を表示する際など、要素の行数を取得します。|
| **<Element name> Column statistics** | ワークブックまたはデータモデルの列の詳細を表示する際など、列の統計情報を取得します。|
| **Export Query** | スケジュールされた、またはオンデマンドのワークブック、ページ、または要素のエクスポートを実行するために最新のデータを取得します。|
| **<Element name> Export Query** | CSVやJSONなどの生データ形式で要素をダウンロードするために最新のデータを取得します。|

* **クエリ実行パス詳細 (Query execution path details)**
    Sigmaで利用可能なデータに応じて、クエリの実行パスは異なる場合があります。

| 実行パス | 詳細 |
| :--- | :--- |
| **Warehouse** | 最適化されたSQLクエリでデータプラットフォームを直接クエリしてデータを取得します。|
| **Warehouse (cache)** | 特定のデータプラットフォームで利用可能。クエリIDを使用して、データプラットフォームのクエリ結果キャッシュからデータを取得するクエリを実行します。詳細は、「[Set a query ID cache duration](https://help.sigmacomputing.com/docs/set-a-query-id-cache-duration)」を参照してください。|
| **Warehouse (materialized)** | マテリアライズされたテーブルにクエリを実行してデータを取得します。「[About materialization](https://help.sigmacomputing.com/docs/about-materialization)」を参照してください。|
| **Browser** | ブラウザキャッシュからデータを取得し、アルファクエリを使用して計算を実行します。詳細は、「[Caching and data freshness](https://help.sigmacomputing.com/docs/caching-and-data-freshness)」を参照してください。|

詳細は、「[Caching and data freshness](https://help.sigmacomputing.com/docs/caching-and-data-freshness)」を参照してください。

### 5-5-2. データセットのクエリを調査する (Examine dataset queries)

#### **最近のクエリを表示する (View recent queries)**
クエリ履歴モーダルは、既存のセッション内に開いているドキュメントから実行された最近のクエリを表示します。
あなたのドキュメントの個々のクエリリストは、各クエリのステータス、アクションタイプ、開始時刻、実行時間を自動的に表示します。

1.  データセットのワークシートタブを開きます。
2.  データセットのツールバーの一番左にある更新ボタンの隣にあるキャレットアイコンをクリックします。
3.  `Query history...`をクリックします。

#### **個々のクエリを表示する (View an individual query)**
1.  データセットの`Worksheet`タブを開きます。
2.  データセットのツールバーの一番左にある更新ボタンの隣にあるキャレットアイコンをクリックします。
3.  `Query history...`をクリックします。
4.  調査したいクエリをクリックします。
5.  クエリ詳細ビューを探索します：
    * Sigmaが生成したSQLを表示およびコピーします。
    * クエリが失敗した場合、エラーも`Query Details`の下に表示されます。

#### **クエリステータスタイプ (Query status types)**
これらはSigma内で可能なクエリステータスタイプです。

| | |
| :--- | :--- |
| **Completed** | あなたのクエリは正常に実行されました！ |
| **Running** | あなたのクエリは現在実行中です。 |
| **Errored** | 何か問題があります。クエリ詳細ビューを開いてエラーメッセージを確認してください。 |
| **Paused** | ドキュメント上のクエリは一時停止しています。クエリを再開するには、ドキュメントツールバーの`Play`をクリックしてください。 |
| **Canceled** | クエリはキャンセルされました。これは、クエリが実行される前にドキュメントに追加の変更が加えられた場合に発生する可能性があります。この状況では、Sigmaは新しいクエリのみを実行します。 |

> 📘
> デフォルトでは、Sigmaはクエリのタイムアウトを120秒（2分）に設定しています。組織の管理者は、接続ごとにこれをカスタマイズするオプションがあります。

#### **クエリ実行時間の内訳 (Query runtime breakdown)**
正常に完了したクエリとタイムアウトしたクエリに対して、詳細なクエリ実行時間の内訳が利用可能です。クエリの実行時間は、ネットワークトラフィック、キューの遅延、またはデータウェアハウスの処理時間によって変動する可能性があります。Sigmaの実行時間の内訳により、クエリが遅延したかどうか、いつ遅延したかを確認できます。

実行時間は3つの部分に分かれています。
| | |
| :--- | :--- |
| **Queue duration** | クエリがウェアハウスに送信される前にSigmaのキューで待機する時間。 |
| **Sigma runtime** | キューの期間とウェアハウスの時間を除く、Sigmaがクエリを処理するのにかかる時間。 |
| **Warehouse runtime**| Sigmaがデータウェアハウスにリクエストを送信してから応答を受け取るまでの時間。これは、おおよそウェアハウスがクエリの実行に費やした時間です。 |

未完了のクエリは、詳細な実行時間の内訳を表示しません。この機能は、ダウンロード/エクスポートリクエストでも利用できません。

#### **クエリを一時停止および再開する (Pause and resume queries)**
ウェアハウスに対して自動的にクエリを実行せずにドキュメントに変更を加えるために、クエリを一時停止できます。

1.  データセットの`Worksheet`タブを開きます。
2.  データセットのツールバーの一番左にある更新/再生ボタンの隣にあるキャレットアイコンをクリックします。
3.  `Pause queries`または`Resume queries`をクリックします。
   
### 5-5-3. クエリIDキャッシュ期間を設定する (Set a query ID cache duration)

一部のクラウドデータウェアハウス（CDW）には、Sigmaが追加のコンピューティングコストを発生させることなくクエリ結果を取得するために使用できるクエリ結果キャッシュがあります。CDWで利用可能な場合、SigmaはクエリIDを使用してキャッシュされたデータにアクセスします。これにより、パフォーマンスが向上します。

ワークブックには、クエリIDのキャッシュ期間、つまり存続期間（TTL）の設定があります。デフォルトの期間は10分です。詳細については、「[Caching and data freshness](https://help.sigmacomputing.com/docs/caching-and-data-freshness)」を参照してください。

実際のクエリ結果はSigmaではなく、CDWにキャッシュされます。通常、CDWキャッシュは結果のコピーの形をとり、24時間保存されます。
TTL期間内にソースデータが変更された場合、キャッシュされた結果は無関係または不正確なデータを反映します。

クエリの結果を返そうとする場合、`Cache duration`設定を使用して、結果キャッシュが特定の分数だけ古いことを指定できます。

#### **要件 (Requirements)**
* この機能は、SnowflakeやBigQueryを含む、結果キャッシュをサポートするCDWでのみ利用可能です。
* ワークブックのクエリIDキャッシュ期間を設定するには、組織の`Admin`である必要があります。

#### **クエリキャッシュID期間を設定する (Set a query cache ID duration)**
1.  ワークブックのヘッダーにある更新ボタンの右側にあるキャレット（▼）ボタンをクリックします。
2.  `Data refresh`を選択します。
    `Data Refresh Settings`モーダルが開きます。
3.  `Cache duration`の下で、分または時間で期間を設定します。
4.  `Save`をクリックします。

### 5-5-4. キャッシュとデータの鮮度 (Caching and data freshness)

ワークブックまたはデータモデルを開くと、Sigmaは最適化されたSQLクエリを生成・実行し、接続されたデータプラットフォームからデータを取得します。Sigmaはあなたのデータを保存せず、ブラウザのキャッシングとウェアハウスレベルのキャッシングを使用して、ウェアハウスのオーバーヘッドを削減しつつ、新鮮なデータを保証します。

#### **Sigmaがウェアハウスのオーバーヘッドを削減する方法 (How Sigma reduces warehouse overhead)**
データ要素が更新されると、Sigmaはウェアハウスへのオーバーヘッドを削減しようと試みます。Sigmaが従うステップは以下の通りです。
1.  ブラウザキャッシュを確認する
2.  アルファクエリを試す
3.  CDWの結果IDキャッシュを試す（一部のCDWでのみ利用可能）
4.  ウェアハウスに再度クエリを実行する

> 🚩
> 手動更新またはスケジュールされた更新は、すべてのキャッシングオプションをバイパスします。「[Manage workbook refresh options](https://help.sigmacomputing.com/docs/manage-workbook-refresh-options)」を参照してください。

どのクエリがどこで実行されているかの詳細については、ワークブック、データモデル、またはデータセットのクエリ履歴を確認してください。「[Examine workbook and data model queries](https://help.sigmacomputing.com/docs/examine-workbook-queries)」および「[Examine dataset queries](https://help.sigmacomputing.com/docs/examine-dataset-queries)」を参照してください。

##### **ブラウザキャッシュを確認する (Check browser cache)**
ブラウザキャッシュは、ブラウザですぐにアクセスできるデータを占めます。キャッシュは空であるため、最初にワークブックまたはデータモデルを開いたときにはブラウザキャッシュは利用できませんが、変更を加えるにつれて、Sigmaは可能な場合に結果を表示するために自動的にブラウザキャッシュを使用します。
データ要素に変更を加えると、Sigmaはまずブラウザに既にある既存のデータが、更新された要素でまだ機能するかどうかを確認します。
これは、以下のような場合に発生する可能性があります。
* 列の名前が変更されたり、移動されたりした場合

##### **アルファクエリを試す (Try alpha query)**
ブラウザ内のデータを直接使用できない場合、Sigmaはブラウザ内の既存のデータを使用して新しい値を再計算できるかどうかを確認します。
これは、以下のような場合に発生する可能性があります。
* 新しい集計列が追加された場合

##### **クエリIDキャッシュを試す (Try query ID cache)**
クエリキャッシュは、SnowflakeやBigQueryのように、データウェアハウスが結果キャッシングをサポートしている場合にのみ使用されます。
これは、以下のような場合に発生する可能性があります。
* データを再グループ化する場合

Sigmaはクエリ結果を保存せず、ウェアハウスから返されたクエリIDのみを保存し、そのIDを使用してデータウェアハウスのキャッシュから結果を取得します。

##### **クエリIDキャッシュ期間を設定する (Set a query ID cache duration)**
SnowflakeやBigQueryなど、一部のデータプラットフォームは、クエリIDを使用してキャッシュから過去のクエリの結果を返すことをサポートしています。
ワークブックのキャッシュ期間、つまり存続期間（TTL）とは、SigmaがクエリIDを使用してCDWの結果キャッシュから結果を取得しようと試みる期間を指します。
SigmaがクエリIDキャッシュをクエリに使用できると判断し、CDWに対して最後にクエリが実行された時刻がクエリIDキャッシュ期間内である場合、Sigmaはウェアハウスに対してクエリを再実行しようとはしません。
ウェアハウスに対して最後にクエリが実行された時刻がクエリIDキャッシュ期間外である場合、SigmaはクエリIDを使用してCDWの結果キャッシュから結果を取得してワークブックをレンダリングし、並行してウェアハウスに対してクエリを実行します。最新の結果がウェアハウスから返されると、Sigmaはワークブック要素を更新します。
TTLの変更に関する情報については、「[Set a query ID cache duration](https://help.sigmacomputing.com/docs/set-a-query-id-cache-duration)」を参照してください。

##### **手動更新と更新スケジュール (Manual refresh and refresh schedules)**
必要に応じて、更新スケジュールを使用してください。詳細は「[workbook refresh options](https://help.sigmacomputing.com/docs/manage-workbook-refresh-options)」を参照してください。
> 🚩
> Sigmaはクエリ結果を保存せず、ウェアハウスから返されたクエリIDのみを保存します。すべてのデータ更新は、ウェアハウス内のデータに再度クエリを実行します。自動更新を設定すると、接続に負荷がかかり、多額のウェアハウスコストが発生する可能性があります。

