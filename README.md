# ASLCart

> ASLCart pretends to be a basic and simple implementation of a shopping cart available for Laravel and Lumen 5.

# Setting up the environment

##Install via Composer

From the command line, run:

$ composer require agsotelo/aslcart

##Laravel 5

###Step 1: Publishing config

From the command line, run:

$ php artisan vendor:publish --provider=ASLCartLaravelServiceProvider

###Step 2: Service Provider

For your Laravel app, open config/app.php and, within the providers array, append:

agsotelo\ASLCart\Providers\ASLCartLaravelServiceProvider::class,

This will bootstrap the package into Laravel.

###Step 3: Facade

For your Laravel app, open config/app.php and, within the aliases array, append:

'ASLCart' => agsotelo\ASLCart\Facades\ASLCart::class

This will add the ASLCart Facade into Laravel.

###Step 4: Configuration (TODO)

Add the following entries to your environment (.env) file:

ASLCART_¿? // TODO

##Lumen 5

###Step 1: Service provider

Inside your bootstrap/app.php file, add:

$app->register(agsotelo\ASLCart\Providers\ASLCartLumenServiceProvider::class);

###Step 2: Configuration

Copy the vendor/agsotelo/aslcart/src/config/aslcart.php file to your local config directory (if not exists must create) and don't forget add the entries to your environment (.env) file described in Step 4 of the Laravel Configuration.

## Usage

// TODO

## Bugs

If you find a bug or an unusual behavior don't hesitate to send me an email to <agsotelo@gmail.com> and I will respond as soon as possible BUT if you are a proactive person feel free to fork these project and then create a pull request =).

## License

The MIT License (MIT)

Copyright (c) 2017 Augusto Gerardo Sotelo Labarca

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
