# weswaldix\phpaustrianholidays
PHP library to test if given date is an austrian holiday.

Contains all austrian holidays between (inclusive) **2011-01-01** and **2025-12-31**.

usage:
```php
require 'vendor/autoload.php';
use weswaldix\austrianholidays\AustrianHoliday;

$is_holiday = AustrianHoliday::isHoliday("2017-01-01 00:00:00");
// true, because it´s New Year´s Day

$is_holiday = AustrianHoliday::isHoliday("2017-02-01 00:00:00");
// false, because no austrian holiday

$is_holiday = AustrianHoliday::isHoliday("02.04.2018");
// true
