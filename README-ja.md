PXrubrica パッケージ
====================

LaTeX: 日本の慣習に従ったルビ（振り仮名）出力

JIS 規格「JIS X 4051」および W3C 技術ノート「[日本語組版処理の要件]」
で述べられているような、日本において一般的な様式に従ってルビを付ける
機能を提供する。

[日本語組版処理の要件]: <http://www.w3.org/TR/jlreq/ja/>

### 前提環境

  * フォーマット： LaTeX
  * エンジン： pTeX／upTeX／LuaTeX／XeTeX
  * DVI ウェア： pTeX 対応のもの

### 構成物

  * `pxrubrica.pdf`： 説明書
  * `pxrubrica.dtx`： DocStrip ソースファイル
  * `pxrubrica.ins`： DocStrip インストーラファイル
  * `pxrubrica-en.pdf`： 英語版の説明書
  * `pxrubrica-en.tex`： 英語版の説明書(ソース)
  * `sample/*.tex`： サンプル文書

### インストール

アーカイブにパッケージファイル（`*.sty`）が含まれていない場合は、
以下のコマンドを実行して生成する。

    ptex -kanji=jis pxrubrica.ins

その後、各ファイルを次の場所に移動する。
（TDS 1.1 に従ったシステムの場合。）

  - `*.sty`         → $TEXMF/tex/platex/pxrubrica/
  - `*.dtx`/`*.ins` → $TEXMF/source/platex/pxrubrica/
  - `*.pdf`/`*.tex` → $TEXMF/doc/platex/pxrubrica/

### ライセンス

MITライセンスの下で配布される。

更新履歴
--------

  * Version 1.1  〈2017/04/10〉
      - XeTeX／LuaTeX のサポート。
      - 両側ルビの処理を改良。
      - バグ修正
  * Version 1.0a 〈2014/12/23〉
      - バグ修正
  * Version 1.0  〈2012/04/30〉
      - 最初の公開版

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/
