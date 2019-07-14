# キッシュパンツパッチ
パンツは一期一会  

現在対応アバターはパンツ変換を含め、[キッシュ](https://mutachannel.booth.pm/items/954376)ちゃん(素体はブラジャーも対応)、[キッシュ・ライト](https://mutachannel.booth.pm/items/1379653)ちゃん、[シャーロ](https://tomori-hikage.booth.pm/items/987296)ちゃん、[吸血鬼アンナ](https://wakonoatorie.booth.pm/items/1067958)ちゃん([ライト](https://wakonoatorie.booth.pm/items/1405336))、[ミルク](https://komado.booth.pm/items/1209496)ちゃん、[リンツ](https://mutachannel.booth.pm/items/1255264)ちゃん(素体はブラジャーも対応)、[ルア](https://ficsnade.booth.pm/items/1255054)ちゃん([クエスト](https://ficsnade.booth.pm/items/1414368))、[右近](http://seiga.nicovideo.jp/seiga/im8378009)ちゃん、[ミーシェ](https://ponderogen.booth.pm/items/1256087)ちゃん、[ファジー](https://nagatorokoyori.booth.pm/items/1255283)ちゃん、 [たぬ](https://udonfactory.booth.pm/items/1414433)ちゃんです。

## 導入にあたって
2019/06/12以降は[自動インストールバッチファイル](https://gist.github.com/TenteEEEE/1ef33308bd841e3c5f1c8a1a8ab95d67)を実行するのが一番簡単です。  

手動で導入する場合は、[siro_choco0621](https://twitter.com/siro_choco0621)さんが導入についての[メモ](https://twitter.com/siro_choco0621/status/1131587508238659585)をまとめてくださいましたので、こちらを参考に！  
URL: https://twitter.com/siro_choco0621/status/1131587508238659585

## 更新履歴
2019/07/14: [たぬ](https://udonfactory.booth.pm/items/1414433)ちゃんへの変換に対応しました。  
2019/07/12: 似たようなパンツを検索するfind_similar_pantie.pyを追加しました。`python find_similar_pantie.py 1` とすれば1番に似たパンツがデフォルトで5枚表示されます。  
2019/06/27: [ルア・クエスト](https://ficsnade.booth.pm/items/1414368)への変換に対応しました。  
2019/06/18: キッシュ/リンツちゃん素体用のブラジャーへの変換に対応しました。  
2019/06/12: [自動インストールバッチファイル](https://gist.github.com/TenteEEEE/1ef33308bd841e3c5f1c8a1a8ab95d67)を公開しました。  
2019/06/07: [アンナ・ライト](https://wakonoatorie.booth.pm/items/1405336)への変換に対応しました。  
2019/06/05: フーリエ変換されたパンツ画像の逆変換に対応しました。phase_retrieval.pyでは[ERあるいはHIOアルゴリズム](https://en.wikipedia.org/wiki/Phase_retrieval)の選択、cupyがあればGPU上で実行できます。  
2019/05/30: パンツ画像のフーリエ変換に対応しました。convert_fourier.pyではRGBモードと16bit出力がオプションで指定できます。  
2019/05/20: [キッシュ・ライト](https://mutachannel.booth.pm/items/1379653)への変換に対応しました。patch.pyで-Lオプションを指定してください。  
2019/04/15: [ファジー](https://nagatorokoyori.booth.pm/items/1255283)ちゃんの変換に対応しました。  
2019/04/13: [ミーシェ](https://ponderogen.booth.pm/items/1256087)ちゃんの変換に対応しました。  
2019/04/12: [キッシュちゃん素体](https://mutachannel.booth.pm/items/1026956)用のオプションを追加。patch.pyで-nをオプションを指定してください。  
2019/04/10: [右近](http://seiga.nicovideo.jp/seiga/im8378009)ちゃんへの変換スクリプトを[thakyuu](https://github.com/thakyuu)さんが開発、本リポジトリにマージしました。  
2019/04/06: [ルア](https://ficsnade.booth.pm/items/1255054)ちゃんの変換に対応しました。  
2019/03/08: [リンツ](https://mutachannel.booth.pm/items/1255264)ちゃんの変換に対応しました。patch.pyで-lオプションを指定してください。  
2019/02/09: [ミルク](https://komado.booth.pm/items/1209496)ちゃんの変換に対応しました。また、dreamフォルダにあるパンツをすべて変換するスクリプトを追加しました。  
2019/01/30: [キッシュ](https://mutachannel.booth.pm/items/954376)ちゃんの他に、[シャーロ](https://tomori-hikage.booth.pm/items/987296)ちゃんと[吸血鬼アンナ](https://wakonoatorie.booth.pm/items/1067958)ちゃんは変換スクリプトで対応しています。  
ちなみに吸血鬼アンナちゃん、ミルクちゃん、ミーシェちゃんは淫紋も刻めます。詳細はパンツコンバートにて。

## 必要なもの
ペイントもしくはレタッチソフトがある方はbody.pngの上に画像を重ねるだけでOKです。  
それすらも面倒だという人の為に、Pythonスクリプトもあります。  
他アバターへのパンツ変換をしたい方は変換スクリプトを動かすためにPythonが必須です。  
[Python(3系を推奨)](https://www.python.org/downloads/)

必要な外部パッケージはコンソールからワン・コマンドでインストールできます。  
`pip install -r requirements.txt`  

このリポジトリは基本的に毎日更新されるので、最新のパンツを追いたい方はGitのインストール推奨です。  
[Git for windows](https://git-scm.com/)  
インストール後はコンソール(cmdもしくはpowershell)を開いて `git clone https://github.com/TenteEEEE/quiche_pantie_patch.git` でダウンロードできます。  
とりあえず最新版にしたければクローンしたディレクトリで`git pull`でいい感じに更新してくれます。

## パンツパッチ(キッシュ、リンツちゃん)
0. このリポジトリを[ダウンロード](https://github.com/TenteEEEE/quiche_pantie_patch/archive/master.zip)します (gitが分かる人はcloneを推奨)
1. body.pngをあなたのbodyテクスチャで置き換えてください
2. コンソールからpatch.pyを実行します `python patch.py`
3. パンツ番号を聞かれるので好きな番号を入力します 例:0001.png
4. patched.pngが上書き済みテクスチャです Enjoy!

パッチを実行するときに `python patch.py -r` とすると、ランダムでパンツが選ばれます。  
また、`-l`を追加するとリンツちゃん向けの微補正を加えます。`-n`はキッシュ/リンツちゃん素体用のオプションです。`-L`はキッシュちゃんライト用のオプションです。`-a`で全てのパンツの変換を行います。`-p`で変換するパンツを指定できます。`-i`でベースとなるテクスチャを指定できます。`-o`で変換後のファイルを指定できます。

## ブラコンバート(キッシュ、リンツちゃん素体用)
convert_bra.pyでキッシュ/リンツちゃん素体用のブラジャーを自動生成できます。  
`python convert_bra.py`  
とすれば最新のパンツが変換されます。番号を指定したい場合は  
`python convert_bra.py --num 101`  
のようにします。また、上から重ねるだけの楽ちんテクスチャを作りたければ更に  
`python convert_bra.py --num 101 --pad`  
のように`--pad`オプションを併用すると良いです。

### オプション
* --num: 変換するパンツ番号を指定できます。何も入力しなければ最新のパンツが選ばれます。
* --all: 全てのパンツを変換できます。numで指定するとその番号から最新まで変換します。
* --pad: パディングを行い、上から重ねるだけの楽ちんテクスチャを作ります
* --lace: デフォルトではフリルを貼り付けますが、レースにもできます

以下はペイントソフトなどで手動調整する人向けのオプションです。
* --disable_ribbon: リボンはデフォルトで取り付けられますが、付けたくない場合はこれを書くと良いです。
* --disable_decoration: フリルやレースを貼り付けないようにします。
* --disable_shading: 影の自動彩色をやめます。
* --disable_texture: ブラの胸パッド部分以外の自動テクスチャをやめます。

## パンツコンバート
すべてきれいに変換できるわけではありませんが、[シャーロ](https://tomori-hikage.booth.pm/items/987296)ちゃん、[吸血鬼アンナ](https://wakonoatorie.booth.pm/items/1067958)ちゃん、[ミルク](https://komado.booth.pm/items/1209496)ちゃん、[ルア](https://ficsnade.booth.pm/items/1255054)ちゃん、[右近](http://seiga.nicovideo.jp/seiga/im8378009)ちゃん、[ミーシェ](https://ponderogen.booth.pm/items/1256087)ちゃん、[ファジー](https://nagatorokoyori.booth.pm/items/1255283)ちゃんのパンツに変換できます。  
基本的にパンツパッチに使うコマンドを `python patch_[character].py` に変えるだけです。  
変換画像だけ欲しいときは `python convert_[character].py`で作れます。  
他にも使用者が多いアバターはできるだけ対応したいので、対応して欲しい人はテストユーザになる覚悟とともにテクスチャ画像を[@tenteeeee_vrc](https://twitter.com/tenteeeee_vrc)に送ってください。

### 特殊オプション
#### シャーロちゃん
* -c: 縫い目の補正方法を変更できます。なんか変になったというときに書いてみてください。

#### アンナちゃん
* -s: 淫紋をお腹に刻みます。

#### ミルクちゃん
* -s: 淫紋をお腹に刻みます。

#### ミーシェちゃん
* -s: 淫紋をお腹に刻みます。

#### ファジーちゃん
* -f: お尻側にフリルのあるパンツはこれを指定してください。

## 変換サンプル
|||
|:-:|:-:|
|[シャーロ](https://tomori-hikage.booth.pm/items/987296)ちゃん|[吸血鬼アンナ](https://wakonoatorie.booth.pm/items/1067958)ちゃん|
|![test](./sample/shaclo_pantie.png)|![test](./sample/anna_pantie.png)|
|[ミルク](https://komado.booth.pm/items/1209496)ちゃん|[ルア](https://ficsnade.booth.pm/items/1255054)ちゃん|
|![test](./sample/milk_pantie.png)|![test](./sample/lua_pantie.png)|
|[右近](http://seiga.nicovideo.jp/seiga/im8378009)ちゃん|[ミーシェ](https://ponderogen.booth.pm/items/1256087)ちゃん|
|![test](./sample/ukon_pantie.png)|![test](./sample/mishe_pantie.png)|
|[ファジー](https://nagatorokoyori.booth.pm/items/1255283)ちゃん|[吸血鬼アンナ light](https://wakonoatorie.booth.pm/items/1405336)ちゃん|
|![test](./sample/fuzzy_pantie.png)|![test](./sample/anna_light_pantie.png)|
|キッシュ/リンツ用のブラ(フリル)|キッシュ/リンツ用のブラ(レース)|
|![test](./sample/bra_frill.png)|![test](./sample/bra_lace.png)|
|[ルア・クエスト](https://ficsnade.booth.pm/items/1414368)ちゃん|[たぬ](https://udonfactory.booth.pm/items/1414433)ちゃん|
|![test](./sample/lua_quest_pantie.png)|![test](./sample/tanu_pantie.png)|


## スペシャルサンクス
[Booth:キッシュちゃん](https://mutachannel.booth.pm/items/954376)  
右近ちゃんパンツコンバータの作者:[thakyuuさん](https://github.com/thakyuu)  
patch.pyのargparse対応:[4hiziriさん](https://github.com/4hiziri)  

## 画像のライセンス
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/tenteeeee_vrc" property="cc:attributionName" rel="cc:attributionURL">TenteEEEE</a> を著作者とするこの <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/StillImage" rel="dct:type">作品</span> は <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">クリエイティブ・コモンズの 表示 - 非営利 - 継承 4.0 国際 ライセンス</a>で提供されています。  
作品のクレジットの表示が必要なライセンスではありますが、アバターのテクスチャにクレジット表記という無粋なものは不要です！  
どこかで再配布する場合などに別のテキストファイルなどで記載してください。  
また、商用利用したい場合は[@tenteeeee_vrc](https://twitter.com/tenteeeee_vrc)までご相談ください。  

## ソフトウェアのライセンス
MITライセンス(一行で:無料で自由に使える/変更できるが、なにか問題があっても作者は責任を負わない)に従います。  
https://opensource.org/licenses/mit-license.php  
Copyright (c) 2019 TenteEEEE  


---
**English**
# Quiche Pantie Patch
Treasure every pantie encounter as it may not come again.

## Update log
2018/12/05 crop.py crops the pantie texture for pantie designer.  
2018/12/06 patch.py supports random pantie option '-r'. (`python patch.py -r`)  
2018/12/18 convert_shaclo.py converts Quiche pantie to [Shaclo](https://tomori-hikage.booth.pm/items/987296) pantie.  
2018/12/25 convert_shaclo.py supports stitch correction switch.  
2018/12/25 convert_anna.py converts Quiche pantie to [Anna](https://wakonoatorie.booth.pm/items/1067958) pantie.  
2019/02/09 convert_milk.py converts Quiche pantie to [Milk](https://komado.booth.pm/items/1209496) pantie.  
2019/03/08 patch.py supports [Linz](https://mutachannel.booth.pm/items/1255264). Please set -l option when you run the patch.py  
2019/04/06 convert_lua.py converts Quiche pantie to [Lua](https://ficsnade.booth.pm/items/1255054) pantie.  
2019/04/10 [thakyuu](https://github.com/thakyuu) developed [Ukon](http://seiga.nicovideo.jp/seiga/im8378009) converter, and it was merged.  
2019/04/12 patch.py supports [Quiche body](https://mutachannel.booth.pm/items/1026956). Please set -n option when you run the patch.py  
2019/04/13 convert_mishe.py converts Quiche pantie to [Mishe](https://ponderogen.booth.pm/items/1256087) pantie.  
2019/04/15 convert_fuzzy.py converts Quiche pantie to [Fuzzy](https://nagatorokoyori.booth.pm/items/1255283) pantie.  
2019/05/20 Support [Quiche-Light](https://mutachannel.booth.pm/items/1379653). Please set -L option when you run the patch.py  
2019/05/30 Support Fourier transform of the panties. convert_fourier.py has options that RGB mode and 16bit output mode.  
2019/06/05 Support inverse Fourier transform from the intensity of the Fourier transformed panties. phase_retrieval.py handles [ER or HIO algorithm](https://en.wikipedia.org/wiki/Phase_retrieval). If you know cupy, it can run on GPUs.  
2019/06/07: Support [Anna light version](https://wakonoatorie.booth.pm/items/1405336).  
2019/06/12: I published [the auto install batch file](https://gist.github.com/TenteEEEE/1ef33308bd841e3c5f1c8a1a8ab95d67).  
2019/06/18: Support bra conversion for Quiche and Linz body.  
2019/06/27: Support [Lua for Quest](https://ficsnade.booth.pm/items/1414368).  
2019/07/12: find_similar_pantie.py find it. e.g. `python find_similar_pantie.py 1` it finds panties like 0001.png. 
2019/07/14: Support [Tanu](https://udonfactory.booth.pm/items/1414433).  

# Installation
Please check it out [the automatic install batch](https://gist.github.com/TenteEEEE/1ef33308bd841e3c5f1c8a1a8ab95d67).  
You just run the batch file with administrator permission.

# Pre-requirements
If you have any paint or retouch software, you can override easily.  
However, I understand that you guys are lazy.   
Don't worry, I prepared a python script to override the body.png.  
[Python(3 is recommended)](https://www.python.org/downloads/)

The patch require external packages.  
I summarized them in the requirements.txt and you can install it easily.  
`pip install -r requirements.txt`

# Texture overriding
1. Overwrite body.png
2. Run patch.py `python patch.py`
3. Put your favorite number (example: 0001.png)
4. Enjoy

The instructions can also be used for Shaclo and Anna patch.  

# Your own dream panties overriding
1. Overwrite body.png
1. Place your panties in the dream folder
2. Run patch.py `python patch.py`
3. Put your pantie name
4. Enjoy

## Bra conversion for Quiche/Linz
convert_bra.py generates a bra automatically. You just run the following command.  
`python convert_bra.py`  
It converts the latest pantie to bra. When you want to set the number which you want,  
`python convert_bra.py --num 101`  
That's it. Of course, there is a nice option to generate size and position optimized bra,  
`python convert_bra.py --num 101 --pad`  
You just set `--pad` option like this.

### Options
* --num: You can set the number which you want.
* --all: It converts the all panties to bra. When you set num option, it is a start number.
* --pad: Enable padding for easy overlaying.
* --lace: It enables lace decoration instead of frill.

The following options are made for designers who want to design by yourself.
* --disable_ribbon: It disables ribbon pasting.
* --disable_decoration: It disables race and frill decoration.
* --disable_shading: It disables auto shading.
* --disable_texture: It disables texture painting on the base of bra.

## Converted examples
|||
|:-:|:-:|
|[Shaclo](https://tomori-hikage.booth.pm/items/987296)|[Anna](https://wakonoatorie.booth.pm/items/1067958)|
|![test](./sample/shaclo_pantie.png)|![test](./sample/anna_pantie.png)|
|[Milk](https://komado.booth.pm/items/1209496)|[Lua](https://ficsnade.booth.pm/items/1255054)|
|![test](./sample/milk_pantie.png)|![test](./sample/lua_pantie.png)|
|[Ukon](http://seiga.nicovideo.jp/seiga/im8378009)|[Mishe](https://ponderogen.booth.pm/items/1256087)|
|![test](./sample/ukon_pantie.png)|![test](./sample/mishe_pantie.png)|
|[Fuzzy](https://nagatorokoyori.booth.pm/items/1255283)|[Anna light](https://wakonoatorie.booth.pm/items/1405336)|
|![test](./sample/fuzzy_pantie.png)|![test](./sample/anna_light_pantie.png)|
|Bra for Quiche and Linz (Frill)|Bra for Quiche and Linz (Lace)|
|![test](./sample/bra_frill.png)|![test](./sample/bra_lace.png)|
|[Lua for Quest](https://ficsnade.booth.pm/items/1414368)|[Tanu](https://udonfactory.booth.pm/items/1414433)|
|![test](./sample/lua_quest_pantie.png)|![test](./sample/tanu_pantie.png)|

# Any error?
## Windows
Open your favorite terminal and then `pip install -r requirements.txt`.
## Linux/OSX
`pip install -r requirements.txt` or `sudo pip install -r requirements.txt`

# Special thanks
[Quiche model](https://mutachannel.booth.pm/items/954376)  
Developer of the Ukon pantie converter: [thakyuu](https://github.com/thakyuu)
Improvement of patch.py:[4hiziri](https://github.com/4hiziri)  

# License for my images
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work by <a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/tenteeeee_vrc" property="cc:attributionName" rel="cc:attributionURL">TenteEEEE</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.  
When you want to use it on your business, please ask [@tenteeeee_vrc](https://twitter.com/tenteeeee_vrc).

# License for my scripts
Released under the MIT license  
https://opensource.org/licenses/mit-license.php  
Copyright (c) 2019 TenteEEEE  
