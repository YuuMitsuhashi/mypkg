# 概要  
ロボットシステム学課題2～ROSのパッケージの作成～  
4sのロボットシステム学でROSのパッケージを作成  
授業の内容通り、2ずつカウントアップするものを作成した．  

# 実行した動画  


# 実行方法  
以下のコマンドをUbuntuの端末画面に入力  
最低でも4つの端末画面が必要.  
## 1. 端末1つ目でroscoreを起動  
`$ roscore`  

## 2. 端末2つ目でscripts内のcount.pyを走らせる  
`$ rosrun mypkg1 count.py`  

## 3. 端末3つ目でscripts内のtwice.pyを走らせる  
`$ rosrun mypkg1 twice.py`

## 4. 端末4つ目で動作の確認をする  
`$ rostopic echo /twice`
