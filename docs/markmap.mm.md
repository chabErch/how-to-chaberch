---
markmap:
  colorFreezeLevel: 2
  maxWidth: 300
  htmlParser:
    selector: h1,h2,h3,ul,ol,li,table,pre
  embedAssets: true
  color: '#2980b9'
---

# Markmap test

## Привет как дела как погода азаза мне нравятся ноги твои глаза

- [Website](https://markmap.js.org/)
    - Yo 1
        - Yo 1.1
    - Yo 2
    - Yo 3
- [GitHub](https://github.com/gera2ld/markmap)

## Related Projects

- [coc-markmap](https://github.com/gera2ld/coc-markmap) for Neovim
- [markmap-vscode](https://marketplace.visualstudio.com/items?itemName=gera2ld.markmap-vscode) for VSCode
- [eaf-markmap](https://github.com/emacs-eaf/eaf-markmap) for Emacs

## Features

Note that if blocks and lists appear at the same level, the lists will be ignored.

### Lists

- **strong** ~~del~~ _italic_ ==highlight==
- `inline code`
- [x] checkbox
- Katex: $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ <!-- markmap: fold -->
  - [More Katex Examples](#?d=gist:af76a4c245b302206b16aec503dbe07b:katex.md)
- Now we can wrap very very very very long text based on `maxWidth` option

### Blocks

```js
console('hello, JavaScript')
const a = 8;
```

| Products | Price |
| -------- | ----- |
| Apple    | 4     |
| Banana   | 2     |
