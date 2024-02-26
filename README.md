# nodularity.py

## 概要

**nodularity.py**nodularity.py es un programa que calcula la tasa de nodularidad del grafito utilizando el método ISO JIS G5502-2022 y el método JIS para productos de hierro fundido de grafito esferoidal (FCD). Aquí, la imagen del tejido se muestra a continuación.


<br><br>

<img src="https://user-images.githubusercontent.com/91704559/202900113-c0a879b3-b298-4bd7-a2df-a03c2ddf4c07.jpg" width=400>
<br>
図 球状黒鉛鋳鉄品の組織画像
<br><br>

## 動作環境

**nodularity.py**は、[Python](https://www.python.jp/)がインストールされたパソコンで動作します。このプログラムの実行には、画像処理のライブラリ[OpenCV](https://opencv.org/)が必要です。
<br><br>

## 使い方

1. **nodularity.py**を適当なフォルダに置きます。
2. **nodularity.py**の18行目以降の環境設定の**iDir**と**min_grainsize**の値を設定します。<br>
ここで、**iDir**はダイアログ「画像ファイルを選んでください」で最初に表示させたいフォルダを設定し、**min_grainsize**は「最小黒鉛のサイズ」÷「画像の幅」の値を設定します。
3. 上記2.の**iDir**に設定したフォルダに上図のような組織画像を格納して**nodularity.py**を実行します。**nodularity.py**と組織画像は全角文字を含まないフォルダに格納してください。
4. プログラムを実行すると最初にダイアログ「画像ファイルを選んでください」が表示されるので、球状化率を求める組織画像を選択します。**min_grainsize**が同じ組織画像でしたら複数選択しても構いません。画像ファイルを選択して開くをクリックして少し待つと、球状化率を計算して以下のファイルを作成します。

- **nodularity_日付時刻.csv** ... ファイル名や球状化率などのデータ
- **画像ファイル名_ISO.jpg** ... 黒鉛形状の判定結果(ISO)
- **画像ファイル名_JIS.jpg** ... 黒鉛形状の判定結果(JIS)

## ご利用に関して

使用結果について当方は責任は負いません。

## 開発環境
- Windows11
- VSC 1.7.3.1
- Python 3.8.10
- OpenCV 4.5.4
