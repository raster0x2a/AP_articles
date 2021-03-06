# 応用情報技術者試験のセキュリティ分野における用語メモ

## OSコマンドインジェクション

Webアプリにおいて、閲覧者の入力を利用しシェル呼び出しやOSコマンドを実行する機能で、コマンドやオプションなどの文字列を埋め込み、不正な操作を行うこと。

## SQLインジェクション

Webアプリにおいて、閲覧者の入力を利用しSQLクエリを実行する機能で、SQL文などの文字列を埋め込み、不正なクエリを実行させる攻撃手法。

## クロスサイトスクリプティング(XSS)

動的にWebページを生成するWebアプリにおいて、悪意のあるスクリプトを混入させることで、攻撃者が仕込んだ操作を実行させたり別のサイトを横断してユーザのクッキーや個人情報を盗んだりする攻撃手法。

## セッションハイジャック

ブラウザとWebサーバ間における通信で、CookieやセッションIDなどのセッション情報を盗むことで、対象セッションを乗っ取る攻撃。

## バインド機構

SQLインジェクションの対策として、プログラム内のSQL文のうち変数部分にプレースホルダと呼ばれる記号を置き、実行時に実際の値を割り当てる仕組み。

## DNSキャッシュポイズニング

DNSサーバに偽の応答をキャッシュさせることで、利用者のアクセスに対し、攻撃者が用意したサーバーに誘導し、フィッシングや送信された情報の窃盗などを図る攻撃。

## レインボー攻撃

ハッシュ値と平文をチェーンによって管理する特殊な逆引き表(レインボーテーブル)を用いて、ハッシュ値からパスワードを特定する攻撃手法。

## ディレクトリトラバーサル

入力文字列を利用してファイル名を要求するシステムに対し、親ディレクトリへの移動(../)などを指定することによって、本来許されないファイルの不正な閲覧・取得を行う攻撃方法。

## ステガノグラフィ

あるデータを画像や音声データなどの他のデータの中に秘密裏に埋め込む技術。電子透かし技術などに応用されている。

## クリプトグラフィ(暗号化)

データを第三者に盗み見られても解読できないようにするため、決まった規則に従ってデータを変換すること。

## TPM

Trusted Platform Module。コンピュータのマザーボードなどに装着される、セキュリティ関連の処理機能を実装した半導体チップ。[RSA暗号](#rsa暗号)の暗号化/復号や鍵ペアの生成、ハッシュ値の計算、デジタル署名の生成・検証などの機能を有す。

## SPF

Sender Policy Framework。SMTPを利用したインターネット電子メールの送受信において送信者のドメインの偽称(なりすまし)を防ぎ、正当性を検証する送信ドメイン認証方式のひとつ。

## SIEM

Security Information and Event Management。セキュリティソフトのひとつで、機器やソフトウェアの動作状況ログを一元的に管理し、保安上の脅威となるインシデントを自動的に検知・分析し、管理者に通知する仕組み。

## UTM

Unified Threat Management、統合脅威管理。ネットワークセキュリティにおいて、不正アクセスやウィルスなどによる脅威からネットワークやサーバーを守るために、ファイアウォール、アンチウィルス、不正侵入検知・防御([IDS](#ids)・IPS)などをひとつに集約して運用する形態。

## 耐タンパ性

タンパ(tamper)は改ざんを意味し、ソフトウェアやハードウェアの内部構造や記録されたデータなどの解析や改変が困難な性質。ICチップにおいて、不正な読み取りを検出すると内部の保存情報を消去する機能などがある。

## SECE

Secure Electronic Commerce Environment。オンライン決済の通信を行う際の国際標準的プロトコルであるSET(Secure Electronics Transaction)を日本独自に拡張したプロトコル。

## インターロック

誤操作や確認不足から機器に生じる誤作動を防止する安全機構。

## ダークネット

インターネット上で到達可能かつ、特定のネットワークに割り当てられていないIPアドレス領域。通常利用では使用されず、[マルウェア](#マルウェア)がIoT機器やサーバなどの攻撃対象を探すために送信するパケットなどが観測される。

## ソーシャルエンジニアリング

ネットワークに侵入するために必要となるパスワードなどの機密情報を、情報通信技術以外の人間の心理的な隙や、行動のミスを利用して盗み出す方法。

## ショルダーハッキング

他人がパスワードや暗証番号を入力しているところを盗み見ること。ソーシャルエンジニアリングの手法のひとつ。

## トラッシング（スカベンジング）

廃棄された光学ディスクやハードディスクなどの記憶媒体などを回収して解析し、機密情報などを探り出すソーシャルエンジニアリングの手法のひとつ。

## マルウェア

不正かつ有害に動作させる意図で作成された悪意のあるソフトウェアや悪質なコードの総称。 [コンピュータウイルス](#コンピュータウイルス)や[ワーム](#ワーム)、[トロイの木馬](#トロイの木馬)などが含まれる。

## コンピュータウイルス

自立的には活動はせず、宿主のプログラムファイルから自身を他のプログラムに複製することで静的に感染する[マルウェア](#マルウェア)の一種。

## ワーム

独立したプログラムであり、自身を複製して他のシステムに感染する[マルウェア](#マルウェア)の一種。

## トロイの木馬

有用なプログラムあるいはデータファイルのように偽装されていながら、その内に[マルウェア](#マルウェア)として機能する部分を隠し持っており、何らかのトリガによりそれが活動するように仕組まれている[マルウェア](#マルウェア)の一種。

## 踏み台攻撃

他者のサーバーやパソコンを乗っ取り、サイバー攻撃や迷惑メールなどに利用して行う攻撃。攻撃元の隠蔽や、発信源を多数動員して行うDDoS攻撃などで利用される。

## ISMS適合性評価制度

Information Security Management System、情報セキュリティマネジメントシステム。組織における情報資産のセキュリティを管理するための枠組みであり、[機密性、完全性、可用性](#情報セキュリティにおける3大要素)を一定の水準で確保するための仕組みが整っていることを認定する制度。

## ISMS認証基準

[ISMS適合性評価制度](#isms適合性評価制度)において、第三者である指定審査機関が事業者の適合性を評価するための認証基準。

## 非公式アプローチ

専門的知識と経験を持つ個人によってリスクを評価する手法。分析者の能力に依存するため、分析の時間や品質に差が出る。

## 詳細リスク分析

組織内の対象となる情報資産に対し、「資産価値」、「脅威」、「脆弱性」、「セキュリティ要件」を識別し、リスクを評価する手法。精度の良い分析結果が得られるが、実施にはコストがかかる。

## ベースラインアプローチ
既存の標準をもとに、組織のベースライン(セキュリティ対策レベル)を策定し、対象となるシステムに一律に適用して簡易的にリスク分析が行える手法。

## 組合せアプローチ

あらかじめ組織にとって重要な情報資産や高いリスクにさらされる情報資産を特定し、リスクが高いと評価された情報資産に対しては[詳細リスク分析](#詳細リスク分析)を優先的に行い、価値が低いと評価された情報資産に対しては[ベースラインアプローチ](#ベースラインアプローチ)を行う手法。

## 情報セキュリティにおける3大要素

- 機密性(Confidentiality)
  
決められた人だけが対象のデータにアクセスできるようにコントロールし、情報漏えいが起こらないようにする能力。
  
- 完全性(Integrity)
  
データを最新かつ正確な状態で維持し、改ざんが行われないようにする能力。

- 可用性(Availability)
  
システムを障害などで**停止させることなく継続して稼働できる**能力。可用性を確保する方法のひとつとして「冗長化」がある。

3つの頭文字をとってCIAとも呼ばれる。

## 情報セキュリティにおける7大要素

[情報セキュリティにおける3大要素](#情報セキュリティにおける3大要素)(機密性、完全性、可用性)に以下の4つを加えたもの。

- 真正性(Authenticity)

利用者、プロセス、システム、情報などが、主張通りであること。なりすましや虚偽入力を防止するために、デジタル署名や二段階認証などの対策がある。

- 責任追跡性(Accountability)

情報資産に行われた操作について、ユーザと動作を一意に特定でき、過去に遡って追跡できること。

- 否認防止(Non-repudiation)

操作が行われた事実や発生した事象を証明でき、後になって否認できないようにすること。デジタル証明の発行などの対策がある。

- 信頼性(Reliability)

システムが持つ**障害への耐性**。平均故障間隔(MTBF)で評価され、平均故障間隔の値が大きければ大きいほど信頼性は高いと言える。
頭文字はCIA+AANRとなる。

## 水飲み場型攻撃

特定の組織の機密情報を狙い、組織のユーザーが普段利用するWebサイトを改ざんし、[マルウェア](#マルウェア)に感染させる標的型攻撃のひとつ。

## ドライブバイダウンロード

ウェブサイトにアクセスしただけで、スパイウェアやランサムウェアなどの不正なプログラムをダウンロードさせ、感染させる攻撃。

## サイバー情報共有イニシアティブ(J-CSIP: Initiative for Cyber Security Information sharing Partnership of Japan)

公的機関である[IPA](#ipa)を情報ハブ(集約点)として、参加組織間で情報共有を行い、高度なサイバー攻撃対策に繋げていく取り組み。

## サイバーレスキュー隊(J-CRAT: Cyber Rescue and Advice Team against targeted attack of Japan)

[IPA](#ipa)によって発足された、標的型サイバー攻撃の被害拡大防止のため、相談を受けた組織の被害の低減と攻撃の連鎖の遮断を支援する活動を行う組織。

## 日本セキュリティオペレーション事業者協議会(ISOG-J: Information Security Operation providers Group Japan)

セキュリティオペレーション技術の向上、オペレータ人材の育成、および関係する組織・団体間の連携を推進するために発足された協議会。

## 線形解読法

暗号化変換の線形近似式を発見することを基本とした一般化された暗号解読手法のひとつ。主にブロック暗号およびストリーム暗号に適用される。

## 差分解読法

入力差分がどのように出力差分に影響を及ぼすか考察することによって、秘密鍵を復元できるような性質を発見する暗号解読手法のひとつ。主にブロック暗号に対して用いられる。

## サイドチャネル攻撃

暗号装置の動作状況を様々な物理的手段で観察あるいは測定することにより、装置内部の情報を取得しようとする暗号解読手法のひとつ。暗号処理時間や電力消費量、電磁波などの外部から得られる情報を利用する。

## パスワードクラック

データ分析によって他人のパスワードを割り出すこと。[ブルートフォース攻撃(総当たり攻撃)](#ブルートフォース攻撃)、辞書攻撃、類推攻撃、リバースブルートフォース攻撃などがある。

## ブルートフォース攻撃

ユーザのアカウント・パスワードを解読するため、使用できる文字種全てのパターンを順に試していく攻撃手法。

## 辞書攻撃

辞書にある単語を利用し、パスワードの割り出しや暗号の解読を行う手法。

## PKI(公開鍵暗号基盤)

Public Key Infrastructure。公開鍵暗号方式や電子署名方式で用いる公開鍵とその公開鍵の持ち主の対応関係を保証するための仕組み。認証局(CA、Certification Authority)という第三者機関を用いて運用される。

## CRL(証明書失効リスト)

Certificate Revocation List。[PKI(公開鍵暗号基盤)](#pki公開鍵暗号基盤)における失効した(信頼できない)公開鍵証明書のリスト。主にPKIを使ったアプリケーションが証明書の有効性を検証するのに使われる。

## スニッフィング

ネットワークを流れるデータパケットを捕らえて内容を解析し、ユーザー名やパスワード、個人情報、クレジットカード番号などの機密情報を不正に入手する攻撃手法。

## サラミ法

不正行為が表面化しない程度に、銀行口座などの多数の資産から少しずつ搾取する行為を指す。ソーセージを薄く切り取るという意味に由来する。

## ウォードライビング

自動車などで移動しながらセキュリティ面において十分に保護されていない無線LANのアクセスポイントを探し出す行為。

## ゼロ知識証明

暗号学において、自分の持っている命題が真であることを伝えるのに、真であること以外の情報を伝えることなく証明できるような証明プロトコルの一種。パワードを直接入力する代わりに、パスワードを知っているという証拠を送信することなどができる。

## ハイブリッド暗号

公開鍵暗号と共通鍵暗号を組み合わせた暗号化方式。公開鍵暗号によって共通鍵暗号の鍵を配送し、共通鍵暗号で伝送内容本体の暗号化を行なう。

## ElGamal暗号

位数が大きな群の離散対数問題が困難であることを安全性の根拠とした**公開鍵暗号**のひとつ。

## 楕円曲線暗号

楕円曲線上の離散対数問題 (EC-DLP) の困難性を安全性の根拠とする暗号のひとつ。主に公開鍵暗号としてデジタル署名に用いられる。

## RSA暗号

桁数が大きい合成数の素因数分解問題が困難であることを安全性の根拠とした公開鍵暗号のひとつ。[SSL/TLS](#ssltls)、[PKI](#pki公開鍵暗号基盤)などで利用されている。(RSAという名前は開発者3名の名前の頭文字に由来する。)

## AES
Advanced Encryption Standard、高度暗号化標準。アメリカ政府がDESに代わる標準規格として策定した共通鍵暗号システム。

## SaaS

Software as a Service。アプリケーションまで含めたソフトウェア全体をインターネット上で提供するサービス。普段オンラインで利用しているサービスのほとんどはこれにあたる。GmailといったメールサービスやGoogleDriveといったクラウドストレージサービスなど。

## PaaS

Platform as a Service。OSやミドルウェアなどアプリケーションが動作するプラットフォームを提供するサービス。AWSのLambdaやGCPのAppEngine、Herokuなど。

## IaaS

Infrastructure as a Service。CPUやメモリ、ストレージ、ネットワークなどのハードウェアやインフラといった個々のリソースを提供するサービス。AWSのEC2やGCPのComputeEngineなど。

## SSL/TLS

Secure Sockets Layer/Transport Layer Security。インターネットにおける通信の暗号化に関するプロトコル。クライアントとサーバ間の通信データを暗号化、通信相手の認証、改竄の検出などの機能を提供する。TLSはSSLの次世代規格であり、現在ではSSLはほとんど利用されていないが、SSLという名称が広く普及しているためまとめてSSLと呼ばれる場合も多い。

## WAF

Web Application Firewall。Webサーバへの外部からの攻撃を検知、防御するシステム。Webサーバとインターネットなど外部との中間に設置され、攻撃を検出した場合アクセスをブロックする。

## クロスサイトリクエストフォージェリ(CSRF)

Webアプリにおいて、偽装したURLを開かせることにより利用者に意図せず特定のサイト上で操作を行わせるもの。DDoS攻撃や、閲覧者の個人データやアカウント情報の漏洩や改竄するためなどに利用される。

## リプレイアタック

利用者の確認に用いられる認証データの送受信を盗聴し、得られたデータをそのまま用いてその利用者になりすます不正アクセスのひとつ。暗号化された内容が分からくても利用できる。

## キーロガー

コンピュータのキーボード操作を常時監視して時系列に記録する装置やソフトウェア。他人のコンピュータの機密情報を盗み取るために不正利用されることがある。

## JPCERT/CC

Japan Computer Emergency Response Team/Coordination Center。コンピュータセキュリティの情報を収集し、インシデント対応の支援、コンピュータセキュリティ関連情報の発信などを行っている一般社団法人。

## 内閣サイバーセキュリティセンター(NISC)

National center of Incident readiness and Strategy for Cybersecurity、内閣サイバーセキュリティセンター。サイバーセキュリティ基本法に基づいて内閣官房に設置された、情報システムに対する不正活動の監視・分析、重大事象の原因究明調査、行政各部に対する監査等を行う機関。

## JIPDEC

Japan Information Processing Development Corporation、一般財団法人日本情報経済社会推進協会。個人情報保護やプライバシー、インターネット上の信頼性確保などの情報産業に関する社会基盤整備を行っている。

## IPA

Information-technology Promotion Agency, Japan、独立行政法人情報処理推進機構。情報セキュリティ対策の強化や優れたIT人材の育成に関する活動など、ソフトウェア分野における競争力の総合的な強化を図っている。ITパスポート試験や応用情報技術者試験などを含む情報処理技術者試験も、IPAによって主催・運営されている。

## IDS

Intrusion detection system、侵入検知システム。ネットワーク上を流れるパケットを監視し、不正アクセスなどを検知するシステム。防御の対象により、ネットワーク全体を一括して監視するNIDS(ネットワーク型IDS)と、一台の機器を監視するHIDS(ホスト型IDS)に大別される。

## ペネトレーションテスト

ネットワークに接続されているコンピュータシステムに対し、実際に既知の技術を用いて侵入を試みることで、システムに脆弱性がないかどうかテストする手法。侵入実験または侵入テストとも言われる。

## SSL/TLSアクセラレータ

通信を暗号化する[SSL/TLS](#ssltls)を利用する際に、暗号化や復号を専門に行う機器やソフトウェア。 Webサーバなどが行う暗号化などの処理を肩代わりして負荷を軽減することができる。

## ISO/IEC 13335

## ISO/IEC 15408

[CC(Common Criteria)](#cccommon-criteria)参照。

## ISO/IEC 14516

## ISO/IEC 17799

## JIS Q 27000

## JIS Q 31000:2010

## 発見リスク

組織の内部統制によって発見されなかった財務諸表などの虚偽表示が、 監査手続を実施してもなお発見されないリスク。

## 固有リスク

関連する内部統制が存在していないとの仮定の上で、財務諸表に重要な虚偽表示が存在するリスク。

## 投機リスク

損失または利益のどちらの発生の可能性もあるリスク。

## 残留リスク

組織があるリスクに対してが何らかの対応をした結果、残るリスクの大きさ。

## ディジタルフォレンジックス

不正アクセスや情報漏えいなどのインシデントの発生時に、原因究明や法的証拠を保全するために対象となる電子的記録を収集・解析する技術。

## MAC(Message Authentication Code)

メッセージ認証コード。メッセージの改竄検知や送信者の本人認証の機能がある。一方向ハッシュ関数を拡張し、共通鍵を利用した認証。

## XML署名

XML文書をはじめとするさまざまな電子データに対して付けられる電子署名の一種。XML-Sigとも呼ばれる。

## ブロックチェーン

分散型ネットワークを構成する複数のコンピューターに、暗号技術を組み合わせ、取引情報などのデータを同期して記録する手法。各ブロックには、前のブロックの暗号化ハッシュ 、タイムスタンプ、トランザクションデータが含まれ、2つの当事者間の取引を効率的かつ検証可能で恒久的な方法で記録することができる。

## VDIサーバ

Virtual Desktop Infrastructure、仮想デスクトップ基盤。仮想化されたデスクトップ環境をサーバ上に集約してサーバ上で稼働させる仕組み。サーバ上で集中管理することで各種ソフトウェアの追加や更新などのメンテナンスが容易になるというメリットがある。

## Ipsec

Security Architecture for Internet Protocol。 暗号技術を用いることで、IPパケット単位で改竄検知や秘匿機能を提供するプロトコル。

## L2TP

Layer 2 Tunneling Protocol。データリンク層(第2層)において、ある機器から任意のアドレスの別の機器までの仮想トンネルを作成しデータを送受信するためのプロトコル。 PPP接続を利用してVPN接続ができる。暗号化の目的で[Ipsec](#ipsec)と併用される場合が多い。

## SPF

Sender Policy Framework。電子メールの送信元ドメインが詐称されていないかを検査するための仕組み。メール送信に使用されるプロトコルであるSMTPは、差出人のメールアドレス(Fromアドレス)を自由に設定することが可能であり、その悪用を防ぐための対策として考案された。

## ポートスキャン

ネットワークに接続されているサーバー上の稼働サービスを調査するために、複数のポートに対して接続要求を行い、その応答を調べること。サーバーで動作しているサービスのバージョンやOSなどを特定できることがあり、標的の脆弱性を発見するために用いられる基礎的な手法である。有名なポートスキャナーとしてnmapがある。

## シングルサインオン(SSO)

一度のユーザー認証処理によって独立した複数のソフトウェアシステム上のリソースが利用可能になる仕組みである。これを利用することにより、ユーザーはシステムごとにユーザIDとパスワードの組を入力する必要がなくなる。

## ファジング

ソフトウェアの脆弱性を発見するためのテスト手法のひとつ。ファズ(fuzz: 予測不可能な入力データ)を与えることで意図的に例外を発生させ、その例外の挙動を確認するという方法を用いる。

## ISO 9001

## ISO 14001

## OpenPGP(Open Pretty Good Privacy)

公開鍵暗号方式を利用した暗号・署名ができる暗号化ソフトウェア。IETFのRFCに公開されている。

## NIST

National Institute of Standards and Technology、アメリカ国立標準技術研究所。アメリカの国立の計量標準研究所であり、計量学や標準規格、産業技術の発展を推進している。セキュリティに関する規格(NIST CSF)などを定めている。

## TKIP

無線LANの暗号化に用いられるWPAで採用された暗号化プロトコルのひとつ。解読が容易になってしまったWEPの代替手段として広く普及している。

## MACアドレスフィルタリング

Wi-FiルーターにMACアドレスを登録し、特定の機器のみを接続させる機能。ただし、MACアドレスは秘匿情報ではないため、MACアドレスを割り出し偽装される危険性もある。

## CRYPTREC

Cryptography Research and Evaluation Committees。
電子政府が推奨する暗号リストで、安全性を評価・監視し、暗号技術の適切な実装法・運用法を調査・検討するプロジェクトの総称でもある。

## JISC

Japanese Industrial Standards Committee、日本産業標準調査会。様々な技術や規格など工業分野における標準化を促進するのが役割で、日本工業規格(JIS規格)の調査や審議などを行なう。

## 危殆(たい)化

何らかの作為や状況の変化により、対象が危険に晒されるようになること。IT分野では主にコンピュータの性能向上によって暗号化技術をはじめとするセキュリティ技術の安全性が相対的に低下していくこと指す。

## JIS Q 27002

## OCSP

Online Certificate Status Protocol。公開鍵証明書の失効状態を取得するための通信プロトコル。[証明書失効リスト(CRL)](#crl証明書失効リスト)の代替として策定されたもので、CRLを[PKI](#pki公開鍵暗号基盤)で使う際の問題に対応している。

## DNSSEC

Domain Name System Security Extensions。DNSに対し、データ作成元の認証やデータの完全性を確認できるように仕様を拡張したもの。データの偽装を検知することが可能となり、[DNSキャッシュポイズニング](#dnsキャッシュポイズニング)のような攻撃を防ぐことができる。

## ソースポートランダマイゼーション

DNSにおいて、クエリごとにフルリゾルバ(キャッシュDNSサーバー)が権威DNSサーバーに送るクエリパケットのソースポート番号をランダムに変化させる手法。[DNSキャッシュポイズニング](#dnsキャッシュポイズニング)の攻撃成功率を下げることができる。

## ゼロデイ攻撃

新たな脆弱性が発見されたときに、問題の公表や修正プログラムが提供される前に行われるサイバー攻撃のこと。

## エクスプロイトコード

プログラムのセキュリティ上の脆弱性を攻撃するために作成された簡易なプログラムの総称。

## サニタイジング

Webアプリケーションにおけるセキュリティ対策のひとつ。利用者が入力した文字データを受け取る際に、プログラムにとって特別な意味を持つ文字列を検知して、一定の規則に従って別の表記に置き換えること。

## web beacon

HTMLを利用したメールやウェブページの閲覧者を識別する仕組みのこと。Webページが外部から画像などを読み込んでページ内に埋め込んで表示する仕組みを応用し、端末や閲覧者の識別や閲覧行動の捕捉を行う。

## rootkit

コンピュータシステムへの不正アクセスに成功した攻撃者が、侵入後に遠隔操作で活動するために必要なソフトウェア一式をまとめてパッケージにしたもの。遠隔操作の痕跡をシステムのログなどに残さず操作する目的で利用される。

## クリプトジャッキング

ビットコインなどの暗号資産(仮想通貨)はコンピューターのマイニングと呼ばれる演算行為を通じて入手が可能であり、悪意のある攻撃者などがターゲットの端末で不正にマイニング行為を行うこと。

## スキミング

カード犯罪で多く使われる手口の一つで、磁気ストライプカードに書き込まれている情報を抜き出し、全く同じ情報を持つクローンカードを複製する行為。

## CHAP

Challenge Handshake Authentication Protocol。PPPなどで使用されるユーザ認証の一方式。サーバーがクライアントにチャレンジと呼ばれるランダムな短いデータを送信し、クライアントがパスワードとチャレンジを組み合わせたデータを元にしたハッシュ値を送り返すことで認証を行う。

## ボットネット

攻撃者が[トロイの木馬](#トロイの木馬)などの[マルウェア](#マルウェア)を使用して乗っ取った多数のゾンビコンピュータで構成されるネットワークのことを指す。DDoS攻撃や踏み台攻撃に利用されることがある。

## C&Cサーバ

コマンド&コントロールサーバ。ボットネットや感染コンピュータのネットワークに対し、遠隔で制御したり命令を出したりする役割を担うサーバコンピュータのこと。

## Autorun.inf

Windowsの機能の一つで、ストレージをコンピュータに認識させると内部に記録されたプログラムのうち指定されたものを自動的に起動するもの。USBメモリなどでコンピュータウイルスの感染を広げる手段として利用された。

## SMTP-AUTH

SMTPの拡張仕様のひとつで、メールの発送時に、メールサーバが送信依頼をしてきた相手が正規の利用者かどうかを確認する方法を規定したもの。

## サブミッションポート

利用者の電子メールソフトからメール送信サーバにメールを投稿する際に用いる送信専用のTCPポート。標準では587番が、[SSL/TLS](#ssltls)接続の場合は465番が用いられ、併せて[SMTP-AUTH](#smtp-auth)認証を用いることが多い。

## OP25B

Outbound Port 25 Blocking、メール送信規制。ネットワークから外部ネットワークへのTCP 25番ポートの通信を遮断することにより、スパムメールやウイルスメールの送信を抑制しようとする技術。

## DSA(Digital Signature Algorithm)

DLP(Discrete Logarithm Problem、離散対数問題)の困難性をベースとした[ElGamal方式](#elgamal暗号)を改良して、署名の長さを短縮し、秘密鍵の生成などを特定の方法で運用するデジタル署名アルゴリズム。

## IDEA(International Data Encryption Algorithm)

共通鍵暗号方式のブロック暗号アルゴリズム。128ビット長の鍵を用いて8重の暗号化を施すことにより安全性を向上させている。

## DKIM(DomainKeys Identified Mail)

電子署名方式の送信ドメイン認証。送信側のドメインを管理する権威DNSサーバーに公開鍵を登録し、電子メールの署名を確認することで認証を行う。

## APOP(Authenticated Post Office Protocol/Automatic Processing Options Protocol)

電子メールの**受信**に用いるプロトコルであるPOP3において、電子メールの認証に使用する認証情報を暗号化して安全性を高める方式。暗号化にはハッシュ関数が用いられる。

## POP before SMTP

電子メールの**送信**時に正規の利用者であることを認証する方式のひとつ。POP3によるメール受信を行った利用者に一定時間送信を許可する。

## IMAPS(Internet Message Access Protocol)

電子メールの受信に用いるプロトコルであるIMAPに、伝送路を暗号化す[SSL/TLS](#ssltls)を組み合わせたもの。認証情報のみではなくメール本文や添付ファイルの暗号化も行う。

## リスクベース認証

ユーザのアクセス履歴などを元に「不正のリスク」を判定し、高リスクと判定された場合には追加認証などを行うことで、なりすましを防ぐ認証技術。主にユーザの行動パターンとして地理情報、利用デバイス、時間帯、IPアドレスなどが利用される。

## 個人情報の保護に関する法律についての経済産業分野を対象とするガイドライン

## CC(Common Criteria)

コンピュータセキュリティのための国際規格であり、[ISO/IEC 15408](#isoiec-15408)である。情報技術に関連した製品や情報システムなどが適切に設計されているか、総合的に評価し認証するための評価基準を定めている。

## FIPS 140(Federal Information Processing Standardization 140)

暗号モジュールに関するセキュリティ要件の仕様を規定する米国連邦標準規格。

## サイバーセキュリティ経営ガイドライン

経済産業省が[IPA](#ipa)とともに策定した、企業などの経営者が情報セキュリティ対策を実施する上でのガイドライン。

## KCipher-2

九州大学とKDDI研究所により共同開発されたストリーム暗号。ISO/IEC 18033の標準暗号として採用されている。

## 定性的評価

リスクの大きさを金額で表現する方式。

## 定量的評価

リスクの大きさをランク付けやレベルなどの段階評価で表現する方式。

## プライバシーマーク制度

個人情報の保護体制に対する第三者認証制度。個人情報保護体制の基準への適合性を評価し、[JIPDEC](#jipdec)が使用を許諾する。

## WPA2(Wi-Fi Protected Access 2)

IEEE 802.11で使用される無線LANの通信を暗号化する方式の規格のひとつ。[AES](#aes)を利用している。

## WPA2-PSK(Pre-Shared Key)

WPA/[WPA2](#wpa2wi-fi-protected-access-2)では、個人や家庭などの小規模ネットワーク向けにパーソナルモードを用意しており、接続開始前に同じ符号を各機器に入力する認証方式。

## RC4(Rivest's Cipher 4)

[SSL/TLS](#ssltls)やWEP、WPA、sshなど様々なプロトコルの暗号方式の一つとして広く使われている共通鍵暗号方式のストリーム暗号。

## APT攻撃(Advanced Persistent Threat Attack)

持続的標的型攻撃。標的型攻撃のうち、長期間にわたりターゲットを分析して攻撃する緻密なサイバー攻撃。

## ポリモーフィック型マルウェア

パターンマッチングによる検出を免れるため、感染のたびに異なる暗号化/復号ルーチンで暗号化を行って、自身のプログラムコードを都度変化させる機能を有する[マルウェア](#マルウェア)。ミューテーション型とも呼ばれる。

## テンペスト技術

モニタやキーボード，ネットワークケーブルなどから放射されている微弱な電磁波を傍受する技術。

## Man-in-the-Browser攻撃

MITB攻撃。プロキシ型[トロイの木馬](#トロイの木馬)によってWebブラウザの通信を盗聴、改竄を行う攻撃。具体例として、オンラインバンキングへのログインイベントなどを検知し、通信を乗っ取って預金を盗む攻撃などがある。

## Man-in-the-Middle攻撃

MITM攻撃、中間者攻撃。攻撃者がユーザーとその通信相手の間に割り込み、会話内容の読み取りや改ざんをする攻撃。