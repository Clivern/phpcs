<p align="center">
    <img alt="phpcs logo" src="/assets/img/logo.png?v=1.0.0" height="200" />
    <h3 align="center">PHP Coding Standards</h3>
    <p align="center">
        <a href="https://packagist.org/packages/clivern/phpcs">
            <img src="https://img.shields.io/badge/Version-1.0.0-red.svg">
        </a>
        <a href="https://github.com/Clivern/phpcs/blob/master/LICENSE">
            <img src="https://img.shields.io/badge/LICENSE-MIT-orange.svg">
        </a>
    </p>
</p>


## Documentation

### Installation:

To install the package via `composer`, use the following:

```zsh
$ composer require clivern/phpcs
```

Place a file named `.php_cs.dist` that has following content in your project's root directory.

```php
<?php

use Clivern\CodingStandards\Rules;
use PhpCsFixer\Config;
use PhpCsFixer\Finder;

$finder = Finder::create()
    ->name('.php_cs.dist')
    ->in(__DIR__);

return Config::create()
    ->setFinder($finder)
    ->setRiskyAllowed(true)
    ->setRules(Rules::PHP72());
```


## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, phpcs is maintained under the [Semantic Versioning guidelines](https://semver.org/) and release process is predictable and business-friendly.

See the [Releases section of our GitHub project](https://github.com/clivern/phpcs/releases) for changelogs for each release version of phpcs. It contains summaries of the most noteworthy changes made in each release.


## Bug tracker

If you have any suggestions, bug reports, or annoyances please report them to our issue tracker at https://github.com/clivern/phpcs/issues


## Security Issues

If you discover a security vulnerability within phpcs, please send an email to [hello@clivern.com](mailto:hello@clivern.com)


## Contributing

We are an open source, community-driven project so please feel free to join us. see the [contributing guidelines](CONTRIBUTING.md) for more details.


## License

© 2021, clivern. Released under [MIT License](https://opensource.org/licenses/mit-license.php).

**phpcs** is authored and maintained by [@clivern](http://github.com/clivern).

