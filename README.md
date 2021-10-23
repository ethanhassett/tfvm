# tfvm

[![Version](https://img.shields.io/github/v/release/ethanhassett/tfvm?style=flat-square)](https://github.com/ethanhassett/tfvm/releases)
[![MIT License](https://img.shields.io/github/license/ethanhassett/tfvm?style=flat-square)](https://github.com/ethanhassett/tfvm/blob/main/LICENSE)

> A Terraform Version Manager written in Go

## Table of Contents

- [tfvm](#tfvm)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Changelog](#changelog)
  - [How it Works](#how-it-works)
  - [Getting Started](#getting-started)
    - [Installation](#installation)
    - [CLI Usage](#cli-usage)
  - [Contributing](#contributing)
    - [Development](#development)

## Features

- Easily manage multiple terraform versions to use across projects.
- Run `tfvm use` with no version argument to switch to the version specified in the current directory's `.tfversion` file.

## Changelog

See the [CHANGELOG](https://github.com/ethanhassett/tfvm/blob/main/CHANGELOG.md)

## How it Works

tfvm installs and manages different versions of terraform in the CLI.

## Getting Started
### Installation

Windows users can install via [Scoop](https://scoop.sh):
```PowerShell
scoop bucket add tfvm https://github.com/ethanhassett/tfvm
scoop install tfvm
```

Linux users can install via the [install script](install.sh):
```bash
wget -q -O - https://raw.githubusercontent.com/ethanhassett/tfvm/main/install.sh | bash
```
Running the install script after installation will keep tfvm updated.

Using `go get`:
```bash
go get -u github.com/ethanhassett/tfvm@1.0.1
```
This will require manually adding `<USER_HOME>/.tfvm` to PATH.

Run `tfvm --version` to verify installation.

### CLI Usage

```
$ tfvm --help

Usage: tfvm [--version] [--help] <command> [<args>]

Available commands are:
    install    Install a version of Terraform
    list       List all installed versions of Terraform
    remove     Remove a specific version of Terraform
    use        Select a version of Terraform to use
```

## Contributing

Contributions to this project are welcome and much appreciated!

### Development

1. Use Golang version `>= 1.16`
2. Fork [this repo](https://github.com/ethanhassett/tfvm)
3. Create a `feat-` branch
4. Commit and push your changes
5. Open a Pull Request, rebasing against `main` if needed.

Bugs, feaure requests, and comments are more than welcome in the [issues](https://github.com/ethanhassett/tfvm/issues).
