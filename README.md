# FFprobe
FFprobe php wrapper

## Install
composer require appzz/ffprobe

## Usage
### Init
```php
use AppZz\VideoTools\FFprobe;
require vendor/autoload.php;

/**
If needed specify path to local binary files
**/
FFprobe::$binary = '/usr/local/bin/ffprobe';
```
### Get metadata
```php
$info = FFprobe::factory('video.mp4')->probe();
var_dump($info);
```
