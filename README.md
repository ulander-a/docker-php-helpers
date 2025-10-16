# 🐋 Docker/PHP helpers 🐘

This is a set of bash scripts made to simplify the management and usage of PHP code quality tools across different PHP versions and containers.

**Includes functionality for: [PHP](https://www.php.net/), [PHP Code sniffer](https://github.com/squizlabs/PHP_CodeSniffer), [PHP Code Beautifier and Fixer](https://phpqa.io/projects/phpcbf.html)** - all these are included in the default Totara docker container.

**Supported PHP versions: 7.4, 8.2, 8.3, 8.4.** (this is arbitrary and can be easily changed)

## Installation (should work on UNIX systems, mileage may vary on Windows)

1. Copy scripts from `docker-php-helpers/scripts` to somewhere in PATH, i suggest `/usr/local/bin`.
2. Make the scripts into executables with `chmod +x docker-php.sh docker-phpcs.sh docker-phpcbf.sh`
3. Run something like `docker-php --version` to check that everything works as intended.
