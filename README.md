# myled1
ロボットシステム学2019 課題１

### 概要
Raspberry piと講義で用いたデバイスドライバ，LEDランプ，抵抗を使いLEDを点灯させるプログラム．

### 動作環境
|||
|:--:|:--:|
| Raspberry Pi | Raspberry Pi Model 3B+ |
| OS | raspbian |

### 実行方法
```
$ git clone https://github.com/OhnoKotaro/myled1.git
$ cd myled1
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ sudo echo 1 > /dev/myled0
$ sudo echo 0 > /dev/myled0
$ ./flash.sh
$ sudo rmmod myled.ko
```
echo 1でLED点灯,echo 0でLED消灯．./flash.shで3回点滅させる．

### デモ動画
https://youtu.be/L6IA2AlpFIg
