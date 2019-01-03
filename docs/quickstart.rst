Quickstart
==========

To try Parsl now (without installing any code) experiment with our `hosted tutorial notebooks <http://try.parsl-project.org>`_.


Installation
------------

Parsl is available on PyPI, but first make sure you have Python3.5+

>>> python3 --version

Parsl has been tested on Linux and MacOS.


Installation using Pip
^^^^^^^^^^^^^^^^^^^^^^

While ``pip`` and ``pip3`` can be used to install Parsl we suggest the following approach
for reliable installation when many Python environments are avaialble.

1. Install Parsl::

     $ python3 -m pip install parsl

     (to update a previously installed parsl to a newer version, use: python3 -m pip install -U parsl)

2. Install Jupyter for Tutorial notebooks::

     $ python3 -m pip install jupyter


.. note:: For more detailed info on setting up Jupyter with Python3.5 go `here <https://jupyter.readthedocs.io/en/latest/install.html>`_


Installation using Conda
^^^^^^^^^^^^^^^^^^^^^^^^

1. Install Conda and setup python3.6 following the instructions `here <https://conda.io/docs/user-guide/install/macos.html>`_::

     $ conda create --name parsl_py36 python=3.6
     $ source activate parsl_py36

2. Install Parsl::

     $ python3 -m pip install parsl

     (to update a previously installed parsl to a newer version, use: python3 -m pip install -U parsl)

Installation of Optional Packages
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Parsl supports several optional components that require additional module installations.
For example support for Amazon Web Services, Extreme Scale Executor etc require additional packages that
can be installed easily via `pip` using a pip extras option.

Here's a list of the components and their extras option:

* Amazon Web Services (Cloud) : `aws`
* Google Cloud : `google_cloud`
* Extreme Scale Executor (Supercomputing) : `extreme_scale`
* Database logging of monitoring data : `db_logging`
* Jetstream (NSF Cloud) : `jetstream`

Optional extras can be installed using the following syntax::

     $ python3 -m pip install parsl[<optional_package1>, <optional_package2>]

For Developers
--------------

1. Download Parsl::

    $ git clone https://github.com/Parsl/parsl

2. Install::

    $ cd parsl
    $ pip install .
    ( To install specific extra options from the source :)
    $ pip install .[<optional_pacakge1>...]

3. Use Parsl!

Requirements
------------

Parsl requires the following:

* Python 3.5+

For testing:

* nose
* coverage

For building documentation:

* nbsphinx
* sphinx
* sphinx_rtd_theme
