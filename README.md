pyfpdf: FPDF for Python
=======================

This is a fork of the PyFPDF library and fixes unicode issues. It allows usage
of non-latin-1 characters (e.g. Euro sign €) in Python 3. This is possible
by internally using a bytearray output buffer instead of a string (and should
also be more efficient). This library is used by [reportbro-lib][2]
(see [ReportBro][3]).

PyFPDF is a library for PDF document generation under Python, ported from PHP
(see [FPDF][1]: "Free"-PDF, a well-known PDFlib-extension replacement with many
examples, scripts and derivatives).

Compared with other PDF libraries, PyFPDF is simple, small and versatile, with
advanced capabilities, and is easy to learn, extend and maintain.

  [1]: http://www.fpdf.org/
  [2]: https://github.com/jobsta/reportbro-lib/
  [3]: https://www.reportbro.com/

Features:
---------

 * Python 2.7 and 3.5+ support
 * Unicode (UTF-8) TrueType font subset embedding
 * Barcode I2of5 and code39, QR code coming soon ...
 * PNG, GIF and JPG support (including transparency and alpha channel)
 * Templates with a visual designer & basic html2pdf 
 * Exceptions support, other minor fixes, improvements and PEP8 code cleanups
 
Installation Instructions:
--------------------------

You can install PyFPDF from PyPI, with easyinstall or from Windows 
installers. For example, using pip:
```
   pip install reportbro-fpdf
```

To get the latest development version you can download the source code running:

```
   git clone https://github.com/jobsta/pyfpdf.git
   cd pyfpdf
   python setup.py install
```

**Note:** the [Python Imaging Library](http://www.pythonware.com/products/pil/) 
(PIL) is needed for GIF support. PNG and JPG support is built-in and doesn't 
require any external dependency. For Python 3, 
[Pillow - The friendly PIL fork](https://github.com/python-pillow/Pillow) is 
supported.

Documentation:
--------------
[![Documentation Status](https://readthedocs.org/projects/pyfpdf/badge/?version=latest)](http://pyfpdf.rtfd.org)

 * [Read the Docs](http://pyfpdf.readthedocs.org/en/latest/)
 * [FAQ](docs/FAQ.md)
 * [Tutorial](docs/Tutorial.md) (Spanish translation available)
 * [Reference Manual](docs/ReferenceManual.md)

For further information, see the project site:
https://github.com/reingart/pyfpdf or the old Google Code project page
https://code.google.com/p/pyfpdf/.

