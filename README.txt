==================
``gs.content.css``
==================
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Core CSS support for GroupServer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

:Authors: `Michael JasonSmith`_,
         Mike Harding,
         Ben Ford,
         Josh Campbell
:Contact: Michael JasonSmith <mpj17@onlinegroups.net>
:Date: 2013-03-12
:Organization: `GroupServer.org`_
:Copyright: This document is licensed under a
  `Creative Commons Attribution-Share Alike 3.0 New Zealand License`_
  by `OnlineGroups.Net`_.

Introduction
============

The core GroupServer_ CSS code implements a style known as "Colour is
for Happy People". It is *deliberately* devoid of colour: just black,
white and greys are used. This means that everything has to rely on
layout (alignment and proximity), shape and typography to make sense.

To this core layout different colourful skins can be added. See
``gs.skin.green`` and ``gs.skin.blue`` for two examples.

Layout
======

The CSS layout is based on a 16px typeface on a 20px line, with all
measurements specified in ems. Below is a table that can be used to convert
between units, pixels and ems. (All measurements should be multiples of
half-units).

+-------+-----+--------+--------------------------------------------+
|       |     |        | Without Border Width (in em)               |
+-------+-----+--------+--------------+--------------+--------------+
| Units |  px |   em   |  Thin (1px)  | Medium (3px) | Thick (6px)  |
+=======+=====+========+==============+==============+==============+
|   0.5 |  10 |  0.625 |        0.562 |        0.438 |        0.250 |
+-------+-----+--------+--------------+--------------+--------------+
|   1.0 |  20 |  1.250 |        1.188 |        1.062 |        0.875 |
+-------+-----+--------+--------------+--------------+--------------+
|   1.5 |  30 |  1.875 |        1.812 |        1.688 |        1.500 |
+-------+-----+--------+--------------+--------------+--------------+
|   2.0 |  40 |  2.500 |        2.438 |        2.312 |        2.125 |
+-------+-----+--------+--------------+--------------+--------------+
|   2.5 |  50 |  3.125 |        3.062 |        2.938 |        2.750 |
+-------+-----+--------+--------------+--------------+--------------+
|   3.0 |  60 |  3.750 |        3.688 |        3.562 |        3.375 |
+-------+-----+--------+--------------+--------------+--------------+
|   3.5 |  70 |  4.375 |        4.312 |        4.188 |        4.000 |
+-------+-----+--------+--------------+--------------+--------------+
|   4.0 |  80 |  5.000 |        4.938 |        4.812 |        4.625 |
+-------+-----+--------+--------------+--------------+--------------+
|   4.5 |  90 |  5.625 |        5.562 |        5.438 |        5.250 |
+-------+-----+--------+--------------+--------------+--------------+
|   5.0 | 100 |  6.250 |        6.188 |        6.062 |        5.875 |
+-------+-----+--------+--------------+--------------+--------------+
|   5.5 | 110 |  6.875 |        6.812 |        6.688 |        6.500 |
+-------+-----+--------+--------------+--------------+--------------+
|   6.0 | 120 |  7.500 |        7.438 |        7.312 |        7.125 |
+-------+-----+--------+--------------+--------------+--------------+
|   6.5 | 130 |  8.125 |        8.062 |        7.938 |        7.750 |
+-------+-----+--------+--------------+--------------+--------------+
|   7.0 | 140 |  8.750 |        8.688 |        8.562 |        8.375 |
+-------+-----+--------+--------------+--------------+--------------+
|   7.5 | 150 |  9.375 |        9.312 |        9.188 |        9.000 |
+-------+-----+--------+--------------+--------------+--------------+
|   8.0 | 160 | 10.000 |        9.938 |        9.812 |        9.625 |
+-------+-----+--------+--------------+--------------+--------------+
|   8.5 | 170 | 10.625 |       10.562 |       10.438 |       10.250 |
+-------+-----+--------+--------------+--------------+--------------+
|   9.0 | 180 | 11.250 |       11.188 |       11.062 |       10.875 |
+-------+-----+--------+--------------+--------------+--------------+
|   9.5 | 190 | 11.875 |       11.812 |       11.688 |       11.500 |
+-------+-----+--------+--------------+--------------+--------------+
|  10.0 | 200 | 12.500 |       12.438 |       12.312 |       12.125 |
+-------+-----+--------+--------------+--------------+--------------+


For values above 10u use the following formula::

       u × 20.0
  em = ────────
         16.0

The only complication are borders. They can throw out the rhythm, so must
be taken off the margin or padding. The last three columns in the above
table have the border widths taken out. For values above 6u take away one
of the following three values:

+--------+-----+-------+
| Size   | px  |  em   | 
+========+=====+=======+
| Thin   |   1 | 0.063 |
+--------+-----+-------+
| Medium |   3 | 0.188 |
+--------+-----+-------+
| Thick  |   6 | 0.375 |
+--------+-----+-------+

Icons
=====

An glyph-font is supplied by this product. Twenty-two icons are provided,
as detailed below.

+-------------+----------------+-----+---------------------------------+
|    Icon     |    Character   |Std? | Note                            |
+=============+================+=====+=================================+
| **Breadcrumb trail**                                                 |
+-------------+----------------+-----+---------------------------------+
| Home        | ``&#x2302;``   | Yes |                                 |
+-------------+----------------+-----+---------------------------------+
| Separator   | ``&#xe000;``   | No  | A right-pointing chevron        |
+-------------+----------------+-----+---------------------------------+
| **Navigation**                                                       |
+-------------+----------------+-----+---------------------------------+
| Left/Prev   | ``&#x25c3;``   | Yes | Replaces "small left-triangle"  |
+-------------+----------------+-----+---------------------------------+
| Up          | ``&#x2b06;``   | Yes | Replaces bold up arrow          | 
+-------------+----------------+-----+---------------------------------+
| Right/Next  | ``&#x25b9;``   | Yes | Replaces "small right-triangle" |
+-------------+----------------+-----+---------------------------------+
| Web feed    | ``&#xe003;``   | No  | The RSS or ATOM symbol          |
+-------------+----------------+-----+---------------------------------+
| Settings    | ``&#x2699;``   | Yes | A cog                           |
+-------------+----------------+-----+---------------------------------+
| Lock        | ``&#x1f512;``  | Yes | Sign in                         |
+-------------+----------------+-----+---------------------------------+
| **Actions**                                                          |
+-------------+----------------+-----+---------------------------------+
| Share       |  ``&#xe001;``  | No  | Arrow pointing out of a box     |
+-------------+----------------+-----+---------------------------------+
| Reply       | ``&#x27a6;``   | Yes | Arrow curving right (redo)      |
+-------------+----------------+-----+---------------------------------+
| Delete      | ``&#x1f5d1;``  | Yes | Wastebasket (rubbish, trash)    |
+-------------+----------------+-----+---------------------------------+
| Search      | ``&#x1f50d;``  | Yes | Magnifying glass                |
+-------------+----------------+-----+---------------------------------+
| **True icons**                                                       |
+-------------+----------------+-----+---------------------------------+
| Picture     | ``&#x1f3a8;``  | Yes | Replaces "artist palette"       |
+-------------+----------------+-----+---------------------------------+
| Movie       | ``&#x1f3a6;``  | Yes | Replaces "movie projector"      |
+-------------+----------------+-----+---------------------------------+
| Sound       | ``&#x1f509;``  | Yes | Speaker                         |
+-------------+----------------+-----+---------------------------------+
| Documents   | ``&#x1f4da;``  | Yes | Replaces "empty pages"          |
+-------------+----------------+-----+---------------------------------+
| Attach      | ``&#x1f4ce;``  | Yes | Paperclip (attachments exist)   |
+-------------+----------------+-----+---------------------------------+
| Email       | ``&#x2709;``   | Yes | An envelope                     |
+-------------+----------------+-----+---------------------------------+
| Pin         | ``&#x1f4cc;``  | Yes | For *sticky* topics             |
+-------------+----------------+-----+---------------------------------+
| **Social-media services**                                            |
+-------------+----------------+-----+---------------------------------+
| Facebook    | ``&#x66;``     | No  | The ``f`` character             | 
+-------------+----------------+-----+---------------------------------+
| Google Plus | ``&#x67;``     | No  | The ``g`` character             |
+-------------+----------------+-----+---------------------------------+
| Twitter     | ``&#x74;``     | No  | The ``t`` character             |
+-------------+----------------+-----+---------------------------------+

Where possible the glyphs are mapped onto standard Unicode code-points,
otherwise they are placed at the start of the private-use area.

`Two patterns from CSS Tricks`_ are used to display the icons:

#.  `Enhance a word`_, and
#.  `Standalone icons`_.

Enhance a word
--------------

Two data attributes can be used to add icons::

  <button data-icon="&#x25c3;">Newer</button>
  <button data-icon-after="&#x25b9;">Older</button>

The first attribute is ``data-icon``. It take the character to display (a
left arrow in the above example) as its argument. That character is
displayed before the text within the element. It is the most common use of
the icon. By using the ``data-icon`` attribute screen-readers do not
"speak" the icon, and older browsers degrade gracefully.

The second example above shows the ``data-icon-after`` attribute. It
displays the icon after the text within the element, and is mostly used for
*Next* buttons.


Standalone icons
----------------

Standalone icons need additional markup so screen-readers can hear "read"
what the icon is, while visual browsers just see the glyph. For example,
the following displays a Web feed icon::

  <a type="application/atom+xml" class="icon-alone" href="/some/feed.atom">
    <span aria-hidden="true" data-icon="&#xe003;"></span>
    <span class="screen-reader-text">Web feed</span>
  </a>

* The outer element is marked up with the ``icon-alone`` class.
* The second element provides the icon, using the same ``data-icon``
  attribute that is used to `enhance a word`_. The ``aria-hidden``
  attribute prevents screen readers from "saying" the icon.
* The third and final element provides the text for the screen-reader. It
  is given the ``screen-reader-text`` class so it is not visible to
  visual-browsers.

Acknowledgements
================

The `Twitter Bootstrap`_ CSS is pasted at the start of the GroupServer file
to eliminate the need for an HTTP request. It is licenced under the `Apache
License, Version 2.0`_.

The Icons_ were taken from two glyph-fonts:

* Entypo_ by Daniel Bruce provided most of the icons. It is licenced under
  the `CC BY-SA 3.0 license`_ (much like this README).
* `Font Awesome`_ by Dave Gandy provided the pin icon. It is licenced under 
  the `CC BY 3.0 license`_.

The `IcoMoon`_ App, by Keyamoon, was used to crate the font-files.

Authors
=======

Josh Campbell did the initial design and implementation (GS 0.9). Ben Ford
from Metasolutions_ did a major redesign (GS 1.0). Mike Harding from
`Cactus Lab`_ re-imagined the design into what is implemented here (GS
2.0). The CSS coding for the most recent two versions, and egg creation,
was by `Michael JasonSmith`_.

Resources
=========

- Code repository: https://source.iopen.net/groupserver/gs.content.css
- Questions and comments to http://groupserver.org/groups/development
- Report bugs at https://redmine.iopen.net/projects/groupserver

.. _GroupServer: http://groupserver.org/
.. _GroupServer.org: http://groupserver.org/
.. _OnlineGroups.Net: https://onlinegroups.net/
.. _Michael JasonSmith: http://groupserver.org/p/mpj17/
.. _Creative Commons Attribution-Share Alike 3.0 New Zealand License:
   http://creativecommons.org/licenses/by-sa/3.0/nz/
.. _Two patterns from CSS Tricks: http://css-tricks.com/html-for-icon-font-usage/
.. _Twitter Bootstrap: http://twitter.github.com/bootstrap/
.. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
.. _Entypo: http://entypo.com/
.. _CC BY-SA 3.0 license: http://creativecommons.org/licenses/by-sa/3.0/
.. _CC BY 3.0 license: http://creativecommons.org/licenses/by/3.0/
.. _Font Awesome: http://fortawesome.github.com/Font-Awesome/
.. _IcoMoon: http://icomoon.io/
..  _Metasolutions: http://metasoltuions.co.nz/
.. _Cactus Lab: http://cactuslab.com/
