Python-bing-translate-layer
=========

Python module for interfacing with **the latest** Windows Azure Marketplace \ Microsoft Translate API \ Whatever its name is now.

What's the name of the "Do whatever the fuck you want with this, just credit me\show me what your doing with it" license?

*You are welcomed to expand this module or notify me about issues.*

**Last check** that this module worked: 3th July 2013' (Microsoft could have changed the API by the time you're looking at this)

Features
--------

- translate a text or html file in a language into another language
- Stores the access_token and the expiration date in the background. Uses that access_token unless 10 minutes have passed since it's generation (and then generate a new one).

TODO (someday)
----
- test it with HTML requests (only tested with individual words)

Prerequisites
-------------

 - You need an API key from the "DataMarket" https://datamarket.azure.com/account/keys
 - You need to create an application for a Client_Id and a Client_Secret, also from the "DataMarket" https://datamarket.azure.com/developer/applications/

Install
-------

Import this module from your code. No need to install anything.

Example
-------

Look at the tests.py. OR:

~~~~.python
import translate as tas
tas.set_credentials(app_id='YOURAPPID',client_id='YOURCLIENTID',client_secret='YOURCLIENTSECRET')
print tas.translate('hello', 'en', 'ko')
~~~~

Homepage
--------

https://github.com/wildeyes/python-bing-translate-layer

Wildeyes.