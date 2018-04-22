# A standard PHP project skeleton

Are you tired of copy-pasting your boilerplate PHP code whenever you need to start a new project?

This repository contains a single-line command that will automatically setup for you all the needed code to create a modern, clutter-free and test-oriented PHP package.

It will automatically install the following dependencies:

* PHPUnit 6.x: run your unit tests.
* PHP_CodeSniffer: validate your code against code convention.
* PHP_CsFixer: automatically fix your code to match the code convention.
* PHPMD: analyze your code to detect sub-optimal or overly complex code.

As well as config file for popular continuous integration tool.
 
## Create Project
   
To create your project, enter the following command in your console.    
```
composer create-project koriym/php-skeleton {project-path}
```

## Composer Commands

Once installed, the project will automatically be configured so you can run those commands in the root of your application:

### test

`composer test` run [`phpunit`](https://github.com/sebastianbergmann/phpunit).

### tests

`composer tests` run [`phpcs`](https://github.com/squizlabs/PHP_CodeSniffer), [`php-cs-fixer`](https://github.com/FriendsOfPHP/PHP-CS-Fixer), [`phpmd`](https://github.com/phpmd/phpmd), [`phpstan`](https://github.com/phpstan/phpstan) and [`phpunit`](https://github.com/sebastianbergmann/phpunit). 

### coverage

`composer coverage` builds test coverage report.

### cs-fix

`composer cs-fix` run [`php-cs-fixer`](https://github.com/FriendsOfPHP/PHP-CS-Fixer) and [`phpcbf`](https://github.com/squizlabs/PHP_CodeSniffer/wiki/Fixing-Errors-Automatically) to fix up the PHP code to follow the coding standards. (Check only command `compposer cs` is also available.)


### build

`composer build` run [`phploc`](https://github.com/sebastianbergmann/phploc), [`pdepend`](https://pdepend.org/) and [tests](#tests) above. It's handy for Jenkins. 
You need "composer require phploc/phploc pdepend/pdepend --dev" for this.

## Setup continuous integration

Maybe some instructions with screenshot on how to setup GitHub CI and Scrutinizr?
