# mypkg
![test](https://github.com/kyo0221/mypkg/actions/workflows/test.yml/badge.svg)

このリポジトリはロボットシステム学の授業内課題リポジトリであり,mypkgファイルの中には数字をカウントしてトピックを通じて送信するtalker.pyとトピックからメッセージを貰って表示するlistener.pyというノードのプログラムが含まれている.
# talker.pyコマンド
## コマンドの概要
数字をカウントしてトピック/countupを通じて送信する機能を持つパブリッシャを持つノードである.
メッセージの型はInt16型でありトピックはcountupである.
## 使用例
```
ros2 run mypkg talker
```

(何も表示されない)
# listener.pyコマンド
## コマンドの概要
listener.pyは/countupからメッセージを受け取り表示する機能を持つサブスクライバを持つノードである.
talker.pyから発せられたInt16型のcountupを受け取る.
## 使用例
```
ros2 run mypkg listener
```

(talkerの出した数値を表示)
# 必要なソフトウェア
* Python 3.10.6
# テスト環境
* Ubuntu 22.04
* ROS2
# ライセンス
* このソフトウェアパッケージは,3条項BSDライセンスの下,再頒布および使用が許可されます.

© 2022 Kyo Yamashita
