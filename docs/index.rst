.. SmartDL documentation master file, created by
   sphinx-quickstart on Sat Jun 29 13:36:18 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Python Smart Download Manager -- pySmartDL
==========================================

``pySmartDL`` strives to be a full-pleged smart download manager for Python. Main features:

* Built-in download acceleration (with the `multipart downloading technique <http://stackoverflow.com/questions/93642/how-do-download-accelerators-work>`_).
* Mirrors support.
* Pause/Unpause feature.
* Hash checking.
* Non-blocking, shows progress bar, download speed and eta.

=============
Project Links
=============

 * Downloads: http://pypi.python.org/pypi/pySmartDL/
 * Documentation: http://itaybb.github.io/pySmartDL/
 * Project page: https://github.com/iTaybb/pySmartDL/
 * Bugs and Issues: https://github.com/iTaybb/pySmartDL/issues

=====
Usage
=====

Download is as simple as creating an instance and launching it::

	import os
	from pySmartDL import SmartDL

	url = "http://mirror.ufs.ac.za/7zip/9.20/7za920.zip"
	dest = "C:\\Downloads\\" # or '~/Downloads/' on linux

	obj = SmartDL(url, dest)
	obj.start()
	# [*] 0.23 / 0.37 MB @ 88.00KB/s [##########--------] [60%, 2s left]

	path = obj.get_dest()

==============
Requirements
==============

 * Python 2.6 or 2.7.
 * The `threadpool  <https://pypi.python.org/pypi/threadpool>`_ package.

Documentation
=====================================

.. toctree::
   :maxdepth: 2
   
   examples
   code
   notes
   todo

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

