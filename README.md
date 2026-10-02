<p align="center">
    <img src="https://raw.githubusercontent.com/burnlang/burn/master/assets/logo.svg" alt="Burn logo" width="128">
</p>

# Burn TextMate Bundle

This is a TextMate bundle for the [Burn](https://github.com/burnlang/burn) programming language.

## Features

- Syntax highlighting for `.bn` files: `def type`, `def struct` (also `abstract` and `static`), `def interface`, `def enum`, `new` and `destroy`, type-first
  declarations such as `String name`, string templates `"${expr}"`, nullable types, `async`/`await`, `is`/`as`
- Snippets for common language constructs
- Commands for running Burn files and starting the REPL

## Installation

### TextMate 2

1. Clone this repository or download it
2. Double-click the `Burn.tmbundle` folder to install it in TextMate

### Other editors

The grammar in `Syntaxes/Burn.tmLanguage` is a standard TextMate grammar and works in editors that accept
TextMate grammars (Sublime Text, Nova, and others). For VS Code use the
[Burn extension](https://github.com/burnlang/vscode-burn), which also connects to the Burn language server.

## Usage

### Snippets

| Trigger | Inserts |
| --- | --- |
| `def` | `def type` definition |
| `struct` | `def struct` with constructor parameters and a method |
| `new` | create a struct object with `new` |
| `interface` | `def interface` |
| `enum` | `def enum` |
| `fun` | function |
| `async` | async function |
| `main` | main function |
| `if` | if / else |
| `for` | `for i in 0..10` loop |
| `match` | `match` with a value arm and `else` |
| `while` | while loop |
| `import` | import statement |

### Commands

The commands need the Burn toolchain on your `PATH`:

```sh
curl -fsSL https://raw.githubusercontent.com/burnlang/burn/master/install.sh | sh
```


- `⌘R` - Run the current file
- `⌃⌘R` - Start the Burn REPL

## License

GNU General Public License v3.0 - see [LICENSE](LICENSE).
