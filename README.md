MqPmxConvert　.20160730
====

## 概要
.mqo&.mqx形式と.pmx形式のモデルデータを相互変換するためのプログラムです。  
プラグイン形式ではなくプログラム単体で動作し、Metasequoia4標準のボーン情報にも対応しています。  
(This program provides the interconversion between .mqo&.mqx and .pmx, and supports bone information of Metasequoia Ver4.  
 You can run it as not a plugin software but a single program.)  

## 必須要件
Windows向けソフトウェアです。動作には.NET Framework 4.0のインストールが必要です。(http://www.microsoft.com/ja-jp/download/details.aspx?id=17718)  
(For Windows. .NET Framework 4.0 is needed.)    

## 使い方
・プログラムを開くまでの手順   
① Releaseページ(https://github.com/untiepante/MqpmxConvert/releases)からダウンロード，もしくはプロジェクト全体をダウンロードします   
② MqPmxConvert/bin/Releaseまでフォルダをたどります   
③ プログラムMqPmxConvert.exeを開きます   
④ 目的に応じて以下の項目に従ってファイルを指定してください   

・mqoからpmxへの変換  
① プログラムを開きます  
② 変換したい.mqoファイルを選択します  
③ 変換してできる.pmxファイルの名前を指定します。標準では元の名前の後ろに「.cnv.pmx」を付与した名前になっています   
④ 変換が実施されコンソールウィンドウに「正常終了」と表示されます  
※曲面やIK、一部材質等の情報は変換されません  
  
・pmxからmqoへの変換  
① プログラムを開きます  
② 変換したい.pmxファイルを選択します  
③ 変換してできる.mqo・.mqxファイルの名前を指定します。標準では元の名前の後ろに「.cnv.mqo」を付与した名前になっています  
④ 変換が実施されコンソールウィンドウに「正常終了」と表示されます  
※物理やモーフ、一部材質等の情報は変換されません  
  
※本プログラムに変換したいファイルをドラッグアンドドロップすることによっても変換することができます  
※また、コマンドライン引数を入力ファイルパス、出力ファイルパスの順で与えることによっても変換することができます  
  
(  
[How to launch program]
 1. Obtain an archive file at Release page (https://github.com/untiepante/MqpmxConvert/releases), or download the whole of this project.   
 2. Open MqPmxConvert/bin/Release directory.   
 3. Launch MqPmxConvert.exe, and specify files like the followings.   

[Mqo to pmx]
 1. Launch this program.  
 2. In a file browser dialog, select source mqo file.  
 3. In a file browser dialog, decide the name of a destination file.  
 4. After the conversion finishes, "正常終了" will be displayed.  
  * Information of curved surfaces and inverse-kinematicsk, materials has been lost maybe.  

[Pmx to Mqo]
 1. Launch this program.  
 2. In a file browser dialog, select source pmx file.  
 3. In a file browser dialog, decide the name of a destination file.  
 4. After the conversion finishes, "正常終了" will be displayed.
  * Information of rigids and joints, morph, materials has been lost maybe.

* You can convert a file with drag-and-drop or command-line arguments.)

## 更新履歴

・20160730
<修正>
MQ->PMX変換時に、ボーンのウェイトがうまく設定されないことがある不具合を修正しました。
Fixing the problem of wrong bone weight setting.

・20160522
<追加>
MQ->PMX変換時に、VMDモーションのボーン名文字列長制限に適合するようにリネームするような処理を追加しました。
Adding feature of renaming bone's names whose length is too long to be read by MMD.

・20160504
初期リリース
Initial release.

## ライセンス
本プログラムはフリーウェアです。完全に無保証で提供されるものでありこれを使用したことにより発生した、または発生させた、あるいは発生させられたなどしたいかなる問題に関して製作者は一切の責任を負いません。  
別途ライセンスが明記されている場所またはファイルを除き、個人・商用利用にかかわらず使用者は自らの責任において本プログラムを自由に複製、改変することが可能です。  

## 謝辞
本プログラム作成にあたっては以下の方のコードを利用させていただいております。この場を借りてお礼申し上げます。  
b2ox様作成 MQOplugin (https://github.com/b2ox/MQOplugin)  
ぱるた様作成 tso2mqo (https://osdn.jp/projects/tdcgexplorer/)  
Alexandre Mutel様 SharpDX (http://sharpdx.org/)  

## Author
saso
