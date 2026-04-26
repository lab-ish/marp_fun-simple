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
