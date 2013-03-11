http403
=======

Http403 response from http://devwithpassion.com/felipe/manipulando-erros-http-403-permissao-negada-no-django/

This will be integrated with django-response-helpers

https://github.com/chronossc/django-response-helpers/
https://github.com/imtapps/django-response-helpers
http://pypi.python.org/pypi/django-response-helpers

Usage
-----
Add this to your middleware:

    MIDDLEWARE_CLASSES += (
         'http403project.http.HttpExceptionMiddleware',
    )

Then in a view:

    from http403project.http import HttpException
    raise HttpException('Custom message here.', status=403)

Forked by seddonym (David Seddon) so that it can be installed using pip. 
