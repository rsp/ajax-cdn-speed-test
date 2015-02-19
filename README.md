This program tests the speed of various free CDNs (content delivery networks)
that can be used for including JavaScript libraries in your websites
("hot linking" if anyone is still using this term).

Usage
=====
`ajax-cdn-speed-test`

How it works
============
It downloads a minified version of jQuery 2.1.3 over HTTP and displays download time.
It also prints the average ping time for the host. It tests the following CDNs:

* [Microsoft Ajax Content Delivery Network](https://www.asp.net/ajax/cdn)
* [Google Hosted Libraries](https://developers.google.com/speed/libraries/)
* [cdnjs](https://cdnjs.com/about) powered by [CloudFlare](https://www.cloudflare.com/)

Tested CDNs
===========


Prerequisites
=============
* [Bash](http://www.gnu.org/software/bash/) (probably any sh-compatible shell)
* [cURL](http://curl.haxx.se/)

Author
======
[Rafał Pocztarski](https://github.com/rsp)

License
=======
This program is open source / free software. See: LICENSE for details.
