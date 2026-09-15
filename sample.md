---
marp: true
theme: fun
footer: '<span class="footer-left">March 21, 2026</span><span class="footer-right">Inamura-Ishida Lab, Future University Hakodate</span>'
paginate: true
math: katex
---

<!-- _class: title -->
# タイトル<br>Title
## Subtitle

<div class="author"><u>Shigemi ISHIDA</u><sup>*1</sup>, Yutaka ARAKAWA<sup>*2</sup></div>
<div class="affiliation"><sup>*1</sup>Future University Hakodate, <sup>*2</sup>Kyushu University</div>

---
# デフォルトレイアウト

- 箇条書きをするレイアウト
  - Level2
  - Level2
    - Level3
    - Level3
- Level1
  - [リンクテキスト](https://www.example.jp/)
  -  一部を**強調**する

---
<!-- _class: ref-content -->
# 文献付きデフォルトレイアウト

- コンテンツ本文<span class="ref-label">[wang'14]</span>
  - サブ項目1
  - Reference 2<span class="ref-label">[dezhi'20]</span>
- 数式も書ける $E = mc^2$
  $$\int_0^\infty x\log x\,dx$$

<div class="ref">

[wang'14] E-eyes: In-home device-free activity identification using fine-grained WiFi signatures, ACM MobiCom.
[dezhi'20] Packet position modulation: A technique for enhancing information transfer capacity in ultra-low duty cycle networks, ACM ICDCN.

</div>

---
<!-- _class: two-content -->
# 2カラムレイアウト

<div class="columns">
<div>

- divで並べる
  - divの前後に空行を入れないといけない
- 左の項目3
  - 左
    - 左

</div>

<div>

- 右の項目A
  - 右の項目B
    - テスト
- コードブロック
```python
def main():
  print("Hello!")
```

</div>
</div>

---
<!-- _class: section -->
# セクションタイトル<br>2行目Title
## サブタイトル<br>2行目Subtitle

---
<!-- _class: emph-section -->
# 強調セクションタイトル<br>2行目Title
## サブタイトル<br>2行目Subtitle

---
<!-- _class: section -->

# 以降はTips

---
<style scoped>section {font-size: 37px;}</style>

# 入りきらないとき

- 少しだけフォントサイズを小さくするのが良い
- ページ先頭にそのページのみに有効な形で `style` を定義する

---
# 中央揃え

- `centering` クラスの `div` を配置すると中央揃えとなるようにしてある
  - 表なども入れられる

<div class="centering">

| 項目1 | 項目2 | 項目3 |
|--|--|--|
| A | 0 | 1 | 2 |
| B | 3 | 4 | 5 |

</div>

---
# 強調したボックス

- `emph-box` クラスの `div` を配置すると強調のためのボックスを配置する

<div class="centering">
<div class="emph-box">ここは強調されたボックス内！！</div>
</div>

---
# 画像の配置

- こんな形で埋め込める
  - ベクトルはSVGが良い(PDF画像は貼れない)
- `--allow-local-files` オプションを付けて実行しないと手元のファイルにはアクセスできない

<div class="centering">

![width:200px center](./img/test.svg)

</div>

---
# 番号付きリスト

1. markdownの番号付きリストも普通に使える
1. 2番目
   1. 2-1
   1. 2-2
1. 3番目
   - 番号なし1
   - 番号なし2

---
<!-- _class: ref-content -->
# 図＋出典キャプション

- `fig` クラスの `div` に画像と `src` クラスの `div` (出典) を入れる
  - 引用図は `src` に「出典: [ラベル] Fig. X より引用」と書く

<div class="fig">

![height:250px](./img/test.svg)

<div class="src">出典: [wang'14] Fig. 1 より引用</div>
</div>

<div class="ref">

[wang'14] E-eyes: In-home device-free activity identification using fine-grained WiFi signatures, ACM MobiCom.

</div>
