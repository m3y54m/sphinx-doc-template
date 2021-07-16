.. Comment

reStructuredText Styling Examples
==================================

Titles
-------------

=, for sections

-, for subsections

^, for subsubsections

", for paragraphs


Bold, Italic
------------------

This is normal text. **This is bold text**

This is normal text. *This is italic text.*

Footnote
-----------

Lorem ipsum dolor sit amet, est ne exerci vivendum accusata, nec molestiae scripserit eloquentiam in,
quodsi moderatius argumentum est ad. Autonumbered footnotes are
possible, like using [#]_ and [#]_.

.. [#] This is the first one.
.. [#] This is the second one.


Table
--------

=====  =====  ======
Inputs        Output
------------  ------
  A      B    A or B
=====  =====  ======
False         False
------------  ------
True   False  True
False  True   True
True          True
============  ======


Note and Warning Boxes
----------------------

.. note::

      Lorem ipsum dolor sit amet, est ne exerci vivendum accusata, nec molestiae scripserit eloquentiam in,
      quodsi moderatius argumentum est ad. Aliquam denique nam in. Malorum percipit sed cu. Ut est vide suscipit,
      an nonumy alterum liberavisse his. Mazim fastidii vim et, vim id noster instructior. At audiam bonorum vim,
      te tantas facete vel.

.. warning::

      Lorem ipsum dolor sit amet, est ne exerci vivendum accusata, nec molestiae scripserit eloquentiam in,
      quodsi moderatius argumentum est ad. Aliquam denique nam in. Malorum percipit sed cu. Ut est vide suscipit,
      an nonumy alterum liberavisse his. Mazim fastidii vim et, vim id noster instructior. At audiam bonorum vim,
      te tantas facete vel.


Inline Code
------------

Lorem ipsum dolor sit amet, :file:`/etc/passwd` est ne exerci vivendum accusata, :code:`result = (1 + x) * 32` nec molestiae scripserit eloquentiam in,
quodsi moderatius press :kbd:`Ctrl` + :kbd:`S` argumentum est ad.

Code Block
------------

.. code-block:: console

  # Console
  sudo apt-get update
  
  
.. code-block:: python

  # Python
  print('Hello, world!')


.. code-block:: cpp
  
  // C++
  #include <iostream>
  using namespace std;
  
  int main() {
      // prints the string enclosed in double quotes
      cout << "This is C++ Programming";
      return 0;
  }


Un-selectable Prompt
---------------------

.. prompt:: bash $

  sudo apt-get update
  sudo apt install build-essential
  sudo apt-get install manpages-dev
  gcc --version
  

Image and Figure
--------------------

.. figure:: /_static/images/baby_hawk.png
    :width: 500px
    :target: http://www.google.com

    This is the caption of the figure with link to http://google.com

.. figure:: /_static/images/baby_hawk.png
    :width: 150px
    
Image in a table
~~~~~~~~~~~~~~~~~~

==========================================  =======================
Image                                       Content               
==========================================  =======================
.. image:: /_static/images/baby_hawk.png    Baby Hawk 1
------------------------------------------  -----------------------
.. image:: /_static/images/baby_hawk.png    Baby Hawk 2
==========================================  =======================

Inline image
~~~~~~~~~~~~~

.. |babyhawk| image:: /_static/images/baby_hawk.png
    :width: 50px

Lorem ipsum dolor |babyhawk| sit amet, est ne exerci vivendum accusata, |babyhawk| molestiae scripserit eloquentiam in


List
-------
This is a bullet list:

* list item 1
* list item 2

More text. **Important:** Always add blank line before and after list!

This is a bullet list:

* list item 1

  * list item 1.1
  * list item 1.2

* list item 2


Numbered List
~~~~~~~~~~~~~~~

some text

#. list item 1
#. list item 2

some text

Field List
~~~~~~~~~~~~

:Authors:
    Tony J. (Tibs) Ibbs,
    David Goodger
    (and sundry other good-natured folks)

:Version: 1.0 of 2001/08/08
:Dedication: To my father.


:0:  True
:1:  False


Math Formula
--------------

.. math::
   :label: myequation

   a^2 + b^2 = c^2

.. math::
   :label: myarray

     x^2 & : x < 0 \\
     x^3 & : x \ge 0 \\

.. math::

    n_{\mathrm{offset}} = \sum_{k=0}^{N-1} s_k n_k


UML Diagrams
-------------------

.. uml::

  == Initialization ==

  Alice -> Bob: Authentication Request
  Bob --> Alice: Authentication Response

  == Repetition ==

  Alice -> Bob: Another authentication Request
  Alice <-- Bob: another authentication Response


.. uml::

  robust "Web Browser" as WB
  concise "Web User" as WU

  WB is Initializing
  WU is Absent

  @WB
  0 is idle
  +200 is Processing
  +100 is Waiting
  WB@0 <-> @50 : {50 ms lag}

  @WU
  0 is Waiting
  +500 is ok
  @200 <-> @+150 : {150 ms}

Cross-referencing
-------------------

Go to first title of :ref:`this page <reStructuredText Styling Examples>`
or learn how to :ref:`install Sphinx <Installing Sphinx>`
or learn how to :ref:`install Sphinx <install-sphinx>`

Links
----------------------------

* `reST & Sphinx Cheat Sheet <https://docs.typo3.org/m/typo3/docs-how-to-document/master/en-us/WritingReST/CheatSheet.html>`_
* `reST & Sphinx Reference <https://docs.typo3.org/m/typo3/docs-how-to-document/master/en-us/WritingReST/Reference.html>`_
* `Getting Started with Sphinx <https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html>`_
* `Rest and Sphinx Memo <https://rest-sphinx-memo.readthedocs.io/en/latest/index.html>`_
* `Sphinx-RTD-Tutorial <https://sphinx-rtd-tutorial.readthedocs.io/en/latest/index.html>`_
* `Code documentation lesson: Sphinx and reStructuredText <https://coderefinery.github.io/documentation/04-sphinx/>`_
* `Quick reStructuredText <https://docutils.sourceforge.io/docs/user/rst/quickref.html>`_
* `reStructuredText Primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_
* `Create Documentation with RST, Sphinx, Sublime, and GitHub <https://sublime-and-sphinx-guide.readthedocs.io/en/latest/index.html>`_
