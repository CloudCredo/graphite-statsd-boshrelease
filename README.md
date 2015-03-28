# Graphite BOSH Release

This BOSH release can be used to deploy [Graphite](http://graphite.readthedocs.org/en/0.9.12/overview.html)! The current release configures a single-node Graphite server with the following:

* 1 x carbon-cache.py process
* graphite-web using a sqlite DB (can be configured to use psql)
* Apache httpd and mod_wsgi
* statsd

There is an example [bosh-lite](https://github.com/cloudfoundry/bosh-lite) deployment manifest in the examples directory to help you get started.

# TODO

There is much to be done:

* Add HTTPS and authentication
* Add examples + Getting Started guide
* Add support for multiple carbon processes and > 1 graphite node
* Add support for memcache/AMQP
* Etc...

# Blobs

| Filename | Download URL | MD5 |
| -------- | ------------ | --- |
| python-2.7.9.tar.xz | [www.python.org](https://www.python.org/ftp/python/2.7.9/Python-2.7.9.tar.xz) | 38d530f7efc373d64a8fb1637e3baaa7 |
| zope.interface-4.1.2.tar.gz | [pypi.python.org](https://pypi.python.org/packages/source/z/zope.interface/zope.interface-4.1.2.tar.gz) | 04298faeaa70b4f3b23fa2ae8987262c |
| Twisted-11.1.0.tar.bz2 | [pypi.python.org](https://pypi.python.org/packages/source/T/Twisted/Twisted-11.1.0.tar.bz2) | 972f3497e6e19318c741bf2900ffe31c |
| whisper-0.9.12.tar.gz | [github.com](https://github.com/graphite-project/whisper/archive/0.9.12.tar.gz) | fcaa34d128d13278ba1b8e23443e0871 |
| mocker-1.1.1.tar.bz2 | [pypi.python.org](https://pypi.python.org/packages/source/m/mocker/mocker-1.1.1.tar.bz2) | 0bd9f83268e16aef2130fa89e2a4839f |
| carbon-0.9.12.tar.gz | [github.com](https://github.com/graphite-project/carbon/archive/0.9.12.tar.gz) | 674c7376be70b07a90eecf013dad6600 |
| sqlite-autoconf-3080803.tar.gz | [www.sqlite.org](http://www.sqlite.org/2015/sqlite-autoconf-3080803.tar.gz) | 51272e875879ee893e51070b07c33888 |
| pysqlite-2.6.3.tar.gz | [pypi.python.org](https://pypi.python.org/packages/source/p/pysqlite/pysqlite-2.6.3.tar.gz) | 7ff1cedee74646b50117acff87aa1cfa |
| Django-1.3.tar.gz | [pypi.python.org](https://pypi.python.org/packages/source/D/Django/Django-1.3.tar.gz) | 1b8f76e91c27564708649671f329551f |
| django-tagging-0.3.1.tar.gz | [pypi.python.org](https://pypi.python.org/packages/source/d/django-tagging/django-tagging-0.3.1.tar.gz) | a0855f2b044db15f3f8a025fa1016ddf |
| libpng-1.6.16.tar.gz | [prdownloads.sourceforge.net](http://prdownloads.sourceforge.net/libpng/libpng-1.6.16.tar.gz?download) | 1a4ad377919ab15b54f6cb6a3ae2622d |
| pixman-0.32.6.tar.gz | [cairographics.org](http://cairographics.org/releases/pixman-0.32.6.tar.gz) | 3a30859719a41bd0f5cccffbfefdd4c2 |
| freetype-2.5.5.tar.gz | [download.savannah.gnu.org](http://download.savannah.gnu.org/releases/freetype/freetype-2.5.5.tar.gz) | 7448edfbd40c7aa5088684b0a3edb2b8 |
| expat-2.1.0.tar.gz | [netcologne.dl.sourceforge.net](http://netcologne.dl.sourceforge.net/project/expat/expat/2.1.0/expat-2.1.0.tar.gz) | dd7dab7a5fea97d2a6a43f511449b7cd |
| fontconfig-2.11.1.tar.bz2 | [www.freedesktop.org](http://www.freedesktop.org/software/fontconfig/release/fontconfig-2.11.1.tar.bz2) | 824d000eb737af6e16c826dd3b2d6c90 |
| cairo-1.14.0.tar.xz | [cairographics.org](http://cairographics.org/releases/cairo-1.14.0.tar.xz) | fc3a5edeba703f906f2241b394f0cced |
| py2cairo-1.10.0.tar.bz2 | [www.cairographics.org](http://www.cairographics.org/releases/py2cairo-1.10.0.tar.bz2) | 20337132c4ab06c1146ad384d55372c5 |
| pytz-2014.10.tar.gz | [pypi.python.org](https://pypi.python.org/packages/source/p/pytz/pytz-2014.10.tar.gz) | eb1cb941a20c5b751352c52486aa1dd7 |
| graphite-web-0.9.12.tar.gz | [github.com](https://github.com/graphite-project/graphite-web/archive/0.9.12.tar.gz) | c09f19fc0076cbadec64039f161bafc0 |
| httpd-2.4.12.tar.gz | [apache.mirror.anlx.net](http://apache.mirror.anlx.net//httpd/httpd-2.4.12.tar.gz) | ec8676a7fe62433883868b8341da6734 |
| apr-1.5.1.tar.gz | [mirror.vorboss.net](http://mirror.vorboss.net/apache//apr/apr-1.5.1.tar.gz) | d3538d67e6455f48cc935d8f0a50a1c3 |
| apr-util-1.5.4.tar.gz | [mirror.vorboss.net](http://mirror.vorboss.net/apache//apr/apr-util-1.5.4.tar.gz) | 866825c04da827c6e5f53daff5569f42 |
| pcre-8.36.tar.gz | [garr.dl.sourceforge.net](http://garr.dl.sourceforge.net/project/pcre/pcre/8.36/pcre-8.36.tar.gz) | ff7b4bb14e355f04885cf18ff4125c98 |
| mod_wsgi-4.4.9.tar.gz | [github.com](https://github.com/GrahamDumpleton/mod_wsgi/archive/4.4.9.tar.gz) | afc9e65587cab4aab3b2fa8b8c41ceae |
| statsd-v0.7.2.tar.gz | [github.com](https://github.com/etsy/statsd/archive/v0.7.2.tar.gz) | fd7e4bec91ce8c765f9a88b81cbf96bb |
| node-v0.12.0.tar.gz | [nodejs.org](http://nodejs.org/dist/v0.12.0/node-v0.12.0.tar.gz) | 62c8d9c74c8f68193f60e4cba020eb48 |
| postgresql-9.4.1.tar.gz | [ftp.postgresql.org](https://ftp.postgresql.org/pub/source/v9.4.1/postgresql-9.4.1.tar.gz) | 8df613a83654a32ba5a1008510234931 |
| psycopg2-2.6.tar.gz | [initd.org](http://initd.org/psycopg/tarballs/PSYCOPG-2-6/psycopg2-2.6.tar.gz) | fbbb039a8765d561a1c04969bbae7c74 |
