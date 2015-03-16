# [ajax-cdn-speed-test](https://github.com/rsp/ajax-cdn-speed-test)

This program tests the speed of various free CDNs (content delivery networks)
that can be used for including JavaScript libraries in your websites
("hot linking" if anyone is still using this term).

It is a simple shell script that I wrote to quickly compare the speed of two CDNs.
After I wrote it I learned about the [CDNperf](https://www.cdnperf.com/) website
which may be more useful than this script in general.

What this script does, however, is tell you what are the numbers for
**your particular location** in this given instant, which may be interesting to someone.
Using this script I have seen very different results than what is shown on CDNperf.
For example Microsoft CDN that according to CDNperf is the fastest, is usually the slowest
one for me (tested from Warsaw, Poland) which is an important information when choosing
the right CDN for local demographics.

Installation
============
```
wget https://raw.githubusercontent.com/rsp/ajax-cdn-speed-test/master/ajax-cdn-speed-test
chmod a+x ajax-cdn-speed-test
```

Usage
=====
```
ajax-cdn-speed-test
```

How it works
============
It downloads a minified version of jQuery 2.1.3 over HTTP and HTTPS and displays download time.
It also prints the average ping round-trip time for the host. It tests the following CDNs:

* [Google Hosted Libraries](https://developers.google.com/speed/libraries/)
* [Microsoft Ajax Content Delivery Network](https://www.asp.net/ajax/cdn)
* [jQuery CDN](https://code.jquery.com/)
* [Bootstrap CDN](http://www.bootstrapcdn.com/)
* [JavaScript-библиотеки](https://tech.yandex.ru/jslibs/) by [Yandex](https://www.yandex.com/)
* [jsDelivr](http://www.jsdelivr.com/) (multi-CDN infrastructure)
* [cdnjs](https://cdnjs.com/about) powered by [CloudFlare](https://www.cloudflare.com/)

Prerequisites
=============
* [Bash](http://www.gnu.org/software/bash/) (probably any sh-compatible shell)
* [cURL](http://curl.haxx.se/)
* [ping](http://en.wikipedia.org/wiki/Ping_%28networking_utility%29)

Author
======
[Rafał Pocztarski](https://github.com/rsp)

License
=======
This program is open source / free software. See: LICENSE for details.

Download
========
The latest version is available on GitHub:

https://github.com/rsp/ajax-cdn-speed-test
