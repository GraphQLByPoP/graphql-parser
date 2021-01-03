# GraphQL Parser

[![Build Status][ico-travis]][link-travis]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Software License][ico-license]](LICENSE.md)

<!--
[![Latest Version on Packagist][ico-version]][link-packagist]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Total Downloads][ico-downloads]][link-downloads]
-->

Parser for the GraphQL syntax

This component is a fork of [Youshido GraphQL](https://github.com/youshido-php/GraphQL), extracting the parser functionality from within.

## Install

Via Composer

``` bash
composer require graphql-by-pop/graphql-parser
```

## Development

The source code is hosted on the [PoP monorepo](https://github.com/leoloso/PoP), under [`GraphQLByPoP/packages/graphql-parser`](https://github.com/leoloso/PoP/tree/master/layers/GraphQLByPoP/packages/graphql-parser).

## Usage

Initialize the component:

``` php
\PoP\Root\ComponentLoader::initializeComponents([
    \GraphQLByPoP\GraphQLParser\Component::class,
]);
```

## PHP versions

Requirements:

- PHP 7.4+ for development
- PHP 7.1+ for production

### Supported PHP features

Same as the [Supported PHP features for `getpop/root`](https://github.com/getpop/root/#supported-php-features)

### Downgrading code to PHP 7.1

Via [Rector](https://github.com/rectorphp/rector) (dry-run mode):

```bash
composer preview-code-downgrade
```

## Standards

[PSR-1](https://www.php-fig.org/psr/psr-1), [PSR-4](https://www.php-fig.org/psr/psr-4) and [PSR-12](https://www.php-fig.org/psr/psr-12).

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Testing

``` bash
composer test
```

## Static Analysis

Execute [phpstan](https://github.com/phpstan/phpstan) with level 8:

``` bash
composer analyse
```

To run checks for level 0 (or any level from 0 to 8):

``` bash
./vendor/bin/phpstan analyse -l 0 src tests
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) for details.

## Security

If you discover any security related issues, please email leo@getpop.org instead of using the issue tracker.

## Credits

- [Leonardo Losoviz][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/graphql-by-pop/graphql-parser.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/graphql-by-pop/graphql-parser/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/graphql-by-pop/graphql-parser.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/graphql-by-pop/graphql-parser.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/graphql-by-pop/graphql-parser.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/graphql-by-pop/graphql-parser
[link-travis]: https://travis-ci.org/graphql-by-pop/graphql-parser
[link-scrutinizer]: https://scrutinizer-ci.com/g/graphql-by-pop/graphql-parser/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/graphql-by-pop/graphql-parser
[link-downloads]: https://packagist.org/packages/graphql-by-pop/graphql-parser
[link-author]: https://github.com/leoloso
[link-contributors]: ../../../../../../contributors
