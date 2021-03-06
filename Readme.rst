|language| |license|

=========
pyudpscan
=========

Description
~~~~~~~~~~~

Fast and simple UDP port scanner with SOCKS5 proxy support.
Compare to nmap this thing can do direct UDP scanning twice faster
with same precise and also has possibility to do scan through SOCKS5 proxy.

Installation
~~~~~~~~~~~~

``python setup.py install``

or

``pip install -e .``

or

``pip install pyudpscan``

How to use
~~~~~~~~~~

Run ``sudo pyudpscan --proxy 99.99.99.99:1080 --host 8.8.0-8.0/24 --ports 20-22 53 -i eth0``

Also checkout list of `arguments`_

arguments
^^^^^^^^^
* ``-H, --hosts`` - List of target hosts/subnets/ranges separated by space.
* ``-P, --ports`` - List of target ports/ranges separated by space.
* ``-p, --proxy`` - List of SOCKS5 proxies which will be taken at random for every ip.
* ``-t, --timeout`` - How long to wait for reply at UDP request from target host.
* ``-r, --recheck`` - Number of recheck for every port.
* ``-D, --decoys`` - List of decoys to use.
* ``-i, --interface`` - Name of local source interface to listen on.

.. |language| image:: https://img.shields.io/badge/language-python-blue.svg
.. |license| image:: https://img.shields.io/badge/license-Apache%202-blue.svg


