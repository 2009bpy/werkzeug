public: yes

Welcome
=======

    Werkzeug is a WSGI utility library for Python.  It's widely used and
    BSD licensed.

Werkzeug is Simple
------------------

::

    from werkzeug.wrappers import Request, Response

    @Request.application
    def application(request):
        return Response('Hello World!')

    if __name__ == '__main__':
        from werkzeug.serving import run_simple
        run_simple('localhost', 4000, application)

And Powerful
------------

Werkzeug started as a simple collection of various utilities for WSGI
applications and has become one of the most advanced WSGI utility modules.
It includes a powerful debugger, fully featured request and response
objects, HTTP utilities to handle entity tags, cache control headers, HTTP
dates, cookie handling, file uploads, a powerful URL routing system and a
bunch of community contributed addon modules.

It does Unicode and doesn't enforce a specific template engine, database
adapter or anything else.  It doesn't even enforce a specific way of
handling requests and leaves all that up to the developer.

In the Box
----------

-   HTTP header parsing and dumping
-   Easy to use request and response objects
-   Interactive JavaScript based in-browser debugger
-   100% WSGI 1.0 compatible
-   Supports Python 2.6, 2.7 and 3.3+
-   Unicode support
-   Basic session and signed cookie support
-   URI and IRI utilities with unicode awareness
-   builtin library of fixes for buggy WSGI servers and browsers
-   integrated routing system for matching URLs to endpoints and vice
    versa

A Strong Foundation
-------------------

Werkzeug is the base of frameworks such as `Flask`_ and more, as well as
in house frameworks developed for commercial products and websites.

What other people say
---------------------

    Have you looked at werkzeug.routing? It's hard to find anything that's
    simpler, more self-contained, or purer-WSGI than Werkzeug, in general
    — I'm quite a fan of it!  —  `Alex Martelli
    <http://en.wikipedia.org/wiki/Alex_Martelli>`_


Contribute
----------

Found a bug? Have a good idea for improving Werkzeug? Head over to
`Werkzeug's new github <http://github.com/mitsuhiko/werkzeug>`_ page and
create a new ticket or fork.  If you just want to chat with fellow
developers, visit the `IRC channel </community/#irc-channel>`_ or join the
`mailinglist </community/#mailinglist>`_. 

.. raw:: html

    <a href="http://github.com/mitsuhiko/werkzeug"><img style="position: fixed; top: 0; right: 0; border: 0;"
       src="http://s3.amazonaws.com/github/ribbons/forkme_right_gray_6d6d6d.png" alt="Fork me on GitHub"></a>


.. _Flask: http://flask.pocoo.org/
