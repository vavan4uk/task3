# Time tracking source, Symfony 4.4
https://github.com/vavan4uk/task3.git

Technical Requirements
Before installing application you must:

Install PHP 7.4.13 and these PHP extensions (which are installed and enabled by default in most PHP 7 installations): Ctype, iconv, JSON, PCRE, Session, SimpleXML, and Tokenizer;
Install Composer, which is used to install PHP packages.
Optionally, you can also install Symfony CLI. This creates a binary called symfony that provides all the tools you need to develop and run your Symfony application locally.

Before installation make sure what you have installed git/composer

Installation
cd ~/
git clone https://github.com/vavan4uk/task3.git task
cd task
symfony check:requirements
composer install
bin/console doctrine:database:create
bin/console doctrine:schema:update --force
symfony server:start




For run functionality test ( after complete instalation )
cd ~/
cd task
vendor/bin/codecept run --steps