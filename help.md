$Header: fe.hlv  2.3  95/09/13 21:02:12  Hong.Chen  Rel $
_______________________________________________________________________

            ＰＣ／ＡＴ
            ＰＣ－９８　    　シリーズ汎用　ファイル管理ツール
            ＦＭーＲ

                        ■■■■■  ■■■■■
                        ■          ■      
                        ■          ■      
                        ■■■■    ■■■■
                        ■          ■      
                        ■          ■      
                        ■ iler &   ■■■■■ditor  Ver. 2.03

                     オンライン・操作マニュアル

			 1995年9月13日

		Copyright (C) 1989-1995 , Chen Hong
_______________________________________________________________________

１  【操作・オンライン・マニュアルについて】

２  【キー操作方法及び共通コマンド】

2-1  [/]               コマンドメニュー
2-2  [INS]             画面のリフラシュ
2-3  [ User cmd ]      ユーザー登録コマンドの実行
2-4  [ delete Bakfile] ＢＡＫファイルの削除
2-5  [ Sort   ]        ファイルの並び替え
2-6  [ Option ]        システムオプションの設定
2-7  [ Group  ]        ワールドカードの指定

３  【ディレクトリ画面操作方法】

3-1　[ Logdisk][1..9]  ドライブの変更
3-2　[ Copy   ]        ファイルのコピー
3-3  [ Information ]   ディスクのインフォメーション表示
3-4  [ Find   ]        ファイルの検索表示
3-5  [ Deldir ]        ディレクトリの削除
3-6  [ Mkdir  ]        ディレクトリの作成
3-7  [ Rendir ]        ディレクトリ名の変更
3-8  [ disk copyWrite ]ディスクコピー
3-9  [ eXec   ]        COMMAND.COM実行
3-10 [ lha Pack file ] ディレクトリファイルの凍結

４  【ファイル画面操作方法】

4-1　[ eXec   ]        プログラムファイルの実行
4-2　[ Copy   ]        ファイルのコピー、まだはファイルの移動
4-3  [ Rename ]        ファイル名の変更
4-4　[ Delete ]        ファイルの削除
4-5  [ Attr   ]        アトリビュートの変更
4-6  [ P.P.C  ]        ファイルのフォーマット付き印刷
4-7  [ Editor ]        ファイルの編集
4-8  [ Viewer ]        ファイルを見る
4-9  [ Timestampe ]    タイムスタンプの変更
4-10 [ Lha Pack file ] ファイルの凍結
_______________________________________________________________________

１ 【操作・オンライン・マニュアルについて】
==========================================

  FE 2.01から追加した機能です。
　ディレクトリ画面、ファイル画面で[？]キー押せば何時でもこの「操作・オン
ライン・マニュアル」見ることが出来ます。


２ 【キー操作方法及び共通コマンド】
==================================


	画面変更は[RET]と[ESC]キーで行う。
                  [TAB]  [BS]

          ･--------------------･      ･--------------------･
          |ディレクトリ画面操作|      | ファイル画面操作   |
          ･--------------------･      ･--------------------･
  ･-･ FE  |L:Log Disk          |[RET] |P:Print text        |[RET] ･----･
　| |---->|F:Findfile under dir|----->|R:Rename            |----->|エ内|
  |D|     |M:Make new dir      |[TAB] |A:Attribute change  |[TAB] |デ蔵|
  |O|     |D:Delete            |      |C:Copy .or. move   +|      |ィ簡|
  |S|[ESC]|C:Copy dir tree     | [ESC]|T:Touch file       +| [ESC]|タ易|
  | |<----|I:disk Information  |<-----|D:Delete           +|<-----･----･
  ･-･[BS] |W:disk copyWrite    | [BS] |L:Lha pack(Ext.Cmd)+| [F1]
          |P:lha Pack(Ext.cmd) |      |E:Edit    (Ext.Cmd) |
          |R:Rename  (Ext.cmd) |      |V:Viewer  (Ext.Cmd) |
          |X:eXecute (Ext.Cmd) |      |X:eXecute (Ext.Cmd) |
          |S:dir Sort(Ext.Cmd)*|      |S:dir Sort(Ext.Cmd)*|
          |U:User def(Ext.Cmd)*|      |U:User def(Ext.Cmd)*|
          |B:kill[.Bak,%]file *|      |B:kill[.Bak,%]file *|
          |O:system Option    *|      |O:system Option    *|
          |G:set   fileGroup  *|      |G:set   fileGroup  *|
          ･--------------------･      ･--------------------･

            *) は両画面共通コマンド
            +) はスペースバーで処理対象ファイルリスト選択可能なコマンド


2-1 [/]:コマンドメニュー

　　コマンドの実行するには, 直接コマンドキーワード入力しでも実行されるが、
　　「/］を押すとコマンドメニュー表示されで、選択してから[RET]を押すと同
    じことできる。（初心者向き？）


2-2 [INS]　画面のリフラシュ

        【基本キー操作】  [INS]

　　押すとDOS の画面が表示する。 も一回押すとＦＥの画面に戻る。
　　画面乱れるとき等[INS]２回押すと画面リフラシュになる。


2-3 [ User cmd ]　ユーザー登録コマンドの実行

        【基本キー操作】  [U]

　　　押すとユーザー登録コマンドメニュー表示されで、選択してから [RET]を
    押すと実行できる。
　　15個のユーザーコマンドが登録できる.
　　プログラムの登録及び変更はエディタを使って FE.CFGを直接編集する．


2-4 [delete Bakfile]  ＢＡＫファイルの削除

        【基本キー操作】  [B]

    *.BAK, %*	ファイルが削除される (%*はMIFES のDUMMY ファイル).


2-5  [ Sort   ]        ファイルの並び替え

        【基本キー操作】  [S]

　　外部コマンドに依存する。
    同梱している FE.CFG にはデフォルト設定が記入されている．


2-6  [ Option ]        システムオプションの設定

        【基本キー操作】  [O]

　　1. ターゲット文書コードタイプ設定
	( 起動オプション -K 参照 )

  　2. 表示行数の指定．
	( 起動オプション -L 参照 )

  　3. ファイルの名前表示順の指定．


2-7  [ Group  ]        ワールドカードの指定

        【基本キー操作】  [G]

　　画面上ファイル表示グループのワイルドカード指定。
　　画面表示以外、コピーコマンドにも影響する。


３ 【ディレクトリ画面操作方法】
==============================

　　カレントドライブのツリー構造を表示する．
　　検索可能なディレクトリの総数は 400 以下である．
　　また階層は無制限に検索するが，表示文字数の関係で 8 ～ 10階層になると
  正常な表示がされない場合がある．
　　表示するファイルの拡張子は [G]コマンド設定したワールドカードに影響さ
  れる。


3-1　[ Logdisk ][1..9] ドライブの変更

        【基本キー操作】  [L] [1]..[9]

  　[L] を入力すると，移動先ドライブ名をたずねてきる．ここで変更したいド
  ライブを入力するか選択すると，そのドライブのディレクトリを検索しツリー
  を表示する．
    数字キー押すと直接対応ドライブへ変更する。
　　[1] --> [A]
　　[2] --> [B]
    ...
　　[9] --> [I]


3-2　[ Copy   ] ファイルのコピー

        【基本キー操作】  [C]

　　コピーしたいファイルをカーソルキーで選び，[C] を入力する．コピー先の
  ディレクトリ、日付のチェック、サブディレクトリのコピー等を聞いてくるの
  で，入力して[RET]を押すとコピーを開始する．
　　ドライブのみを指定すると，指定ドライブのカレントディレクトリになるの
  でルートディレクトリの場合は必ず最後に \ が必要である．
　　[TAB] を押すとディレクトリ、ドライブの選択ができます。この方が誤入力、
  誤動作する確率小さいのでお勧めします。直接ディレクトリ、ドライブ入力時、
  絶対パス名指定の方がお勧めする．
　　もしコピー先にディレクトリが不存在の場合に，１つ以下の階層に限りサブ
  ディレクトリを作ってコピーする．
　　転送先の空き容量不足の時にはコピーを中止する．また，コピーの対象にな
  るファイルは，全ての属性のファイルである．
　　[G] コマンド設定したワールドカードに影響される。


3-3  [ Information ] ディスクのインフォメーション表示

        【基本キー操作】  [I]

　　ディスクの容量，クラスタサイズ等の，各種情報を表示する．


3-4  [ Find   ] ファイルの検索表示

        【基本キー操作】  [F]

　　[F] を押すと，ワイルドカードでのファイル検索表示モードになる．適当な
  ワールドカードを使用して検索表示が出来る（*.log , ujo*.* 等）.


3-5  [ Deldir ] ディレクトリの削除

        【基本キー操作】  [D]

　　このコマンドでは，サブディレクトリが空いてないときディレクトリ内ファ
イル削除するかどうか聞いてくるので，[Y]入力して[RET]を押すと削除を行う．


3-6  [ Mkdir  ] ディレクトリの作成

        【基本キー操作】  [M]

　　[M] を押すと現在の表示ディレクトリの下にサブディレクトリを作成する。


3-7  [ Rendir  ] ディレクトリ名の変更

        【基本キー操作】  [R]

　　外部コマンドに依存する。
    同梱している FE.CFG にはデフォルト設定が記入されている．


3-8  [ disk copyWrite ] ディスクコピー

        【基本キー操作】  [W]

　　ディスクコピーのみ、フォーマットができない.
　　ソースディスクはカレントディスクに固定、ターゲットディスクは選択可能
になっている。ディスク照合はしない.


3-9  [ eXec  ] COMMAND.COM実行

        【基本キー操作】  [X]

    [X] を押すと，COMMAND.COM が起動するのでここでDOS のコマンドの実行が
  出来ます．なお『ＦＥ』に戻るには EXIT と入力してください．


3-10 [lha Pack file]  ファイルの凍結

        【基本キー操作】  [P]

　　[P] を入力すると凍結の格納ファイル名を聞いてくるので，入力して[RET]
　を押すと凍結を開始する．
　　なお圧縮ツールの起動には FE.CFG で使用する圧縮ツールを設定しておく。
  パスの通ったディレクトリに存在しないと圧縮ツールは起動しません．


４ 【ファイル画面操作方法】
==========================
　　カレントディレクトリのツリー構造を表示する．
　　なお，扱えるファイルの最大値は 400である，これ以上同一ディレクトリに
  ファイルがあると無視される。
　　[G]コマンド設定したワールドカードに表示が影響される。
　　スペースキーによりファイルの選択ができる。[DEL] によりファイル選択の
  全解除、全選択もできる。


4-1　[ eXec   ] プログラムファイルの実行

        【基本キー操作】  [X]

　　実行させたいファイルをカーソルキーで選び，[X] を入力すると．拡張子が
　FE.CFGに指定した場合には自動的に実行する。その他では必要なときはパラメ
　ータも付加してから [RET]キーで実行させる．
　　同梱している FE.CFG にはデフォルト設定が記入されている．


4-2　[ Copy   ] ファイルのコピー、まだはファイルの移動

        【基本キー操作】  [C]

　　コピーしたいファイルをカーソルキーで選び，[C] を入力する．
　　コピー先のディレクトリ名、[COPY|UPDATE|MOVE]等のコピー条件等を聞いて
　くるので，入力して[RET]を押すとコピーを開始する．
　　ドライブのみを指定すると，指定ドライブのカレントディレクトリになるの
　でルートディレクトリの場合は必ず最後に \ が必要である．
　　[TAB] を押すとディレクトリ、ドライブの選択ができます。この方が誤入力、
  誤動作する確率小さいのでお勧めします。直接ディレクトリ、ドライブ入力時、
  絶対パス名指定の方がお勧めする．
　　スペースで選択されたすべでファイルに対して操作を行う。

　1.[COPY]の場合
　　コピー先に同名ファイルがあると上書きする、コピー時には転送先の空き容
  量を調べて容量不足の時にはコピーを中止する．また，コピーの対象になるフ
  ァイルは，全ての属性のファイルである．

　2.[UPDATE]の場合
　　コピー先に同名ファイルがあるとコピー元が新しい場合のみコピーをする。

　3.[MOVE]の場合
　　移動先が同一ドライブであれば，ディレクトリエントリの変更のみを行うの
　で高速にファイルの移動が行える、但し移動先に同名ファイルが存在するとき
　は，そのファイルは移動されませんので，必要に応じて [ Copy ]と[ Delete]
　で移動して下さい．
　　移動先が違うドライブの場合は単に [ Copy ]と[ Delete]を続けて実行する
　だけである．


4-3  [ Rename ] ファイル名の変更

        【基本キー操作】  [R]

　　ファイルの名の変更です。同一ドライブ内ファイルの移動もできる。


4-4　[ Delete ] ファイルの削除

        【基本キー操作】  [D]

　　削除したいファイルをカーソルキーで選び，[D] を入力する．
　　スペースで選択されたすべでファイルに対して操作を行う。



4-5  [ Attr   ] アトリビュートの変更

        【基本キー操作】  [A]

　　アトリビュートは変更したい属性の位置に [↑/↓]でカーソルを移動して，
  [←/→]で属性が反転する．
　　実際の変更は [RET] を押すと実行される，中止するときは [ESC] を押して
  下さい．
　　スペースで選択されたすべでファイルに対して操作を行う。


4-6  [ P.P.C    ] ファイルのフォーマット付き印刷

        【基本キー操作】  [P]

　　印刷オプション入力画面表示する
　　印刷は [RET] を押すと実行される，中止するときは [ESC] を押して下さい．


4-7  [ Editor ] ファイルの編集

        【基本キー操作】  [E]

　　編集したいファイルをカーソルキーで選び，[E] を入力する．
　　なおエディターの起動には fe.CFG で使用する起動エディターを設定してお
  く。パスの通ったディレクトリに存在しないとエディターは起動しません．


4-8  [ Viewer ] ファイルを見る

        【基本キー操作】  [V]

　　見たいファイルをカーソルキーで選び，[V] を入力する．
　　なおビューアの起動には fe.CFGで使用するビューアを設定しておく。 パス
  の通ったディレクトリに存在しないとビューアは起動しません．


4-9  [ Timestampe ] タイムスタンプの変更

        【基本キー操作】  [T]

　　タイムスタンプの変更はまず [↑] / [↓]でカーソルを日付か時間の位置に
  移動して，数字を入力する．
　　実際の変更は [RET] を押すと実行される，中止するときは [ESC] を押して
  下さい．あり得ない日付を入力しないように（ 2月31日等），注意してくださ
  い．


4-10 [Lha Pack file]  ファイルの凍結

        【基本キー操作】  [L]

　　凍結したいファイルをカーソルキーで選び，[L] を入力する．
　　凍結の格納ファイル名を聞いてくるので，入力して[RET] を押すと凍結を開
  始する．
　　スペースで選択されたすべでファイルに対して操作を行う。
　　なお圧縮ツールの起動には FE.CFG で使用する圧縮ツールを設定しておく。
  パスの通ったディレクトリに存在しないと圧縮ツールは起動しません．

************************************************************************

　マニュアルの自分見易いように修正もできますが、修正したものは再配布は
ご遠慮下さい。

　オンライン・操作マニュアルについて御意見，御感想，御要望などは作者宛
メールで是非御連絡ください．

				作  者: Hong Chen (陳 泓)
				連絡先: chen@hako.is.uec.ac.jp
                                        GFG04511@niftyserve.or.jp
