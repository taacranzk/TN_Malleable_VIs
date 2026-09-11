# My_Malleable_VIs
Malleable VI

自分用にある程度汎用性のあるMalleable VI(順応性VI)をライブラリにしました。

- Array Average：入力配列の平均値を計算します。配列の総和を計算してから要素数で割っているため、オーバーフローする場合は要修正。配列の次元は何でも可。
- Array Nearest Index：配列から入力値に最も近い要素を取得します。配列の次元は何でも可。配列の型はDoubleを想定。
- Array Same Size：2つの入力配列のサイズを比較します。2つの配列の型が異なる場合も対応可能です。配列の次元は任意ですが、2つの入力で同じである必要があります。
- Boolean to 0-1：ブールを0,1に変換します。入力のブールは任意の次元の配列でも対応可能。変換する型を指定できるようにしています。
- Close Front Panel：パネルを閉じます。入力するVIリファレンスは任意の次元の配列でも対応可能。このVIでは閉じるときに発生するエラーを無視します。エラーが入力されていてもパネルを閉じようとします。
- Format Accounting Number：数値入力を会計の表記(日本のもの、3桁ごとにカンマ区切り)に変換します。
- Generate Value Change Event at Current Value：現在の値のまま値変更イベントを発生させます。
- Get Current Timestamp：最大3つの配線が全て入力されたときのタイムスタンプを取得します。
- Get Tail of 1D Array：1次元配列から後ろn個だけを出力します。
- Random Number：乱数を発生させます。出力する型をType入力で指定できます。アルゴリズムは既存のPolymorphic VIのコピーペーストです。
- Set Named Number Default if Invalid：Named Number(列挙体やテキストリング)制御器の現在値が無効の値なら入力したデフォルト値に変更します。デフォルト値の無効確認は行いません。
