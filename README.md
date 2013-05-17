# Max-secureDisplay

## 概要

マウスポインタの位置を制限するMax Patchです。Google Chromeで[Fullscreen API](https://developer.mozilla.org/ja/docs/DOM/Using_full-screen_mode)を用いてフルスクリーン表示したウェブコンテンツを展示する際に作成しました。    

## 詳細

Google Chromeにて、Fullscreen API由来のフルスクリーンモードを解除する方法は、

1. ESCAPEキーを押す
2. 別のページへ移動する
3. マウスカーソルを画面上端まで動かすとメニューバーが表示されるので、そこでフルスクリーン解除ボタン（Mac OS 10.7で確認した際は右上のもの）を押す

などが考えられます。来場者にマウスで操作してもらうコンテンツである場合、キーボードを取り外して 1. の方法を防ぎ、右クリックを無効にして 2. を防いだとしても 3. の方法が残ります。    
そこで、マウスが一定以上に上の位置へ移動できないようにして 3. の方法も防ぐため、本Patchによってマウスカーソルの位置を監視・変更しました。

## 動作環境

最新の [Max](http://cycling74.com/products/max/) または [Max Runtime](http://cycling74.com/downloads/runtime/) を使用してください。 [aka.mouse オブジェクト](http://www.iamas.ac.jp/~aka/max/#aka_mouse) （赤松正行 氏）に依存しているので、そちらもインストールしてご利用ください。


## ライセンス

MITライセンスを採用しています