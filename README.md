# EEx Formatter

Fork of [EEx Formatter/Beautify](https://marketplace.visualstudio.com/items?itemName=zerokol.vscode-eex-beautify) with support of new elixir-ls html-eex.

This extension basically using [htmlbeautifier](https://github.com/threedaymonk/htmlbeautifier) to format your file using the Formatter API from the vscode, so no need to create a hack using Task, etc.

## Features

![Demo GIF](https://raw.githubusercontent.com/RoyalMist/vscode-eex-format/master/images/demo.gif)

## Requirements

```bash
gem install htmlbeautifier
```

NOTE: For you that have a filename with extension `.html.eex`, your file might be recognized as `html` file, not as `eex` file. In that case, add a setting in your `settings.json` like below:

```json
"files.associations": {
  "*.eex": "eex"
}
```

## Settings

| Setting                            | Description                                           | Default |
| ---------------------------------- | ----------------------------------------------------- | ------- |
| `vscode-eex-format.tabStops`       | Set number of spaces per indent                       | 2       |
| `vscode-eex-format.tab`            | Indent using tabs                                     | false   |
| `vscode-eex-format.indentBy`       | Indent the output by NUMBER steps                     | 0       |
| `vscode-eex-format.stopOnErrors`   | Stop when invalid nesting is encountered in the input | false   |
| `vscode-eex-format.keepBlankLines` | Set number of consecutive blank lines                 | 0       |

## References

[Base Idea](https://github.com/aliariff/vscode-erb-beautify)
