=============
Pyramid Nitro
=============

.. IMPORTANT::

  This package is currently in the "planning" stage. In short, much of
  the conceptual parts of the package exist in disparate locations:
  this package was created to bring those concepts together.


The `pyramid_nitro` package adds dependencies, useful libraries,
sensible default configurations, "glue code", and other goodies to a
"standard pyramid application" that makes developing pyramid
applications fast... *super* fast. In short, it's the "batteries
included" *opinionated* version of Pyramid_. It draws it's inspiration
from the TurboGears_ application framework.


Project
=======

* Homepage: https://github.com/canaryhealth/pyramid_nitro
* Bugs: https://github.com/canaryhealth/pyramid_nitro/issues


TL;DR
=====

Install with:

.. code-block:: bash

  $ pip install pyramid_nitro

Then create an application with:

.. code-block:: bash

  $ nitro "myapp" /path/to/myapp
  $ cd /path/to/myapp
  $ nitro etc/dev.ini


Overview
========

The objectives of `pyramid_nitro` are three-fold:

* Trivial to get a completely functional application going
* Lots of out-of-the-box functionality, but nothing that can't be disabled
* Support for infinite scalability when needed

Some of the opinions made to achieve that is that you'll:

* expose and document API endpoints with pyramid_controllers_ and pyramid_describe_
* parse and serialize HTTP requests with pyramid_input_ and pyramid_output_
* validate and sanitize data formats with pyramid_armor_
* authenticate requests with SAML or models with (TODO: to be determined)
* perform access control with pyramid_authz_
* paginate response datasets with pyramid_pagination_
* use SQLAlchemy_ for your ORM model
* store ORM data in PostgreSQL_ and big data in MongoDB_
* send message bus events over RabbitMQ_
* schedule asynchronous and deferred jobs with pyramid_scheduler_
* manage configurations with pyramid_iniherit_
* generate JavaScript, CSS, and images with pyramid_webassets_, lessc_
* enable sessions and caching with pyramid_beaker_
* encrypt data with GPG keys
* thoroughly implement unit/integration/system tests with pyramid_test_
* think globally but act locally with i18n
* use Apache_ to infinity-scale your server
* depend on microservices, such as:

  * indexing and searching with Solr_
  * URL-shortening with pyramid_tinyurl_




.. _Pyramid: http://www.pylonsproject.org/
.. _TurboGears: http://www.turbogears.org/
.. _pyramid_controllers: https://pypi.python.org/pypi/
.. _pyramid_describe: https://pypi.python.org/pypi/pyramid_describe
.. _pyramid_input: https://pypi.python.org/pypi/pyramid_input
.. _pyramid_output: https://pypi.python.org/pypi/pyramid_output
.. _pyramid_armor: https://pypi.python.org/pypi/pyramid_armor
.. _pyramid_authz: https://pypi.python.org/pypi/pyramid_authz
.. _pyramid_pagination: https://pypi.python.org/pypi/pyramid_pagination
.. _pyramid_scheduler: https://pypi.python.org/pypi/pyramid_scheduler
.. _pyramid_iniherit: https://pypi.python.org/pypi/pyramid_iniherit
.. _pyramid_webassets: https://pypi.python.org/pypi/pyramid_webassets
.. _pyramid_tinyurl: https://pypi.python.org/pypi/pyramid_tinyurl
.. _pyramid_test: https://pypi.python.org/pypi/pyramid_test
.. _lessc: https://pypi.python.org/pypi/lessc
.. _pyramid_beaker: https://pypi.python.org/pypi/pyramid_beaker
.. _SQLAlchemy: http://www.sqlalchemy.org/
.. _PostgreSQL: https://www.postgresql.org/
.. _MongoDB: https://www.mongodb.org/
.. _RabbitMQ: https://www.rabbitmq.com/
.. _Apache: https://httpd.apache.org/
.. _Solr: https://lucene.apache.org/solr/
