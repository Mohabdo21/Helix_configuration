# Helix Editor Configuration

This repository contains configuration files for the Helix editor, including `config.toml` and `languages.toml`. These configurations enhance the functionality of Helix with features such as automatic formatting, syntax highlighting, and language server support.

## Table of Contents

- [Installation](#installation)
- [Configuration Setup](#configuration-setup)
- [Installing Language Servers and Formatters](#installing-language-servers-and-formatters)
- [Features](#features)
- [Contributing](#contributing)

## Installation

### Step 1: Install Helix Editor

First, you need to install the Helix editor. Follow these steps:

1. Download the latest release from the [Helix GitHub Releases](https://github.com/helix-editor/helix/releases).
2. Extract the downloaded archive:
   ```sh
   tar -xzf helix-vX.Y.Z-x86_64-linux.tar.gz
   ```
3. Move the extracted files to `/usr/local/bin`:
   ```sh
   sudo mv helix-vX.Y.Z-x86_64-linux/hx /usr/local/bin/
   ```

Ensure Helix is accessible from the command line:

```sh
hx --version
```

### Step 2: Clone the Configuration Repository

Clone this repository to your local machine:

```sh
git clone https://github.com/Mohabdo21/Helix_configuration.git
cd Helix_configuration
```

### Step 3: Copy Configuration Files

Copy the configuration files to the Helix configuration directory:

```sh
mkdir -p ~/.config/helix
cp config.toml languages.toml ~/.config/helix/
```

## Installing Language Servers and Formatters

The configuration files specify various Language Server Protocol (LSP) servers and formatters. Install these dependencies using the following commands:

### Python

```sh
# Language Servers
pip install 'python-lsp-server[all]'
npm install -g pyright

# Formatter
pip install autopep8

# Diagnostic Tool
pip install flake8
```

### TypeScript and JavaScript

```sh
# Language Server
npm install -g typescript typescript-language-server

# Formatter and Linter
npm install -g prettier eslint
```

### HTML, CSS, JSON, YAML

```sh
# Language Servers
npm install -g vscode-html-languageserver-bin vscode-css-languageserver-bin vscode-json-languageserver yaml-language-server

# Formatter
npm install -g prettier
```

### Bash

```sh
# Language Server
npm install -g bash-language-server

# Formatter
sudo apt install shfmt
```

### Docker

```sh
# Language Servers
npm install -g dockerfile-language-server-nodejs docker-compose-langserver
```

### Markdown

```sh
# Language Server
cargo install markdown-oxide
```

### Go

```sh
# Language Server
go install golang.org/x/tools/gopls@latest
```

### C

```sh
# Language Server
sudo apt install clangd

# Formatter
sudo apt install clang-format
```

## Features

- **Relative Line Numbers**: Displays line numbers relative to the current line for easy navigation.
- **Automatic Pairs**: Automatically inserts matching pairs for brackets, quotes, etc.
- **Auto Formatting**: Automatically formats code on save.
- **Indentation Guides**: Visual guides for indentation levels.
- **Cursor Shapes**: Custom cursor shapes for different modes (normal, insert, select).
- **Language Server Support**: Integrated LSP support for enhanced code completion, linting, and diagnostics.
- **Statusline Customization**: Customizable statusline with various indicators.

## Contributing

Contributions are welcome! Please fork this repository, make your changes, and open a pull request.
