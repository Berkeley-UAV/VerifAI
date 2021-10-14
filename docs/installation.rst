############################################
Getting Started with VerifAI
############################################

VerifAI requires **Python 3.8** or newer.
To install VerifAI from PyPI, execute::

	pip install verifai

Alternatively, if you want to run the examples used in the :doc:`tutorial <tutorial>`, you can download or clone the `VerifAI repository <https://github.com/BerkelelyLearnVerify/VerifAI>`_.
Install `Poetry <https://python-poetry.org/>`_ and then run::

	poetry install

This will install VerifAI into your current virtual environment (or create a new one if needed).
If you will be developing VerifAI, add the ``-E dev`` option when invoking Poetry.

Some features of VerifAI require additional packages: the tool will prompt you if they are needed but not installed.

.. note::

        For Windows, we recommend using `bashonwindows (the Windows subsystem for Linux) <https://docs.microsoft.com/en-us/windows/wsl/install-win10>`_ on Windows 10.  Instructions for installing Poetry on bashonwindows can be found `here <https://python-poetry.org/docs/#osx-linux-bashonwindows-install-instructions>`__.

.. note::

	In the past, the ``GPy`` package did not always install correctly through the automated process. If necessary, you can build it from source as follows::

		git clone https://github.com/SheffieldML/GPy
		find GPy -name '*.pyx' -exec cython {} \
		pip install GPy/
