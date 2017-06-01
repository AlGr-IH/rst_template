RST Template
============

Document Sectioning
-------------------

In rst sections are identified through their titles, which are marked up with adornment: "underlines" below the title text, or underlines and matching "overlines" above the title. An underline/overline is a single repeated punctuation character that begins in column 1 and forms a line extending at least as far as the right edge of the title text. Specifically, an underline/overline character may be any non-alphanumeric printable 7-bit ASCII character. When an overline is used, the length and character used must match the underline. Underline-only adornment styles are distinct from overline-and-underline styles that use the same character. There may be any number of levels of section titles [rstSections].

The hierarchy of the sectioning symbols is defined during the build process of the document through their order of appearance. I suggest to restrict the hierachy in the BigGIS documentation to no more than 4 levels using the following scheme: ::

	Chapter
	=======
	
	Section
	---------

	Subsection
	...........

	Subsubsection
	*************

Please refer to the RST manual for further reading on `sections <http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#sections>`_.

Images and Figures
-------------------

A "figure" consists of image data (including image options), an optional caption (a single paragraph), and an optional legend (arbitrary body elements). This is an example for a centered figure scaled to 50% with caption and legend.

.. _my-figure:

.. figure:: images/scen-smartcity.*
	:scale: 50 %
	:alt: smartcity symbol
	:align: center

	This is the caption of the figure (a simple paragraph).

	The legend consists of all elements after the caption. In this case, the legend consists of this paragraph

Reference to the figure :numref:`(Fig. %s) my-figure`

TODO: Figure enumeration and referencing (siehe http://www.sphinx-doc.org/en/stable/markup/inline.html#cross-referencing-figures-by-figure-number )

For further reading on `images <http://docutils.sourceforge.net/docs/ref/rst/directives.html#image>`_ and `figures <http://docutils.sourceforge.net/docs/ref/rst/directives.html#figure>`_ refer to the rst documentation.

References
-------------

.. [rstSections] RST documentation (Sections), http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#sections

