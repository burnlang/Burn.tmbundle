# Burn TextMate Bundle

This is a TextMate bundle for the [Burn](https://github.com/burnlang/burn) programming language (Burn 2).

## Features

- Syntax highlighting for `.bn` files: `def type`, `def class`, `def interface`, `def enum`, type-first
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
| `class` | `def class` with a field and a method |
| `interface` | `def interface` |
| `enum` | `def enum` |
| `fun` | function |
| `async` | async function |
| `main` | main function |
| `if` | if / else |
| `for` | `for i in 0..10` loop |
| `while` | while loop |
| `import` | import statement |

### Commands

- `⌘R` - Run the current file
- `⌃⌘R` - Start the Burn REPL

## License

MIT - see [LICENSE](LICENSE).
