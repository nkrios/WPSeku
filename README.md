## WPSeku - Wordpress Security Scanner
WPSeku is a black box WordPress vulnerability scanner that can be used to scan remote WordPress installations to find security issues.

![python](https://img.shields.io/badge/python-3.x-green.svg) ![license](https://img.shields.io/badge/License-GPLv3-brightgreen.svg)

![screen_1](https://raw.githubusercontent.com/m4ll0k/WPSeku/master/screen/main.png)

## Installation
```
$ git clone https://github.com/m4ll0k/WPSeku.git wpseku
$ cd wpseku
$ pip3 install -r requirements.txt
$ python3 wpseku.py
```
## Usage
### Generic Scan

`python3 wpseku.py --url http://www.site.com --verbose`

* __Output__

```
----------------------------------------
 _ _ _ ___ ___ ___| |_ _ _ 
| | | | . |_ -| -_| '_| | |
|_____|  _|___|___|_,_|___|
      |_|             v0.4.0

WPSeku - Wordpress Security Scanner
by Momo Outaadi (m4ll0k)
----------------------------------------

[ + ] Target: https://www.xxxxxxx.com
[ + ] Starting: 02:38:51

[ + ] Server: Apache
[ + ] Uncommon header "X-Pingback" found, with contents: https://www.xxxxxxx.com/xmlrpc.php
[ i ] Checking Full Path Disclosure...
[ + ] Full Path Disclosure: /home/ehc/public_html/wp-includes/rss-functions.php
[ i ] Checking wp-config backup file...
[ + ] wp-config.php available at: https://www.xxxxxxx.com/wp-config.php
[ i ] Checking common files...
[ + ] robots.txt file was found at: https://www.xxxxxxx.com/robots.txt
[ + ] xmlrpc.php file was found at: https://www.xxxxxxx.com/xmlrpc.php
[ + ] readme.html file was found at: https://www.xxxxxxx.com/readme.html
[ i ] Checking directory listing...
[ + ] Dir "/wp-admin/css" listing enable at: https://www.xxxxxxx.com/wp-admin/css/
[ + ] Dir "/wp-admin/images" listing enable at: https://www.xxxxxxx.com/wp-admin/images/
[ + ] Dir "/wp-admin/includes" listing enable at: https://www.xxxxxxx.com/wp-admin/includes/
[ + ] Dir "/wp-admin/js" listing enable at: https://www.xxxxxxx.com/wp-admin/js/
```

## Credits and Contributors
Original idea and script from WPScan Team (https://wpscan.org/)

WPScan Vulnerability Database (https://wpvulndb.com/api)
