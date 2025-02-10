# TReK LC
GL516 inspire keyboard tray.

![TReK L.C](./PXL_0000.jpg)

## 概要
このキーボードトレイは、サリチル酸さんの提唱しているキーボードケース規格「GL516」※1を基に、私が設計／頒布しているキーボードのうち、いくつかの条件に合ったキーボードでの使用を想定しています。
その条件というのは、おおまかには下記にのようになります。

- MCUを左右どちらかに配置している（中央配置のキーボードは使用不可です）
- スイッチプレート天面からMCU底面までの厚さが16mm
- MCU部分以外の、スイッチプレート底面から、PCB裏の最大突起物を含めた厚さが7mm以下

使用出来る対象キーボードは、

- TReK GT40Plus PARALLAX
- TReK G70 CLAVIS

になります。
下記のキーボードは使用不可になります。
- TReK GT40 DONUMCOELI（MCUが中央に配置されているため）
- TReK G50 TIJUANA（そもそもGL516ケースを使用する想定になっていないため）

## パネルマウントケーブル
このトレイは、PCB底面より下の、MCU部分の厚さ（高さ）を7mm以下にしているため、Amazonなどで売っているパネルマウントのUSB-C延長ケーブルが使用出来ません。
なので、使用するにはパネルマウント部の高さが7mm以下のパネルマウントケーブルを自作する必要があります。

私が作成したケーブルのレシピを書いておきます。

パネルマウントするUSB-C Femaleコネクタはこれを使用しました。
- https://amzn.asia/d/55BpzSk

USB-C FemaleコネクタにUSB2.0用のケーブルがハンダ付けされているので、このケーブルをそのまま使用します。
反対側のUSB-C Maleコネクタにはこれを使用しました。
- https://amzn.asia/d/052WZSY

私は後々、このケーブルを複数作ると予想したので10個入りを買いましたが、VCC, D+, D-, GNDの4端子があるUSB-C Maleコネクタであれば使えると思います。
USB-C Femaleコネクタにハンダ付けされているケーブルを、USB-C Maleコネクタにハンダ付けするのですが、その前にMale、Female両コネクタを保護するために熱収縮チューブを通しておきます。
Maleコネクタをハンダ付けする前に、すでにハンダ付けされているFemaleコネクタに熱収縮チューブを通し熱して固定しておくと良いでしょう。

![Femaleコネクタ](./PXL_0001.jpg)

Femaleコネクタの処理が終わりましたら、Maleコネクタ側に熱収縮チューブを通し、ケーブルをハンダ付けし、熱収縮チューブを熱して固定します。
![Maleコネクタ](./PXL_0002.jpg)

このパネルマウントFemaleコネクタの固定部分にあるネジ穴をタップを切っていないので、ネジだけで固定出来ません。
なので、M2のネジとM2のナットが必要です。
M2のネジは自作キーボードをやっている方であれば特に用意しなくても手元にあると思いますが、私はナットが手元に無かったのでAmazonで購入しました。
- https://amzn.asia/d/24mBXOl

このパネルマウント延長ケーブルを使って、トレイにUSBコネクタを固定します。

かなりタイトなので、ケーブルをマスキングテープなどで固定しながらだと、上手く接続出来ると思います。

----

※1 GL561デザインガイド https://zenn.dev/salicylic_acid3/books/gl516_design_guide
