# EditorConfig

> _TIP: Use EditorConfig but download it only when needed_

Starting a code debugging or development session requires the use of the `.editorconfig` file but this risks increasing the number of files in the root of your project especially when you want to present your project on GitHub and avoid confusing users with a long list of dotfiles. Our advice is to download it when needed, creating a specific target in your `Makefile`.

## Usage

### Essential

Add the following line into `.gitignore` file

```
.editorconfig
```

Download `.editorconfig` file

```
curl -fsSL https://editorconfig.javanile.org/.editorconfig
```

### Makefile

Add the followig targets to your `Makefile`

```
## Start development or debugging session
dev: init

## Prepare repository files and directories
init: editorconfig

## Download `.editorconfig` file
editorconfig:
    curl -fsSL https://editorconfig.javanile.org/.editorconfig
```

## Good to know

### Contributing

Thank you for considering contributing to this project! The contribution guide can be found in the [CONTRIBUTING.md](CONTRIBUTING.md).

### Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](CONTRIBUTING.md).

### Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Francesco Bianco via [bianco@javanile.org](mailto:bianco@javanile.org). All security vulnerabilities will be promptly addressed.

### License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
