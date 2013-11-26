epub-testfiles
==============
Epub files to test EPUB Reading system implementation.

Test cases
--------------
### 1. XML file encoding
*[epub files](http://github.com/tkanai/epub-testfiles/tree/master/encoding-check)*

The files are to check whether Reading System handles supported "Unicode" files correctly or not.

#### NOTE:
The EPUB standard states "Any Publication Resouce that is an XML-Based Media Type must be encoded in UTF-8 or UTF-16" in EPUB Publications 3.0.
But there are some variations of UTF-8 and UTF-16, technically, and the test files cover UTF-8, UTF-8 with BOM and UTF-16LE encodings.

#### Files:
Each file name consists of three identifiers.

    test-fileencoding-[A]-[B]-[C]

  * [A] indicates which encoding is applyed for container.xml
  * [B] indicates which encoding is applyed for .opf
  * [C] indicates which encoding is applyed for the navigation document in the file.

##### About the encoding identifiers
  * "8" means the file is encoded in UTF-8.
  * "8b" means the file is encoded in UTF-8 with BOM.
  * "16" means the file is encoded in UTF-16LE.

*Each epub file contains three xhtml files as epub content, and each xhtml file is encoded in each encoding.*
