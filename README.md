# Typst Syntax

This is seperated from [tinymist](https://github.com/Myriad-Dreamin/tinymist).

What I need is to work with [Shift-IM-for-VSCode](https://github.com/wangjiezhe/Shift-IM-for-VSCode) to automatically change IME condition in Typst file. It does work on Windows, but when I use WSL, it does not!

The reason is that Shift-IM must work on as an UI extension, whereas tinymist can only work as a workspace extension. Shift-IM use `vscode.extensions.all` to get all installed extensions, but it only gives extensions running on the same matchine.

So I separate the grammar part of tinymist, to make it work as an UI extension.
