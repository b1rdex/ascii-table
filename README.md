# sphinx-configurator

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/LTD-Beget/ascii-table/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/LTD-Beget/ascii-table/?branch=master)
[![License MIT](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/voksiv/sphinx-configurator/blob/master/LICENSE)

Php library with ascii table enum.

## Installation

```shell
composer require ltd-beget/ascii-table
```

## Usage
```php

<?php
    require(__DIR__ . '/vendor/autoload.php');
    
    use LTDBeget\ascii\AsciiControlChar;
    use LTDBeget\ascii\AsciiPrintableChar;
    
    $backspace = AsciiControlChar::BACKSPACE();
    $backspace->getDec();
    $backspace->getChar();
    $backspace->getHex();
    $backspace->isControlChar();
    $backspace->isPrintableChar();
    
    $colon = AsciiPrintableChar::COLON();
    $colon->getDec();
    $colon->getChar();
    $colon->getHex();
    $colon->isControlChar();
    $colon->isPrintableChar();
```
## Developers
### Regenerate documentation
```shell
$ ./vendor/bin/phpdox
```

## License
released under the MIT License.
See the [bundled LICENSE file](LICENSE) for details.
