## 概要  
ロボットシステム学課題2～ROSのパッケージの作成～  
4sのロボットシステム学でROSのパッケージを作成  
RasberryPiにUbuntuをインストール.授業の内容通り、2ずつカウントアップし、1秒ごとに10増加するプログラムを作成した.  

## 実行した動画  
https://www.youtube.com/watch?v=xNabQXsrK8Y

## インストール方法  
1. catkin_ws と src 2つのディレクトリを作成  
`$ cd ~/catkin_ws/src`  

2. クローン  
`$ git clone https://github.com/YuuMitsuhashi/mypkg1/git`  

3. catkin_ws ディレクトリに戻り catkin_make を実行  
`$ cd ..`  
`$ catkin_make`  

## 実行方法  
以下のコマンドをUbuntuの端末画面に入力  
最低でも4つの端末画面が必要.  
1. 端末1つ目でroscoreを起動  
`$ roscore`  

2. 端末2つ目でscripts内のcount.pyを走らせる  
`$ rosrun mypkg1 count.py`  

3. 端末3つ目でscripts内のtwice.pyを走らせる  
`$ rosrun mypkg1 twice.py`

4. 端末4つ目で動作の確認をする  
`$ rostopic echo /twice`  

## 注意事項  
・既にパッケージを作成し、ディレクトリが存在する場合はcount.pyとtwice.pyを含むscripts、package.xmlはパッケージを作成した際に作ったディレクトリの直下に置く必要があります.  
  
・`$ rosrun` でノードの実行をする際は実行のパーミッション設定をする必要があります.  
 `$ chmod +x count.py`  
 `$ chmod +x twice.py`  

## ライセンス  
BSD 3-Clause License  
https://www.freebsd.org/ja/
