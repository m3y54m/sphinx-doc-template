Getting Started with Sphinx
============================
Sphinx is based on Python so you should have Python installed on your system. Although it is possible to install Python and Sphinx in Windows, it's recommended to use a Linux distribution preferably Ubuntu for this purpose.

If your main OS is Windows, you can use VMWare or VirtualBox to install Ubuntu as a guest OS.

In order to start using Sphinx and generate documents first of all you need to install the Sphinx engine:

.. code-block:: console

  sudo apt-get install python3-sphinx


Then you should initialize your documentation build environment:

.. code-block:: console

  sphinx-quickstart


Having a nice theme brings some joy to your documentation and make it much more readable:

.. code-block:: console

  pip install sphinx-rtd-theme \
  sphinx-ustack-theme \
  sphinx-ansible-theme \
  sphinx_redactor_theme
  
For more themes refer to `Sphinx Themes <https://sphinx-themes.org/>`_


The default language supported in Sphinx is reStructuredText. If you prefer Markdown you can install it on Sphinx using this command:

.. code-block:: console

  pip install recommonmark
  

Some other useful packages for Sphinx:

.. code-block:: console

  pip install sphinx-prompt sphinxemoji 

Whenever you want to generate the HTML output you can use this command:

.. code-block:: console

  make html


If you want to have a beautiful PDF output you should first install the LaTeX engine:

.. code-block:: console

  sudo apt-get install texlive-latex-recommended \
  texlive-fonts-recommended \
  texlive-latex-extra \
  latexmk


Then by entering the following command the PDF output will be generated:

.. code-block:: console
 
  make latexpdf


Required packages for build process of Sphinx are put in a file called ``requirements.txt``. Use the following command to install them:

.. code-block:: console

  pip install -r requirements.txt

If you need other packages to be installed on Sphinx, it is recommended to add them to this ``requirements.txt`` file.

----------------------------

To study more about Sphinx and reStructuredText please refer to the following links:

* `reST & Sphinx Cheat Sheet <https://docs.typo3.org/m/typo3/docs-how-to-document/master/en-us/WritingReST/CheatSheet.html>`_
* `reST & Sphinx Reference <https://docs.typo3.org/m/typo3/docs-how-to-document/master/en-us/WritingReST/Reference.html>`_
* `Getting Started with Sphinx <https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html>`_
* `Rest and Sphinx Memo <https://rest-sphinx-memo.readthedocs.io/en/latest/index.html>`_
* `Sphinx-RTD-Tutorial <https://sphinx-rtd-tutorial.readthedocs.io/en/latest/index.html>`_
* `Code documentation lesson: Sphinx and reStructuredText <https://coderefinery.github.io/documentation/04-sphinx/>`_
* `Quick reStructuredText <https://docutils.sourceforge.io/docs/user/rst/quickref.html>`_
* `reStructuredText Primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_
* `Create Documentation with RST, Sphinx, Sublime, and GitHub <https://sublime-and-sphinx-guide.readthedocs.io/en/latest/index.html>`_
