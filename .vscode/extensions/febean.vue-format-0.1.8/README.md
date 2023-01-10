# vue-format README

- English: [./README_EN.md](https://github.com/win7killer/vue-format/blob/master/./README_EN.md)
- 中文: [./README.md](https://github.com/win7killer/vue-format/blob/master/./README.md)

Format single file with '.vue' used in 'vscode' editor.（vscode 编辑器格式化插件，格式化单文件“.vue”文件代码）
https://marketplace.visualstudio.com/items?itemName=febean.vue-format
> 如果你有问题或者需求，欢迎来提 issue。  https://github.com/win7killer/vue-format

> 你的 issue 就是我的原力.  `欢迎 STAR && FORK`

> 对 js-beautify 依赖很重，所以大部分都受 js-beautify 限制。理论上 js-beautify 的配置都可以适用。

## Features
<img src="https://raw.githubusercontent.com/win7killer/vue-format/master/images/command.gif" alt="command" width=600/>

## Requirements
- js-beautify: [https://github.com/beautify-web/js-beautify](https://github.com/beautify-web/js-beautify)
- pug-beautify: [https://github.com/vingorius/pug-beautify](https://github.com/vingorius/pug-beautify)

## Keyboard Shortcuts
- mac: `cmd+ctrl+p`
- win: `alt+ctrl+p`

## Extension Settings

- 使用[js-beautify](https://github.com/beautify-web/js-beautify)配置 和 [pug-beautify](https://github.com/vingorius/pug-beautify)配置
- indent_size 默认使用 editor.tabSize

```jsonc
{
    "html_indent_root": false, // 是否缩进vue template中的根节点
    "break_attr_limit": -1, // tag 的 attrs 大于该数值时，强制 attrs 换行，-1时不换行
    "attr_end_with_gt": true, // break_attr_limit省生效时，tag的">"是否不换行，默认true
    "format_need": ["html", "js", "css"], // vue单文件中需要格式化的语言，默认["html", "js", "css"]。从数组中删除你不希望格式化的语言
    "js-beautify": {
        "indent_size": "editor.tabSize",
        "indent_char": " ",
        "indent_with_tabs": false,
        "brace-style": "collapse",
        "space_after_anon_function": true,
        "css": {},
        "js": {},
        "html": {
            // "force_format": ["template"],
            "wrap_attributes": "auto"
        }
    },
    "pug-beautify": {
        "fill_tab": false
    }
}

```

|Key|Example|Default|
|---|---|---|
|vue-format.html_indent_root|false|false|
|vue-format.break_attr_limit|2|-1|
|vue-format.attr_end_with_gt|true|true|
|vue-format.format_need|["html"]|["html", "js", "css"]
|vue-format.js-beautify|(See the config at front)|(See the config at front)
|vue-format.pug-beautify|{fill_tab: false}|{fill_tab: false}


## Changelog
U can see the changelog in [CHANGELOG.md](https://github.com/win7killer/vue-format/blob/master/./CHANGELOG.md)

## Todo List
Some things todo in [todo.md](https://github.com/win7killer/vue-format/blob/master/./todo.md)
