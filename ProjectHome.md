★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★
★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★

## NOTE: As of 6/30/2013, this project has migrated to SourceForge: ##
**https://sourceforge.net/projects/jnovelformatter**

★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★
★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★★

## Description ##
JNovel Formatter is a utility that will convert Japanese novels
to nicely formatted HTML files.

## Features ##

  * Most novel encodings are supported (SHIFT-JIS, UTF-8, UTF-16, etc.). The output HTML will be encoded in UTF-8.

  * Supports Aozora formatting （青空文庫形式）, including:
    * Ruby/furigana （ルビ・振り仮名）. Kana that are placed over kanji to indicate pronunciation.
    * Emphasis （傍点）. Marks or dots used to emphasize a word or passage.
    * Images （挿絵）
    * Underlining （傍線）
    * Gaiji （外字）
    * The following formatting constructs are not useful or not currently supported and will be removed:
      * Comments （コメント）. Comments are found between the 2 dashed lines at the start of the novel.
      * Indentation （字下げ、地上げ、中央揃え）
      * New page （改ページ）
      * ［＃改丁］

> Note: Not all browsers support ruby by default:
    * Firefox requires the HTML Ruby add-on: https://addons.mozilla.org/en-us/firefox/addon/html-ruby/
    * Opera requires the HTML Ruby for Opera extension: https://addons.opera.com/addons/extensions/details/html-ruby/7.1.1/
    * IE and Chrome both have out-of-the-box support.

  * Option to add bookmark anchors to "。" characters. Just click a "。" character and bookmark the page. When you load the bookmark, the page will return to the sentence that you left off at.

  * Option to break up the novel into smaller files that won't hose up your browser.

  * Options to change the HTML style (font, colors, alignment, etc.).

  * Can process a single novel or an entire directory of novels.

  * No installation required.

## Screenshot ##

![http://jnovel-formatter.googlecode.com/files/Screenshot.png](http://jnovel-formatter.googlecode.com/files/Screenshot.png)

## How to Run: ##

1) Unzip.

2) In the unzipped JNovel Formatter folder, double-click
> JNovelFormatter.exe.

> Note: You must have the .Net Framework 3.5 installed.


## Feedback Thread ##
Post comments/suggestions/bugs/questions here:
http://forum.koohii.com/viewtopic.php?id=7486


## Special Thanks To ##
  * iSoron/pm215: Authors of the original aozora ruby to HTML code.
  * nest0r: Unofficial systems engineer and all-around helpful person.
  * http://a2k.aill.org/: Gaiji code to UTF-8 table.


## Version History ##
[6.0 (03-07-2012)](Version.md)
  * Added button for selecting an input directory.
  * Optimized emphasis conversion. Now ~2 times faster.
  * Added support to convert ※［＃歌記号］  --->  "〽"
  * Added support to remove ［＃改丁］
  * Added better support to remove aozora indentation
  * Added support for image that begin with ［＃表紙

[5.0 (03-06-2012)](Version.md)
  * Added ability to recursively process all files contained within a folder and its subfolders.
  * Added option to split output file based on character length and an option to not split at all.
  * Added CSS placement options.
  * Added option to set the ruby color
  * Added Webbrowser-based sample. Old textbox-based sample was unable to show ruby color and margin.
  * Made index file a bit more compact.
  * Fixed crash conditions in the ruby and underline code.

[4.0 (04-06-2011)](Version.md)
  * Added feature to replace aozora gaiji codes with UTF-8 equivalents.
  * Added feature to support aozora underline constructs.
  * Added feature to remove the comment between the dashes at the head of the novel.
  * Added feature to remove some more unsupported aozora constructs: bottom indent and center.
  * Remove fonts that start with "@" from the font dropdown.
  * Changed the "Readings/Ruby" option to  "Aozora Formatting".
  * Fixed index file sometimes creating too many links.
  * The Open Directory button on the Complete dialog now also closes the dialog.

[3.1 (02-13-2011)](Version.md)
  * Fixed issue with non-TrueType fonts not being inserted into the HTML files. Note: non-TrueType fonts still don't work with the preview.
  * Added feature to copy any images referenced in either Aozora formatting or HTML img tags to the output directory.
  * The Remove readings option now removes the "｜" character too.

[3.0 (02-11-2011)](Version.md)
  * Added Linux support.
  * Added aozora ruby support (Example: 武州｜青梅《おうめ》の宿) .
  * Added aozora emphasis support (Example: 胡麻塩おやじ［＃「おやじ」に傍点］).
  * Added aozora image support (Example: ［＃挿絵（img/imagename.jpg）入る］).
  * The following aozora format constructs are removed:
> > ［＃改ページ］
> > ［＃ここからnumber字下げ］
> > ［＃ここで字下げ終わり］
  * Program will no longer separate pages in the middle of a sentence.
  * Margin now affects only left and right of page.
  * Catches and ignores exception about only TrueType fonts being supported. (Let me know if you still get the error).
  * The Complete Dialog's button now leads to the directory with the HTML files
> > instead of the directory above that.

[2.0 (02-08-2011)](Version.md)
  * Added HTML5 ruby tag option for readings
  * Input encoding is now user selectable

[1.0 (02-07-2011)](Version.md)
  * Initial release.
