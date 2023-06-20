Flask
======


Install
-------

    # clone the repository
    $ git clone https://github.com/robelberhanu/python_flask_tutorial.git
    $ cd flask_tutorial

Create a virtualenv and activate it::

    $ python3 -m venv env
    $ . env/bin/activate

Or on Windows cmd::

    $ py -3 -m venv env
    $ env\Scripts\activate.bat

Install Flask::

    $ pip install Flask .


Run
---

.. code-block:: text

    $ flask --app flask_tutorial init-db
    $ flask --app flask_tutorial run --debug

Open http://127.0.0.1:5000 in a browser.


Test
----

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser
