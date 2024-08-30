# Run PHP

[![Latest Version on Packagist](https://img.shields.io/packagist/v/futureplc/run-php.svg?style=flat-square)](https://packagist.org/packages/futureplc/run-php)
[![Total Downloads](https://img.shields.io/packagist/dt/futureplc/run-php.svg?style=flat-square)](https://packagist.org/packages/futureplc/run-php)

Run PHP is a single command to assist in executing PHP code in a file.

The intention is to make it easier to execute "scratch files" when writing quick-and-dirty code, simply to save a little bit of time. It has 2 primary features that make it more useful than running a plain PHP interpreter:

1. **Automatic Autoloaders** - When running a PHP file, it will automatically detect and use Composer's autoloader if it exists in the current directory or a parent directory
2. **Class Aliasing** - If a class is used in the file that doesn't exist, it will attempt to alias it to a class in the autoloader

## Installation

You can install the package via Composer:

```bash
composer global require futureplc/run-php
```

## Usage

To run a PHP file with the script, just call the command and pass through a file path as a single argument:
```bash
run-php /path/to/file/to/run.php
```

## License

The MIT License (MIT).
