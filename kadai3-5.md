## 自動販売機（データ構造と各種処理）のミニレポート
### Q5-1. 自動販売機の商品データついて説明せよ。
* データ構造（各項目とその説明）
  * id: 商品番号（今回は1～8番）
  * name: 商品名（緑茶、水など）
  * price: 金額（今回は100～170円）
  * stock: 在庫数（商品が購入されると1減る）
* 連想配列の配列として定義するメリット
  * 1つの変数でデータをまとめて管理できる。
  * for文などの繰り返し処理を利用することで、すべてのデータを一括管理できる。
  * 商品を増やしたり、要素を変更したりするのが容易。
  * 配列内の要素の並び替えが容易。
  * 数字と文字列など、さまざまなデータを格納できる。
  * 配列の要素数を変更できる。
  * キーと値のペアでデータを管理できる。
### Q5-2. showItemListの処理内容について説明せよ。
* 配列の繰り返し処理
  * for文を用いて、繰り返し処理を行っている。
  * iを初期値0で定義し、配列itemsの商品の数だけ、商品番号や商品名といった配列の内容を項目毎に出力する。
* 連想配列の参照方法
  * items[i].idは、i番目の配列itemsのidを参照する。
### Q5-3. buyItemの処理内容について説明せよ。
* 商品購入の可否判定
  * buyItemの引数としてnoを定義し、在庫がある場合(1以上)は、在庫数を1減らし、在庫がない場合(0)は、「在庫がありません。」と出力する。
* 商品在庫を減らす処理
  * items[no-1].stock--;で、配列itemsのno-1番の商品の在庫数を1減らす。
* 商品番号のエラー処理
  * 指定された商品番号が配列の範囲内か確認して、範囲外の場合はエラー文「無効な商品番号です。番号は1～8で指定してください。」を出力する。
### Q5-4. プログラムの考察
* データ構造について
  * 配列として定義することで、商品を管理しやすい。
* 商品一覧表示と購入処理を関数化したメリット
  * 関数としてまとめてデータを管理することで、プログラム文が短縮され、一括処理しやすい。
### Q5-5. 感想
* 今回の課題で苦労したこと
  * 連想配列の参照方法に一番苦労した。
* 演習を通して理解できたこと
  * 配列のメリットや連想配列について学べた。
* この自動販売機プログラムの追加機能や課題など
  * ブラウザ上でUIを作成する。
