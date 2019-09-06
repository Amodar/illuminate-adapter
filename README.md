# Illuminate PSR-6 Cache pool (laravel 6 support)

This is a PSR-6 cache implementation using Illuminate cache. It is a part of the PHP Cache organisation. To read about 
features like tagging and hierarchy support please read the shared documentation at [www.php-cache.com](http://www.php-cache.com). 

This is a PSR-6 to Illuminate bridge.

### Install

```bash
composer require cache/illuminate-adapter
```

## Use

```php
use Illuminate\Cache\ArrayStore;
use Cache\Adapter\Illuminate\IlluminateCachePool;

// Create an instance of an Illuminate's Store
$store = new ArrayStore();

// Wrap the Illuminate's store with the PSR-6 adapter
$pool = new IlluminateCachePool($store);
```


### Contribute

Contributions are very welcome! Send a pull request to the [main repository](https://github.com/php-cache/cache) or 
report any issues you find on the [issue tracker](http://issues.php-cache.com).
