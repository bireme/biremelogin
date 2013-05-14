BIREME Login
===========

Changes the django's default authentication backend to authenticate in Bireme Accounts Service

How to Install
==============

* Add `biremelogin` folder to your project
* Add `biremelogin` to your installed apps
* Add the code below in settings.py

```
  AUTHENTICATION_BACKENDS = (
    'biremelogin.authenticate.EmailModelBackend',
  )

  BIREMELOGIN_BASE_URL = "http://accounts.teste.bireme.org"
  BIREMELOGIN_SERVICE = "DIREVE"
```

* Where:
  *  __BIREMELOGIN_BASE_URL:__ The API url
  *  __BIREMELOGIN_SERVICE:__ The Service that the app will be instaled
