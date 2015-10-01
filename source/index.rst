Hyper: HTTP/2 for Python
========================

Hyper is a set of related projects that provide HTTP/2 functionality to Python
projects. The aim is to provide a complete HTTP and HTTP/2 toolbox, ranging
from complete off-the-shelf solutions to projects that solve individual
specific problems. Developers should be able to compose these solutions
together to fit their specific use-cases, using the general-purpose code where
appropriate and writing code to well-defined interfaces where they have
specific requirements.

The hyper project is comprised of the following sub-projects:

- hyper-h2, a complete HTTP/2 protocol stack that does not perform any I/O,
  intended to be independent of framework.
- hyperframe, a HTTP/2 framing layer.
- hpack, a HPACK implementation in pure-Python.

Please follow the links above for more details on each of those sub-projects.
The rest of this documentation applies to the project as a whole.

Contents
--------

.. toctree::
   :maxdepth: 2

   contributing
