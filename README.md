Mikeotizels HTTPD AutoIndex CSS
===============================

Version 2.0.0 / Apache HTTP Server 2.4.x

This package contains custom CSS that can be used with Apache HTTP Server as 
the Index StyleSheet for server-generated directory listings.

# Usage

Place the "httpd.autoindex.min.css" file in the `./dist` folder in a location
of your choice then modify the Apache HTTPD `IndexStyleSheet` directive in your 
'httpd-autoindex.conf' file to set the name of the file that will be used as 
the CSS for the index listing. For example:

```httpd-autoindex.conf
IndexStyleSheet "/assets/css/httpd.autoindex.min.css"
```

Please refer to the Apache HTTP Server [mod_autoindex][1] module documentation 
for more information about HTTPD AutoIndex module. 

You may also need to include the "/assets/" alias for the 'assets' directory if 
you it is not relative to the server's document root. See the [mod_alias][3]
module documentation for more information.

# Tuning

The Index Styles in this package displays the directory listings well with the 
the following index options included in the HTTPD [IndexOptions][2] directive: 

```httpd-autoindex.conf
IndexOptions FancyIndexing HTMLTable IconWidth=15 IconHeight=15 NameWidth=*
```

  [1]: https://httpd.apache.org/docs/2.4/mod/mod_autoindex.html
  [2]: https://httpd.apache.org/docs/2.4/mod/mod_autoindex.html#indexstylesheet
  [3]: https://httpd.apache.org/docs/2.4/mod/mod_alias.html

-------------------------------------------------------------------------------

Enjoy!

Michael Otieno