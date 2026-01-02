# syntect::SyntaxSet defaults + Nushell generator

![Screenshot](./screenshot.png)

This project generates a
[`syntect::SyntaxSet`](https://docs.rs/syntect/latest/syntect/parsing/struct.SyntaxSet.html)
binary used by the
[Stacks clipboard manager](https://github.com/cablehead/stacks).

### Instructions to Generate the `SyntaxSet`

```bash
git clone https://github.com/cablehead/syntect-SyntaxSet-with-nushell.git
cd syntect-SyntaxSet-with-nushell
cargo r
```

Once the `syntax_set.bin` file has been generated, replace `stacks/src-tauri/syntax_set.bin`

### Using with bat

You can also use the Nushell syntax definition with [bat](https://github.com/sharkdp/bat):

```nushell
mkdir ~/.config/bat/syntaxes
cp nushell.sublime-syntax ~/.config/bat/syntaxes/
bat cache --build
```

Now `.nu` files will have syntax highlighting when viewed with bat.

## Credits

- The `nushell.sublime-syntax` file has been copied from
  [kurokirasama/nushell_sublime_syntax](https://github.com/kurokirasama/nushell_sublime_syntax).
  Thank you @kurokirasama!
