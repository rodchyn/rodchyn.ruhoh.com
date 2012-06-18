### What & Why

In PHP we've had a lousy culture of code-sharing. Because depending on code from others as been tricky, every major PHP application or framework has practically had to reimplement the whole world. Only some tools, like PHPUnit, have managed to break over this barrier and become de-facto standards across project boundaries. But for the rest: just write it yourself.

### What is it?

The [Composer](http://getcomposer.org/) ecosystem is made of two main parts, both are available on [GitHub](http://github.com/composer/composer). The development effort is being led by Nils Adermann and Jordi Boggiano, but we already have more than 20 contributors which I would like to thank a bunch for helping.

### npm inspired

The composer is inspired by npm from node.js and Bundler from ruby language. And you know that this tools works. And works great. Instead of searching whole world yo can find needed package in composer "packagist" repository add it in your requirements and thats all. Other job will do composer.

### Example 
For example you need logger in your application. Go ahead. Add composer.json definition in your project like 


    {
        "require": {
            "monolog/monolog": "1.0.0"
        }
    }

and use it 

    <?php
    
    $autoloader = require_once "vendor/autoload.php"

### PSR-0

Composer follow [PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md) autoload standard from PHP Framework Interpolability Group

### Super easy instalation
While ease-of-installation is important, it isn't enough to build an ecosystem. The other thing that has to be easy is publishing code. Basically: if you've written a piece of functionality in PHP that you could see yourself using in another project, it should be effortless to publish it as a library.

    $ curl -s http://getcomposer.org/installer | php

Where are we now?
It is still early days for Composer, and the project is being worked on at a hectic pace. However, it is already good enough for managing dependencies to modern, PSR-0 compatible libraries.


---
title: Composer solves the PHP code-sharing problem
date: '2012-06-18'
description: PHP ecosystem
categories: php
tags: [php, composer]
---
