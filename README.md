Mikeotizels HTTPD AutoIndex CSS
===============================

Version 1.0.0 / Apache 2.4

This package contains custom CSS that can be used with Apache HTTP Server as 
the Index StyleSheet for server-generated directory listings.

# Usage

Place the "httpd.autoindex.min.css" file in the `./dist` folder in a location 
of your choice then modify the Apache IndexStyleSheet directive to set the 
name of the file that will be used as the CSS for the index listing. Eg.:
  `IndexStyleSheet "/assets/css/httpd.autoindex.min.css"`

Please refer to the Apache HTTP Server [mod_autoindex][1] module docs for more 
information about HTTPD AutoIndex. 

  [1]: https://httpd.apache.org/docs/2.4/mod/mod_autoindex.html