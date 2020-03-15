# アルファ変換
- ラムダ計算においては束縛変数の名前は重要でないと考えられる
- つまりλx.xとλy.yは同じ関数を表していると言える
- 故にあるラムダ式と他のラムダ式との折り合いをつける時に、上記の様に束縛変数の名前を変更する必要がある
- それをアルファ変換と呼ぶ

# ベータ簡約
- 以下の様な物を可簡約項(β-redex)と呼ぶ
- ((λx.M)N) 
  - これは λx.Nと簡単にすることができる。これをベータ簡約と呼ぶ
- 完全ベータ簡約は任意の簡約基をいつでも簡約できる


## 操作的意味論
振る舞いが遷移関数で定義されるような抽象機械を考え、その遷移関数によって起こる状態変化によって、プログラム各語句の意味を説明する。

### 小ステップスタイル
評価の遷移を1ステップごとに書き出すもの

### 大ステップスタイル(自然意味論)
多数回の評価ステップを通じ最終的にどんな値に評価されるのかを定式化する

## 表示的意味論
プログラムの実行過程を抽象化し、プログラムの入出力を意味領域への数学的な写像に例えて説明する。
表示的意味を与えるということは、「項を特定の意味領域に写すような解釈関数を定義する」ということである。
表示的意味論を用いると、実際のプログラム評価の裏で行われるような生々しい詳細を取り去り、言語の本質的な概念を浮き彫りにすることができる。

## 公理的意味論
数理論理学に基づいてプログラムの意味を説明する