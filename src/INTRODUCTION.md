# はじめに

本資料は、Scala初学者向けの学習テキストです。本資料を読み進めることで、

* プログラミング言語Scalaを用いたアプリケーションを開発できるようになること
* [『Scala スケーラブルプログラミング』（第三版）](https://book.impress.co.jp/books/1116101021)（通称コップ本）を通読して理解できるようになること
* [『Scala関数型デザイン&プログラミング ―Scalazコントリビューターによる関数型徹底ガイド』](https://book.impress.co.jp/books/1114101091)（通称FP in Scala）を通読して理解できるようになること

が主な目的です。

『Scalaスケーラブルプログラミング』は、Scalaの言語設計者であるOderskyさんらにより書かれた解説書で、Scalaの言語機能について詳細に書かれており、Scalaプログラマにとってはバイブルと言える本です。
この本は決して読みにくい本ではないのですが、本の分量が多いのと、関数型など他の言語でのプログラミング経験がないとわかりにくい箇所があります。
本テキストを通じてScalaに入門することによって、この『コップ本』も読みやすくなるでしょう。

『Scala関数型デザイン&プログラミング』は、[Scalaz](https://github.com/scalaz/scalaz)[^scalaz]コントリビューターであるPaul Chiusanoさん、Rúnar Bjarnasonさんらにより書かれた関数型プログラミングについての本です。あくまで関数型プログラミングの本なのでScalaやScalazについての解説はあまりありません。ただしScalaについての最低限の文法の説明は随時行われています。「本文中で一から自作」というスタンスが徹底されており、型クラスのみならず、List、Stream、Futureなど、Scala標準ライブラリに存在するものまで、一から自作しています。そのため「単にパターンを覚えて使う」のではなく、それぞれの関数型の色々な型クラスやパターンが「なぜそういう仕組になっているのか？」という根本的な考え方が分かるようになっています。
細かいScala自体の言語仕様やテクニック、（標準ライブラリと外部のライブラリ含めた）既存の実在するライブラリの使い方は一切説明せず、とにかく「考え方や概念」のみを重点的に説明しているので、この本を読んで身につけた知識は古くなりにくいという点でおすすめできる一冊です。

読者層としては、

* 大学の情報学部卒である
* Java言語の基本知識がある
* 何か意味のあるアプリケーションを作ったことがある
* 趣味でTwitter APIなどを触ったり、プログラミングを行っている

人（相当）を仮定しています。なお、上記の指標はこの資料を読むにあたってのあくまで目安であり、特に大学の情報学部卒
でなければ理解できないといったことはありません。ただし、本資料は1つ以上のプログラミング言語でアプリケーションを
作れることを最低限の前提にしていますので、その点留意ください。

## フォーマット

このテキストは下記のフォーマットで提供されています。

* HTML版：https://scala-text.github.io/scala_text/
* PDF版：https://scala-text.github.io/scala_text_pdf/scala_text.pdf
* EPUB版：https://scala-text.github.io/scala_text/scala_text.epub

## フィードバック
* 誤字・脱字の指摘や修正、および明確な技術的誤りの指摘や修正：
  * [scala_text](https://github.com/scala-text/scala_text)のissue欄およびpull requestへ
* それ以外の改善要望や感想：
  * [専用issue](https://github.com/scala-text/scala_text/issues/235)へ

よろしくお願いいたします。

## ライセンス

本文書は、[CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/deed.ja)

![CC-BY-NC-SA](https://licensebuttons.net/l/by-nc-sa/3.0/88x31.png)

の元で配布されています。ただし、直接の利益を得ることを目的としない研修などに利用することは可能とします。
直接の利益というのは、研修自体を実費以上の金額で提供する行為を指します。社内でのScala研修などは一般的に
直接の利益を得ることを目的としないので、断りなく使っていただいて構いません。

[^scalaz]: 関数型プログラミングを行うための純粋なデータ構造や、ファンクターやモナドといった型クラスとそのインスタンスを提供するライブラリのこと。

## 謝辞

本資料は、ドワンゴ社が作成した新卒エンジニア向けのScala研修資料が日本のScalaコミュニティに寄贈されたものです。