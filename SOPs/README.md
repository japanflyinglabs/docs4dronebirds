# SOPs - Standard operating procedure
## A. Operating Standards
### 1. Our Mission
### Creating a society where local communities use Robotics for Social Good.
### 2. 安全第一
### 3. ドローン操縦者は操縦ライセンス制度による国家ライセンス（一等ライセンスまたは2等ライセンス）を取得すること
### 4. ドローン操縦者、補助員および監視員は航空法をはじめとする飛行に係るすべての法律（例：小型無人機等飛行禁止法、電波法など）および運用ルールやガイドラインを遵守することを基本とする
ドローンが単に上空を通過する場合は、今後原則手続きが不要となる法令：道路交通法、道路法、河川法、自然公園法、国有林野の経営管理に関する法律、港則法、海上交通安全法、港湾法、漁場漁場整備法

* [国土交通省の無人航空機の飛行ルール](https://www.mlit.go.jp/koku/koku_tk10_000003.html):　頻繁に更新されるので、常にサイトでチェックすること
* [無人航空機の飛行の安全に関する教則　第3版](https://www.mlit.go.jp/common/001602108.pdf)
* [航空法132条の92の適用を受け無人航空機を飛行させる場合の運用ガイドライン](https://www.mlit.go.jp/common/001110204.pdf) (捜索、救助等のための特例）
  参考：[航空法第132条92の特例適用の対象となり得る事例](https://www.mlit.go.jp/koku/content/001846242.pdf)
 
 参考：
 * [国土交通省の無人航空機総合窓口サイト](https://www.mlit.go.jp/koku/info/index.html)
 * [DIPS2.0 ドローン情報基盤システム](https://www.ossportal.dips.mlit.go.jp/portal/top/)
 
## B. Operating Procedures
### 1.  関係者による飛行計画の話し合い
### 2.  飛行・空撮作業計画書を作成し飛行計画を提出する
参考：[飛行計画の通報方法](https://www.uafpi.dips.mlit.go.jp/contents/fpl/preview/01.DIPS-Manual_FPR_JP_FlightPlanReporting.pdf)

* 飛行目的
* 飛行させる飛行禁止空域および飛行の方法　（CrisisMappersJapanと災害協定を結んでいる自治体上空）
* 飛行日時
* 離発着地点（緊急時着陸させる地点を含む）と所要時間
* 飛行経路　
* 最大飛行高度（地上高、および海抜高）と速度
* 機体数
* 使用機材（機体登録記号表示あるいはリモートID、種類、重量、寸法、色、必要なら型式認証・機体認証など）
* メンバー（役割分担、技能証明書番号）
* 何かあった場合の対策を考えておく（障害物の位置のチェック。安全にホバリング・旋回できる場所の設定など）
* 飛行の許可・承認
* 保険契約
* 緊急および主要連絡先
* 撮影に係るガイドライン
#### 飛行について
 1. [飛行チェックリスト](https://github.com/japanflyinglabs/docs4dronebirds/tree/master/checklist)で機材・環境条件その他を確認 
 2. 高度100-150m上空からの静止画像撮影　（災害時　150ｍ上）
 3. オーバーラップ/サイドラップ 70%以上
 4. 原則オートパイロット
 5. 林野庁、自衛隊などのヘリが目視確認できる場合十分に注意して飛行
 6. コミュニケーションはZelloでおこなう。事故の際の保険申請はZelloの録音情報を使用する
 7. そのほか連絡事項（SNS ハッシュタグ、クレジット）
 8. 持参するべき必要書類またはURL　（無人航空機の飛行に係る許可・承認書や自治体との災害協定書,技能証明書、機体認証書、飛行日誌など）
 9. 飛行日誌で[飛行記録](https://github.com/japanflyinglabs/docs4dronebirds/blob/master/SOPs/%E6%A7%98%E5%BC%8F1%E9%A3%9B%E8%A1%8C%E8%A8%98%E9%8C%B2.pdf)をする
### 3. リスク管理
考えられるリスクを洗い出しどう対処するか準備するとともに、リスク低減の措置を常に考える。
機械は壊れる。飛んでいるものはありとあらゆる可能性（不可抗力、操縦ミスなど）で落ちる可能性がある
### 4.  飛行・空撮作業後は作業者全員でフライトを振り返る
気づき、危険なことはなかったか、次に生かせることはないかなど話し合い記録する
## C. Data Management 
 1. Google Docs に[命名規則](https://github.com/dronebird/namingconvention4dronebird)に沿った名のフォルダーを作成し、撮影データの保存と共有
 3. SfMでオルソモザイク処理後、GeoTIFF/EPSG:4326(WGS84)で共有
 4. Google Docs で GeoTIFFファイルを共有
 5. [OAM(OpenAerialMap)](https://openaerialmap.org/)にGeoTIFFファイルをアップロードし公開
 6. OAMからXYZタイルをエクスポートし[ひなたGIS](https://hgis.pref.miyazaki.lg.jp/hinata/)にレイヤ―追加して公開
 7. [DRONEBIRDのGitHub](https://github.com/dronebird)にRepositoryを作成しRaw Data アップロードし、公開された各Permalink（XYZタイル画像データ,OAM, ひなたGIS）を表示
 8. ライセンスはCC BY 4.0。ライセンス表記は ” ©CrisisMappersJapan/DRONEBIRD, CC BY 4.0” とする
## D. Maintenance & Training
 1. [無人航空機の飛行日誌の取り扱いに関するガイドライン](https://www.mlit.go.jp/common/001599241.pdf) に沿って
   * 点検・整備記録　- [飛行前点検, 飛行終了時点検](https://github.com/japanflyinglabs/docs4dronebirds/blob/master/SOPs/%E6%A7%98%E5%BC%8F2%E6%97%A5%E5%B8%B8%E7%82%B9%E6%A4%9C.pdf), [定期点検　整備](https://github.com/japanflyinglabs/docs4dronebirds/blob/master/SOPs/%E6%A7%98%E5%BC%8F3%E7%82%B9%E6%A4%9C%E6%95%B4%E5%82%99%E8%A8%98%E9%8C%B2.pdf)の記録を取る
   * 飛行日誌の作成
 2. 訓練　- 定期訓練によりドローン操縦技術や安全確保の仕方を習得するだけでなくMapping Toolの使い方も訓練する
 
　


