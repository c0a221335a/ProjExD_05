# 案：大戦争スマッシュこうかとんファイター２


## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
キャラクターのこうかとん二匹を、キー操作で戦わせる格闘ゲーム

## ゲームの実装
### 共通基本機能
* 背景画像とキャラクターの描画
* 他のクラスの変数にアクセスする際にはget, setを利用

### 担当追加機能
* 平谷・キャラ移動 * 2：/キー入力で行動するクラス/ジャンプ, しゃがみ, 左右
* 堀場・攻撃：/ボタン入力で攻撃行動をするクラス/各方向への攻撃, （必殺技）
* 宮田・防御：/Qボタン入力で防御行動をするクラス/円形のガードを表示する, ガードの耐久値(5回)を超えた攻撃を受けるとガードが解除, ガードは受けた攻撃回数によって小さくなっていく, （テスト用）Eボタンで1秒ごとにダメージが発生する
* 高橋・ステータスバー：/攻撃ヒット時にＨＰバーを減少、また回復薬使用時に増加するクラス/HPの増減, （できたら必殺技ゲージ）
* 山平・ゲームの基本設定：/勝敗の条件設定と勝敗が決まった時の画面表示に関するクラス/勝敗条件, 勝敗表示（できたらスタート画面）
* 左側のこうかとんは[wasd]右側のこうかとんは[ijkl]で移動できるようになっている

### ToDo
- [] ジャンプ機能（自由落下）
- [] しゃがむ機能（しゃがんだ時のy座標が変わらないようにする）
- [] ジャンプの時はy座標が500以外では使えないようにする
- 藤沼・アイテム/時間経過毎に設定したアイテムが落下してくるクラス/：回復薬, 行動制限（増やせたら増やす）
- マージした時にパンチの飛距離を調整する必要がある

### メモ
* こうかとんが左右に移動できるようになっている。ジャンプとしゃがみは未完成。
* 左側のこうかとんは[wasd]右側のこうかとんは[ijkl]で移動できるようになっている
* 攻撃：スペースキー
* 防御：「Q」
* 「１」でゲームスタート
*
*

