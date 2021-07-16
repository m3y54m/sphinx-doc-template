.. _install-sphinx:

Installing Sphinx
====================
Sphinx is based on Python so you should have Python installed on your system. Although it is possible to install Python and Sphinx in Windows, it's recommended to use a Linux distribution preferably Ubuntu for this purpose.

If your main OS is Windows, you can use VMWare or VirtualBox to install Ubuntu as a guest OS.

In order to start using Sphinx and generate documents first of all you need to install the Sphinx engine:

.. prompt:: bash $

  sudo apt-get install python3-sphinx

Then you should initialize your documentation build environment:

.. prompt:: bash $

  sphinx-quickstart

Having a nice theme gives an elegant appearance to your documentation and make it much more readable:

.. prompt:: bash $

  pip install sphinx-rtd-theme
 
The default language supported in Sphinx is reStructuredText. If you prefer Markdown you can install it on Sphinx using this command:

.. prompt:: bash $

  pip install recommonmark

Whenever you need to generate the HTML output you can use this command:

.. prompt:: bash $

  make html
 
If you want to have a beautiful PDF output you should first install the LaTeX engine:

.. prompt:: bash $

  sudo apt-get install texlive-latex-recommended
  sudo apt-get install texlive-fonts-recommended
  sudo apt-get install texlive-latex-extra
  sudo apt-get install latexmk
  
Then by entering the following command the PDF output will be generated:

.. prompt:: bash $ 
 
  make latexpdf
  
Required packages for build process of Sphinx are put in a file called ``requirements.txt``. Use the following command to install them:

.. prompt:: bash $

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
