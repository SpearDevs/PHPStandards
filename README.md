# Speardevs PHP Standards

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
    }
}
```

### Install with Composer

```shell
composer require speardevs/php-standards --dev
```

### Allow to execute recipes

![img.png](images/recipes.png)
