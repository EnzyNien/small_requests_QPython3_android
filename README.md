
Small changes in urequests to work with QPython3 on android.
Is a weak alternative to "requests"

# wipy-urllib

This version of urllib is designed to be used with Micropython.

Usage is similar to normal urllib:

> import urequests  
> f = urequests.py.urlopen('http://www.micropython.org')  
> f.code  
> f.headers  
> f.read()

It is possible to do posts:
> f = urequests.urlopen('http://www.someurl.com', {'input': 'value'})

There are also methods for urlencoding:
> urequests.urlencode('abc 123')  
> urequests.quote('abc 123')  
> urequests.quote_plus('abc 123')  
> urequests.unquote('abc%20123')  
> urequests.unquote_plus('abc+123')

Discussion available at http://forum.micropython.org/viewtopic.php?f=11&t=1080

# urequests

First version of urequests for micropython

Supports:
 - SSL
 - Cookies
 - Basic Auth
 - Custom HTTP Headers
 - GET, POST, PUT, DELETE, OPTIONS, HEAD

Similar interface to http://docs.python-requests.org/en/latest/
