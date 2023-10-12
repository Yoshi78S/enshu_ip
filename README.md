# 情報システム工学II 画像処理　インストラクション

## 演習資料
まずは、演習資料`docs/intro.pdf`を読もう。

---
## 課題
OpenCVを使って、なにか「**自分（あるいは誰か特定のユーザ）が得する**」システムを作る！

最低限の条件：
- 画像処理を活用するプログラムであること。
- 諸々の資料を参考にしたり組み合わせるのは良いが、そのままコピーするのはダメ（`tutorial.ipynb`の内容は除く）。
- 参考にした資料があるなら、レポート中に（引用として）書いておくこと。

上記、最低限の条件を守りながら、自由な発想で画像処理アプリを作成しよう。

好ましい条件：
- 実験用素材（入力画像など）は、構築したアプリを良くアピールできるような例を自分で撮影すると良い。
- レポートに、うまくいく例、うまくいかない例を示し、うまく行かない例を改善するための可能性を考察する。
- しっかりした問題意識や需要に基づくアプリの提案。ただし、その問題や需要が一般的であるかどうかは一切問わない。
- ユニークな発想。

---

## 実行方法など

詳細は演習資料を参照。

### インストール
Python3.xは事前にインストールのこと。公式のでOK。Windows Storeなどからもインストール可能。

公式：[https://www.python.org/downloads/](https://www.python.org/downloads/)

チュートリアル周りで必要なライブラリは、以下のコマンドでインストールできる。Anaconda使いたい、venv使いたい、docker使いたい、などの場合は適宜調べてみること（演習資料に、venvの例を掲載している）。
```
$ pip install -r requirements.txt
```

本課題におけるアプリの実装においては、上記のライブラリのみにこだわる必要はない。必要なライブラリは適宜導入して良いが、必ずコード内およびレポートにその旨を記載すること。

### コードやチュートリアルの実行
諸々のインストールが終わったら、以下からjupyter notebookを実行する（あるいは、演習資料にあるようにVSCodeなどのIDEから実行しても良い）。

Pythonコードの実行：
```
$ python3 hello.py
```

Jupyter notebookの実行：
```
$ jupyter notebook
```
まずは、`tutorial.ipynb`を開いてチュートリアルを読みつつ実行してみよう。

---
## 説明資料 `docs/`
演習資料と、スライドによる課題例の説明。
**本課題で作成するのにちょうど良さそう（？）な例を紹介しているのでまずは一読を。**
（もちろん、これらの例に挙げられていないものを作っても良い。むしろ、示された例にとらわれない独創的なアイデアを歓迎する。）

---
## レポート `report/`
レポートテンプレートが`report/08D12345.tex`にあるので参照すること。レポートのフォーマットに関する注意事項や内容例なども記載されている。
参考まで、コンパイル後のpdfは`report/08D12345.pdf`にある。
提出時は`{学籍番号}.pdf`にリネームして提出すること。
- 本レポートの作成にはTeXを使うことを推奨するが、必須ではない。TeX以外を使う場合も、概ねテンプレートのレイアウトを参考にすると良い。
- 添付のテンプレートを使う場合、ページ数は1～2ページ程度を目安とする（が、それより長くても良い）。日本語か英語で記述すること。
- 本レポートのタイトルを、実装したアプリの内容をうまく表現するようなタイトルに適切に変更すること。

---
## 提出方法
本演習では、以下を提出すること。

### ミニレポート・ソースコード（締切はCLEに記載）
`08D12345.py`に実装し、`{学籍番号}.py`にリネームした上で、必要な入力データ（あれば）とあわせて`{学籍番号}.zip`にまとめること。この際、`{学籍番号}.py`を実行したらそのまま読み込める場所に入力データを配置しておくことが望ましい（それが難しい場合はどこかにその旨記載しておくこと）。レポートをコンパイルしたもの（`{学籍番号}.pdf`）と合わせてCLEから提出すること。

つまり、提出物は

- ソースコード（＋必要な入力データ）：`{学籍番号}.zip`
- レポート：`{学籍番号}.pdf`

の2ファイルとなる。


---
## 評価
本演習は、ミニレポート・ソースコードの情報から、実装したアプリの「実用性」「独創性」「完成度」およびレポート記述の「充実度」で評価する。

ここでの「実用性」は、レポートにおいてあなた自身（あるいは特定のターゲットとなるユーザ；架空の存在でも良い）にとっての実用性がきちんと説明されていれば十分である。一般的な観点では実用的と思われづらくとも、あなた自身（あるいは特定のユーザ）が有用であると思い得ることがレポートの記述からわかれば、それで良い。

例えば、「暇つぶし」や「なんとなく楽しい」なども立派な用途である。これらが誰かに有用たり得る背景やシナリオをレポート中で説明することが重要である。

---
## 質問など
質問や相談などは、大倉（[okura@ist.osaka-u.ac.jp](okura@ist.osaka-u.ac.jp)）まで。

### FAQ

**何を作ればよいか思いつかない**

`doc`ディレクトリ以下に、難易度感がちょうど良さそうな例をいくつか紹介したスライドを用意したので、それらに取り組んでも良い。
ただし、それらにとらわれず、自由な発想で取り組むことをおすすめする。

**どれくらいの規模感のものを作れば良い？**

小さいもので構わない。上記のチュートリアルの内容を組み合わせた、あるいは少々書き換えただけのようなものでも、その有用性や実装内容がレポートで十分に説明されていれば問題ない。
ちなみに、`tutorial.ipynb`はあくまで参考資料の一つ、という立ち位置である。
よって、チュートリアルに記載されたコードを使う場合も、それ自体の説明もきちんとレポート中に含めること。


**こういうのが作りたいんだけど、どのように実装すれば良いかわからない**

大倉（[okura@ist.osaka-u.ac.jp](okura@ist.osaka-u.ac.jp)）までお気軽にご相談を。


---
