# SourceListGenerator

A VCSSL script for generating a list file for compiling multiple Java&reg; source files, packages, and so on - 複数のJava&reg;ソースファイルやパッケージ等をコンパイルする際のリストファイルを生成するVCSSLスクリプト

## Abstract - 概要

When you want to compile multiple java source files or packages whithout build-tools or IDEs, you may describe pathes of all source files in a file (e.g. sourcelist.txt), and specify it to the javac command as follows:

複数のJavaソースファイルやパッケージを、ビルドツールやIDEを用いずにコンパイルしたい場合、全ファイルのパスをファイル（例えば sourcelist.txt ）の中に記述して、それを javac コマンドに指定する事ができます：

    javac @sourcelist.txt

This repository provides/manages a script "SourceListGenerator.vcssl" which can generate the above list file (sourcelist.txt) automatically. This script is practically used in other repositories of RINEARN ( e.g. : <a href="https://github.com/RINEARN/vnano/tree/master/src">&quot;src&quot; directory of the Vnano</a> ).

このリポジトリは、上記のリストファイル（sourcelist.txt）を自動生成するスクリプト「 SourceListGenerator.vcssl 」を提供/管理します。
このスクリプトは、RINEARNの他のリポジトリ内（ 例： <a href="https://github.com/RINEARN/vnano/tree/master/src">Vnanoの「src」フォルダ</a> など ）において実際に使用しています。

## License - ライセンス

This script is released under CC0.

このスクリプトは CC0 で公開されています。


## Requirements - 必要なもの

- Java Runtime Environment (8 or later) - Java実行環境（8以降）


## How to Use - 使用方法

### Step-1. Put the Script - スクリプトの配置

At first, put the script "SourceListGenerator.vcssl" in your source code directory. 
Subdirectories will be traversed recursively, so put the script at the top hierarchy in the tree of source code directories.

はじめに、スクリプト「 SourceListGenerator.vcssl 」を、ソースコードディレクトリの直下に配置します。
サブディレクトリは再帰的に探索されるため、最上階層のソースコードディレクトリに配置してください。

### Step-2. Downlaod VCSSL Runtime and Extract - VCSSLランタイムのダウンロードと展開

Then, download the runtime environment of the VCSSL (VCSSL Runtime) from: https://www.vcssl.org/en-us/ . Extract the downloaded ZIP file "vcssl_\*\_\*\_\*.zip" (where \*\_\*\_\* are version numbers) from right-click menu.

&raquo; <a href="https://www.vcssl.org/en-us/info/help#extract_error">If the extraction of the downloaded ZIP file is stopped with the error message...</a>


次に、以下のページからVCSSLの実行環境（VCSSLランタイム）をダウンロードします: https://www.vcssl.org/ja-jp/ . ダウンロードしたZIPファイル「 vcssl_\*\_\*\_\*.zip （ \*\_\*\_\* はバージョン番号 ）」を、右クリックメニューから展開してください。

&raquo; <a href="https://www.vcssl.org/ja-jp/info/help#extract_error">ZIPファイルを展開中にエラーで止まってしまう場合は...</a>


### Step-3. Execute the Script - スクリプトの実行

Finally, launch the VCSSL Runtime and execute the script "SourceListGenerator.vcssl".
VCSSL Runtime can be launched on the command line as follows:

    cd <extracted_directory_of_VCSSL_runtime>
    java -jar VCSSL.jar

最後に、VCSSLランタイムを起動してスクリプト「 SourceListGenerator.vcssl 」を実行します。
VCSSLラインタイムは、コマンドラインから以下のように起動できます：

    cd <展開されたVCSSLランタイムのフォルダ>
    java -jar VCSSL.jar

Just after the VCSSL runtime will be launched, a file choosing dialog will be displayed, so choose the script "SourceListGenerator.vcssl" which was put in your source code directory at the step-2. Then the script will be executed and "sourcelist.txt" will be output in the same directory.

VCSSLランタイムを起動すると、ファイル選択画面が表示されます。そこで Step-2 でソースコードディレクトリに配置したスクリプト「 SourceListGenerator.vcssl 」を選択してください。すると、スクリプトが実行され、出力ファイル「 sourcelist.txt 」が同じディレクトリ内に生成されます。


---

## Credits - 本文中の商標など

- Oracle and Java are registered trademarks of Oracle and/or its affiliates. 

- Other names may be either a registered trademarks or trademarks of their respective owners. 

- OracleとJavaは、Oracle Corporation 及びその子会社、関連会社の米国及びその他の国における登録商標です。文中の社名、商品名等は各社の商標または登録商標である場合があります。

- その他、文中に使用されている商標は、その商標を保持する各社の各国における商標または登録商標です。




