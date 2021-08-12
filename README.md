# Editing Protocol Files

The lab book is formatted using reStructuredText (.rst).

https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#sections

The lab book compiled using Sphinx and one of the main features of this is including file snippets. To include a file in a document the 

`.. include:: <file path>` 

is used. 

By nesting files within each other, special care is needed when setting headers for each file. Below is the general formatting style.

There are three types of files/pages in this lab book.

* Recipes
* Methods
* Tasks


A recipe file will use the asterik `****`. 

A method file will use the equal `====`.

A task file will use the hyphen  `----`.




## Adding Images

.. image:: https://paper-attachments.dropbox.com/s_0971E35B96C0A3333F4EEB16AF0FCF2CA45AE5B5B56AB83FEC688253E286A3B7_1562172071120_picking_setup_step_02.png
  :width: 400
  :alt: Take a small amount grains from the pile and spread them across the plate.
