# Speardevs PHP Standards

## Features

Speardevs PHP Standards package contains:

* PHPStan
* Easy Coding Standard
* Rector
* PHPUnit
* GitHub Action workflow

## Installation

### Configure `composer.json`

```json
{
    "extra": {
        "symfony": {
            "endpoint": [
                "https://api.github.com/repos/speardevs/recipes/contents/index.json",
                "flex://defaults"
            ]
        }
    },
    "repositories": [
        {
            "type": "vcs",
            "url": "git@github.com:SpearDevs/php-standards.git"
        }
    ]
}
```

### Install with Composer

```shell
composer require speardevs/php-standards --dev
```

### Allow to execute recipes

![img.png](images/recipes.png)

### Generate project composer token

Generate token [here](https://github.com/settings/tokens/new?scopes=repo&description=GitHub%20Actions%20Composer) and
create new GitHub Action's secret key `SPEARDEVS_PIPELINES_KEY` with generated token.

## Notes

1. If amount of changes to apply for PHPStan is overwhelming, you
   can [generate baseline](https://phpstan.org/user-guide/baseline) and then slowly improve code file by file.
