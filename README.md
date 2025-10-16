# 🐋 Docker/PHP helpers 🐘

This is a set of bash scripts made to simplify the management and usage of PHP code quality tools across different PHP versions and containers.

**Includes functionality for: [PHP](https://www.php.net/), [PHP Code sniffer](https://github.com/squizlabs/PHP_CodeSniffer), [PHP Code Beautifier and Fixer](https://phpqa.io/projects/phpcbf.html)** - all these are included in the default Totara docker container.

## Installation (should work on UNIX systems, mileage may vary on Windows)

1. Copy scripts from `docker-php-helpers/scripts` to somewhere in PATH, i suggest `/usr/local/bin`.
2. Make the scripts into executables with `chmod +x docker-php docker-phpcs docker-phpcbf`.
3. Run something like `docker-php --version` to check that everything works as intended.

## Usage

Run the scripts (i.e. `docker-php`) from inside a repository and it will attempt to automatically detect the PHP version from the *.gitlab-ci.yml* (subject to change) and find the matching docker container.

**Examples:**

1. Run "reset password" CLI script `docker-php server/admin/cli/reset_password.php`
2. Run PHP Code Sniffer on a file/dir: `docker-phpcs server/local/path/to/dir/`
3. Run PHP Code Beautifier and Fixer on a file/dir: `docker-phpcbf server/local/path/to/file.php`
