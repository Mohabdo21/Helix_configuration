# Helix Text Editor Configuration

This repository contains configuration files for the Helix text editor. These configurations are designed to enhance your coding experience with features like relative line numbers, color modes, auto-pairs, auto-formatting, and more.

## Installation

Before you start, ensure you have [Helix](https://helix-editor.com/) installed on your machine. If not, you can install it using the instructions provided on their official website.

## Configuration Files

This repository contains two main configuration files:

1. `config.toml`: This file contains general settings for the Helix editor. It includes settings for the editor's appearance, behavior, and language server protocol (LSP) configurations.

2. `languages.toml`: This file contains language-specific settings and configurations for various language servers. It includes settings for Python, TypeScript, JavaScript, HTML, CSS, and more.

## Dependencies

The configuration files in this repository require several language servers to be installed on your machine. These include:

- `pyright-langserver` for Python
- `typescript-language-server` for TypeScript and JavaScript
- `vscode-html-languageserver` for HTML
- `deno` for TypeScript X (TSX)
- `emmet-ls` for Emmet abbreviations
- `vscode-eslint-language-server` for ESLint
- `vscode-css-language-server` for CSS
- `vscode-json-language-server` for JSON

Please ensure these language servers are installed and properly configured on your machine.

## Usage

To use these configurations, clone this repository and copy the `config.toml` and `languages.toml` files to your Helix configuration directory (usually `~/.config/helix`). Then, restart Helix to apply the new configurations.

```bash
git clone <this-repo-url>
cp config.toml ~/.config/helix/
cp languages.toml ~/.config/helix/
```
