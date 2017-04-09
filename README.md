PXrubrica Package
=================

LaTeX: Ruby annotations according to JIS X 4051

This package provides function to add ruby annotation (furigana) that
follows the style conventional in Japanese typography, as described in
the W3C technical note “Requirements for Japanese Text Layout” ([JLREQ])
and the JIS specification JIS X 4051.

[JLREQ]: <http://www.w3.org/TR/jlreq/>

### SYSTEM REQUIREMENTS

  * TeX format: LaTeX.
  * TeX engine: pTeX and its derivatives.
  * DVI driver: Anything that supports pTeX DVI.

### CONTENT

  * `pxrubrica.pdf`: the manual in Japanese
  * `pxrubrica.dtx`: DocStrip source file
  * `pxrubrica.ins`: DocStrip installer file
  * `pxrubrica-en.pdf`: the brief manual in English
  * `pxrubrica-en.tex`: the brief manual in English (source)
  * `sample/*.tex`: sample documents

### INSTALLATION

If the archive does not contain the packge file (`*.sty`), then you
must run the command to create it:

    ptex -kanji=jis pxrubrica.ins

Then move the files as follows (in a system compliant to TDS 1.1):

  - `*.sty`         → $TEXMF/tex/platex/pxrubrica/
  - `*.dtx`/`*.ins` → $TEXMF/source/platex/pxrubrica/
  - `*.pdf`/`*.tex` → $TEXMF/doc/platex/pxrubrica/

And rehash your TEXMF trees if necessary.

### LICENSE

This package is distributed under the MIT License.

Revision History
----------------

  * Version 1.1  〈2017/04/10〉
      - Support for XeTeX/LuaTeX.
      - Improve the process of two-side ruby.
      - Bug fix.
  * Version 1.0a <2014/12/23>
      - Bug hix.
  * Version 1.0  <2012/04/30>
      - First public release.

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/
