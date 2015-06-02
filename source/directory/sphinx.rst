.. contents:: Table of Contents
   :depth: 2

########################
Main Sphinx Example File
########################

.. usually # over and under is for Part One or Two or so on of a book

***********
Chapter One
***********

.. * over and under for a chapter, = over and under for a top level header, and so on

==========
Header One
==========

Header Two
==========

Header Three
------------

Header Four
^^^^^^^^^^^

Header Five
"""""""""""

Here is a paragraph that is spread
across multiple lines in the source
but will display on one line in the 
built html file.

a *italic* b **bold** c ``literal`` d

a :emphasis:`emphasis` b :strong:`strong` c :literal:`literal`
d :subscript:`subscript` e :superscript:`superscript` f 
:title-reference:`title-reference` g

character escaping with backslashes: thisis\ *one*\ word


* bullet
* list with a very long second item 
  on two lines.

1. numbered
2. list

a

#. another numbered
#. list

* bullet
* list

  * with
  * nesting

* which then continues

This is a paragraph split across
two lines.

  This is an indented paragraph
  below it.

Here is another left justified paragraph.

| This paragraph with line blocks
| has line breaks in the html output
| just as it does in the rst input.

.. This is a comment.

..
   This whole indented block
   is a comment.

   Still in the comment.

Now out of the comment.

.. code-block:: html

  <html>
    <head>Hello!</head>
    <body>Hello, world!</body>
  </html>

.. code-block:: yaml

  envs_dirs:
    - ~/my-envs
    - /opt/anaconda/envs

.. code-block:: bash

  ls
  pwd
  cat foo.txt

.. code-block:: python

  for i in range(10):
    print(i)

If no other type applies, use "none". It can be useful for 
obscure languages or mixtures of languages.

.. code-block:: none

  cat program.py

  for i in range(10):
      print(i)

Grid table with header:

+----------+-----------+-------+
| a        | b         | c     |
+==========+===========+=======+
| north    | north     | north |
| west     |           | east  |
+----------+-----------+-------+
| west     | center    | east  |
+----------+-----------+-------+
| south    | south     | south |
| west     |           | east  |
+----------+-----------+-------+

Grid table without:

+----------+-----------+-------+
| north    | north     | north |
| west     |           | east  |
+----------+-----------+-------+
| west     | center    | east  |
+----------+-----------+-------+
| south    | south     | south |
| west     |           | east  |
+----------+-----------+-------+

"Simple tables" are easier to write, but must have 
more than one row, and the first column cannot contain multiple lines:

=====  =====  =======
A      B      A and B
=====  =====  =======
False  False  False
True   False  False
False  True   False
True   True   True
=====  =====  =======

http://microsoft.com

`Google <http://google.com>`_

This paragraph links to `the yahoo site`_.

.. _the yahoo site: http://yahoo.com/


This text refers to a :ref:`my-reference-label` section ahead.

.. _my-reference-label:

Section to cross-reference
--------------------------

This is the text of the section.

Here is a :ref:`link to another section<label-two>` up ahead.

.. _label-two:

Section for other cross reference
---------------------------------

Sphinx supports automatic cross references to :doc:`a document called two<two>` in the same archive.

The link caption defaults to the document title if no other title is given: :doc:`two`

Or with absolute pathname: :doc:`/directory/two`

Please see the ``contents`` directive in the source of this file and ``two.rst``, and
the ``toctable`` directive in ``index.rst``.

The document ``/sketches/index`` could refer to the document ``/people`` by absolute name 
as ``:doc:`/people``` or by relative name as ``:doc:`../people``` and could 
refer to ``/sketches/parrot`` by absolute name as ``:doc:`/sketches/parrot``` or by 
relative name as ``:doc:`parrot```.

..
   This is allowed in rst in general, but produces a 'nonlocal image' warning in sphinx:

   .. image:: http://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Green_eyes_kitten.jpg/120px-Green_eyes_kitten.jpg

   So, make sure your images are local images.

.. image:: Puppy_2.jpg

abcd

.. note:: This is a note admonition.
   This is the second line of the first paragraph.

   - The note contains all indented body elements
     following.
   - It includes this bullet list.

abcd

.. raw:: html

        <iframe width="560" height="315" src="https://www.youtube.com/embed/UaIvrDWrIWM" frameborder="0" allowfullscreen></iframe>


intro to sphinx http://docs.writethedocs.org/tools/sphinx/

rst primer http://sphinx-doc.org/rest.html

first steps w sphinx http://sphinx-doc.org/tutorial.html

links http://sphinx-doc.org/markup/inline.html#ref-role

http://reinout.vanrees.org/weblog/2009/10/30/restructured-text-cheat-sheet.html

RST cheat sheet http://openalea.gforge.inria.fr/doc/openalea/doc/_build/html/source/sphinx/rest_syntax.html

