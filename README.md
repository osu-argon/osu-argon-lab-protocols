# Editing Protocol Files

The lab book is formatted using reStructuredText (.rst).

https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html

The lab book compiled using Sphinx and one of the main features of this is including file snippets. To include a file in a document the 



`.. include:: <file path>` 

is used. 

By nesting files within each other, special care is needed when setting headers for each file. Below is the general formatting style.

There are three types of files/pages in this lab book.

* Recipes
  * A recipe file will use the asterik symbol `****`. 

* Methods
  * A method file will use the equal symbol `====`.

* Tasks
  * A task file will use the hyphen symbol `----`.


## Adding Images

```
.. image:: <image path>
  :width: 400
  :alt: 
```

## Commenting Documents

``` .. Everything after the two periods will not be executed ```

## Building a local version of the protocol book

Under Python install these packages using ``pip install``

```
sphinx
sphinx-autobuild
recommonmark
sphinx_pangeo_theme
```

To build the document run.. 

```
sphinx-build -b html "path\to\content" "path\to\output"
```

To start server that recognizes changes to the files and automatically triggers a rebuild...

```
sphinx-autobuild -b html "path\to\content" "path\to\output"
```
