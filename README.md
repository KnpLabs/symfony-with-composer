Symfony 2.0 Composer Edition
============================

Symfony2 Standard Edition, manageable through [Composer](http://getcomposer.org/)
and [Packagist](http://packagist.org/).

1) Download the Standard Edition
--------------------------------

Download archive from [here](https://github.com/KnpLabs/symfony-with-composer/zipball/master).

2) Installation
---------------

Once you've downloaded the composer edition, installation is easy, and basically
involves making sure your system is ready for Symfony.

### a) Check your System Configuration

Before you begin, make sure that your local system is properly configured
for Symfony. To do this, execute the following:

    php app/check.php

If you get any warnings or recommendations, fix these now before moving on.

### b) Install the Vendor Libraries

Now you need to download all of the necessary vendor libraries. Run the
following command:

    php bin/vendors install

### c) Access the Application via the Browser

Congratulations! You're now ready to use Symfony. If you've unzipped Symfony
in the web root of your computer, then you should be able to access the
web version of the Symfony requirements check via:

    http://localhost/Symfony/web/config.php

If everything looks good, click the "Bypass configuration and go to the Welcome page"
link to load up your first Symfony page.

You can also use a web-based configurator by clicking on the "Configure your
Symfony Application online" link of the ``config.php`` page.

To see a real-live Symfony page in action, access the following page:

    web/app_dev.php/demo/hello/Fabien

3) Learn about Symfony!
-----------------------

This distribution is meant to be the starting point for your application,
but it also contains some sample code that you can learn from and play with.

A great way to start learning Symfony is via the [Quick Tour](http://symfony.com/doc/current/quick_tour/the_big_picture.html),
which will take you through all the basic features of Symfony2 and the test
pages that are available in the standard edition.

Once you're feeling good, you can move onto reading the official
[Symfony2 book](http://symfony.com/doc/current/).

Using this Edition as the Base of your Application
--------------------------------------------------

Since the standard edition is fully-configured and comes with some examples,
you'll need to make a few changes before using it to build your application.

The distribution is configured with the following defaults:

* Twig is the only configured template engine;
* Doctrine ORM/DBAL is configured;
* Swiftmailer is configured;
* Annotations for everything are enabled.

A default bundle, ``AcmeDemoBundle``, shows you Symfony2 in action. After
playing with it, you can remove it by following these steps:

* delete the ``src/Acme`` directory;
* remove the routing entries referencing AcmeBundle in ``app/config/routing_dev.yml``;
* remove the AcmeBundle from the registered bundles in ``app/AppKernel.php``;


What's inside?
---------------
The Symfony Standard Edition comes pre-configured with the following bundles:
	
* **FrameworkBundle** - The core Symfony framework bundle
* **SensioFrameworkExtraBundle** - Adds several enhancements, including template
  and routing annotation capability ([documentation](http://symfony.com/doc/current/bundles/SensioFrameworkExtraBundle/index.html))
* **DoctrineBundle** - Adds support for the Doctrine ORM
  ([documentation](http://symfony.com/doc/current/book/doctrine.html))
* **TwigBundle** - Adds support for the Twig templating engine
  ([documentation](http://symfony.com/doc/current/book/templating.html))
* **SecurityBundle** - Adds security by integrating Symfony's security component
  ([documentation](http://symfony.com/doc/current/book/security.html))
* **SwiftmailerBundle** - Adds support for Swiftmailer, a library for sending emails
  ([documentation](http://symfony.com/doc/2.0/cookbook/email.html))
* **MonologBundle** - Adds support for Monolog, a logging library
  ([documentation](http://symfony.com/doc/2.0/cookbook/logging/monolog.html))
* **AsseticBundle** - Adds support for Assetic, an asset processing library
  ([documentation](http://symfony.com/doc/2.0/cookbook/assetic/asset_management.html))
* **JMSSecurityExtraBundle** - Allows security to be added via annotations
  ([documentation](http://symfony.com/doc/current/bundles/JMSSecurityExtraBundle/index.html))
* **WebProfilerBundle** (in dev/test env) - Adds profiling functionality and
  the web debug toolbar
* **SensioDistributionBundle** (in dev/test env) - Adds functionality for configuring
  and working with Symfony distributions
* **SensioGeneratorBundle** (in dev/test env) - Adds code generation capabilities
  ([documentation](http://symfony.com/doc/current/bundles/SensioGeneratorBundle/index.html))
* **AcmeDemoBundle** (in dev/test env) - A demo bundle with some example code

Enjoy!
