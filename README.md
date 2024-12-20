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

## Credits

- The `nushell.sublime-syntax` file has been copied from
  [kurokirasama/nushell_sublime_syntax](https://github.com/kurokirasama/nushell_sublime_syntax).
  Thank you @kurokirasama!
