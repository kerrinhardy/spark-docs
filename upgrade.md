# Upgrade Guide

- [Upgrading To Spark 8.0](#upgrade-spark-8.0)
- [Checking versions](#version-checks)

<a name="upgrade-spark-8.0"></a>
## Upgrading To Spark 8.0

Spark 8.0 is a simple maintenance release to provide compatibility with Laravel 5.8 and Cashier 9.0. As such, there are no Spark specific upgrade instructions. You should simply upgrade your application using the [Laravel 5.8 upgrade guide](https://laravel.com/docs/5.8/upgrade). In addition, ensure that your application's `composer.json` file is requiring Laravel Cashier `^9.0`.

### Upgrading Via Spark CLI

If you installed Spark via the `spark` CLI tool, you may run the `spark:update` Artisan command:

    php artisan spark:update --major

### Upgrading Via Composer

If you installed Spark via Composer, you may simply upgrade your dependency name and version in your `composer.json` file and run the `composer update` command. Of course, in order for your GitHub user to access the repository, you should first join this repository in the Spark dashboard:

    "laravel/spark-aurelius": "~8.0"

<a name="version-checks"></a>
## Checking versions

The following version check commands are available:

- Spark Installer `spark -v`
- Laravel Spark `php artisan spark:version`
- Laravel Installer `laravel -v`
- Laravel Framework `php artisan -V`