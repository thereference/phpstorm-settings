# PhpStorm settings for The Reference Employees

## Project setup

1. In PHPStorm, navigate to *File > Settings Repository...*
2. Set the upstream URL to *git@github.com:thereference/phpstorm-settings.git*
3. Press overwrite local.

> **NOTE**: Assumes a standard setup: Mac OSX with homebrew installed.

## Plugins enabled

The following PhpStorm plugins are installed:
* [.ignore](https://github.com/hsz/idea-gitignore) - support for the .gitignore files
* [BashSupport](https://github.com/jansorg/BashSupport) - support for .sh bash scripts
* [Drupal Symfony Bridge](https://github.com/Haehnchen/idea-php-drupal-symfony2-bridge) - Symfony + Drupal :heart:
* [PHP Annotations](https://github.com/Haehnchen/idea-php-annotation-plugin)
* [PHP composer.json support](https://github.com/psliwa/idea-composer-plugin) - enhanced composer support
* [SvgViewer 2](https://github.com/billdwhite/intellij-plugins-svgviewer2) - SVG!
* [Symfony Plugin](https://github.com/Haehnchen/idea-php-symfony2-plugin)

## PHP_CodeSniffer and the Drupal coding standards

1. Install Drupal coder: `composer global require drupal/coder`
2. Register the Drupal and DrupalPractice coding standards with PHPCS: `phpcs --config-set installed_paths ~/.composer/vendor/drupal/coder/coder_sniffer`
3. Test that it works: `phpcs -i`. It should include DrupalPractice and Drupal coding standards.

It is recommended to simply let PHP_CodeSniffer fix the errors that can be automated. Simply change to the root of the
custom code and run `drupalcbf .`.

## References

- [Drupal Development using PhpStorm](https://confluence.jetbrains.com/display/PhpStorm/Drupal+Development+using+PhpStorm)
- [Using Drupal with PhpStorm](https://www.jetbrains.com/help/phpstorm/using-drupal-with-phpstorm.html)
- [Installing Coder Sniffer](https://www.drupal.org/node/1419988)
