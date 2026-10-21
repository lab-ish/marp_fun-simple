# marpテンプレート

> marpスライドのテンプレートです

## Requirements

- nodejs (npx)
- marp (>=4.0)

## Usage

### PDFの生成

1. `sample.md`を参考に、スライドのmarkdownファイルを作成する。
2. marpでスライドを生成する。

```bash
$ npx @marp-team/marp-cli@latest --theme theme/fun.css --pdf sample.md --output sample.pdf
```

docker内で実行するときなど、サンドボックス機能を無効化しないと実行できない場合があります。
```bash
$ npx @marp-team/marp-cli@latest --theme theme/fun.css --no-sandbox --pdf sample.md --output sample.pdf
```

ローカルの画像などを含む場合は `--allow-local-files` オプションを付けてください。
```bash
$ npx @marp-team/marp-cli@latest --theme theme/fun.css --allow-local-files --pdf sample.md --output sample.pdf
```

### プレゼンテーション

ブラウザを使ってプレゼンテーションすることができます。
以下のコマンドでサーバを起動した後、ブラウザで `http://localhost:8080/` にアクセスし、プレゼンテーションしたい markdown ファイルを選択します。
```bash
npx @marp-team/marp-cli@latest --theme theme/fun.css --allow-local-files -s ./
```

コントロールを表示したくない場合は `--bespoke.osc=false` オプションを付けます。
```bash
npx @marp-team/marp-cli@latest --theme theme/fun.css --allow-local-files --bespoke.osc=false -s ./
```

## License

All the source files are released under the BSD 3-clause license.
See LICENSE.txt.

* Copyright (c) 2026, Shigemi ISHIDA
