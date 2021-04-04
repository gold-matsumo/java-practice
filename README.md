
# java練習環境のインストール
今回は練習環境のため、「dokojava」を使ってもいいが後々のためにローカル環境を用意する。
dokojavaは簡単なものなら問題ないが機能制限がある。
「dokojava」→https://dokojava.jp/
# 環境
Windows10
## 方法1.JDK単体
### OSを確認
Windowsキー+X　からシステム→詳細情報→システムのシステムの種類を確認、32bitか64bitかを確認する。
### サイトへ
OracleのサイトからJDKをダウンロード、今回はjava SE 16を使う。Windows x64 Installerをダウンロードする。後々インストールした場所が必要になるので覚えておく（デフォルトならC直下のProgram　Fileのところだと思う）
Oracleのサイト→https://www.oracle.com/java/technologies/javase-downloads.html
### 環境変数を変える（Path）
Windowsキー＋R　から”sysdm.cpl”打ち込むと環境変数の設定画面へ　システムの詳細設定→環境変数へ　
Pathをクリック→編集→新規を押し、binファイルへのパスを書き込む（例：C:￥Program Files￥Java￥jdk-16￥bin）
### 環境変数を変える（HOME）
環境変数画面に戻り、新規を押すと”新しい環境変数名”というのが出てくるので変数名にJAVA_HOME　変数値にjdk-16のファイルパスを書きこむ（C:￥Program Files￥Java￥jdk-16）
### 確認
コマンドプロンプトを開き”javac -version”を叩いて、結果が”javac 16”と出ればOK
### 参考
https://dan-chan.com/java-update-07/
## 方法2.IDEを使う
今回は学習のため、無料オープンソースのintelij IDEA EDUを使う。
### ダウンロード
ダウンロードページの下の方にあるintelij　EDUの案内からダウンロードする。
ダウンロードページ→https://www.jetbrains.com/ja-jp/idea/download/#section=windows
### 終わり
あとはインストールを進めればOK、PCによっては管理者権限で開く必要あり。
## 方法3.プラグイン入りIDEを使う
euripus日本語化プラグインが入っているPleiadesを使う。
### ダウンロード
今回は最新版の2021年版を使う（Windowsは7zipで解凍しないとだめらしい）
Pleiadesダウンロードページ→https://mergedoc.osdn.jp/
### 解凍
Zipでダウンロードされるので、解凍後にeclipse.exeを実行すればOK

# 使ってみた感じ
全部触ってみた結果、よほどのことが無い限りはIDEかプラグイン入りIDEを使うべきだと感じた。JDKのみは導入も複雑で、ライブラリの追加などプログラムそのもの以外に覚えることが多すぎる。根本的なシステムへの理解を深めるにはJDKのみも触ってみていいと思う。
