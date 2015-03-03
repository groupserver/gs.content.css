Icons
=====

An glyph-font is supplied by this product to provide the icons
that are used in the interfaces, as `detailed below`_. `Two
patterns from CSS Tricks`_ are used to display the icons:

#.  `Enhance a word`_, and
#.  `Standalone icons`_.

The latter is used to display the Loading_ animation.

.. _detailed below:

Icon details
------------

Below are the details of the 22 icons provided by
:mod:`gs.content.css`. Where possible the glyphs are mapped onto
standard Unicode code points, with the XML character entity given
in the *Character* column. Using Unicode code-points allows them
to look *vaguely* right when typefaces other than the glyph-font
are being used. The non-standard icons are placed at the start of
the private-use area.

+-------------+----------------+-----+---------------------------------+
|    Icon     |    Character   |Std? | Note                            |
+=============+================+=====+=================================+
| **Breadcrumb trail**                                                 |
+-------------+----------------+-----+---------------------------------+
| Home        | ``&#x2302;``   | Yes | A house                         |
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
| Install     | ``&#xe002;``   | No  | Arrow pointing to a disk druve  |
+-------------+----------------+-----+---------------------------------+
| **True icons**                                                       |
+-------------+----------------+-----+---------------------------------+
| Picture     | ``&#x1f3a8;``  | Yes | Replaces "artist palette"       |
+-------------+----------------+-----+---------------------------------+
| Movie       | ``&#x1f3a6;``  | Yes | Replaces "movie projector"      |
+-------------+----------------+-----+---------------------------------+
| Sound       | ``&#x1f509;``  | Yes | Speaker                         |
+-------------+----------------+-----+---------------------------------+
| Documents   | ``&#x1f5cd;``  | Yes | Replaces "empty pages"          |
+-------------+----------------+-----+---------------------------------+
| Archive     | ``&#xe004;``   | No  | For zip and tar files           |
+-------------+----------------+-----+---------------------------------+
| Attach      | ``&#x1f4ce;``  | Yes | Paperclip (attachments exist)   |
+-------------+----------------+-----+---------------------------------+
| Email       | ``&#x2709;``   | Yes | An envelope                     |
+-------------+----------------+-----+---------------------------------+
| Pin         | ``&#x1f4cc;``  | Yes | For *sticky* topics             |
+-------------+----------------+-----+---------------------------------+
| Linux       | ``&#xe017;``   | No  | Tux, for <groupserver.org>      |
+-------------+----------------+-----+---------------------------------+
| Groupserver | ``&#xe018;``   | No  | "GS", for <groupserver.org>     |
+-------------+----------------+-----+---------------------------------+
| **Social-media services**                                            |
+-------------+----------------+-----+---------------------------------+
| Facebook    | ``&#x66;``     | No  | The ``f`` character             | 
+-------------+----------------+-----+---------------------------------+
| Google Plus | ``&#x67;``     | No  | The ``g`` character             |
+-------------+----------------+-----+---------------------------------+
| Twitter     | ``&#x74;``     | No  | The ``t`` character             |
+-------------+----------------+-----+---------------------------------+
| **Devices**                                                          |
+-------------+----------------+-----+---------------------------------+
| Mobile      | ``&#x013;``    | No  | A cell-phone                    |
+-------------+----------------+-----+---------------------------------+
| Tablet      | ``&#x014``     | No  |                                 |
+-------------+----------------+-----+---------------------------------+
| Laptop      | ``&#x015``     | No  |                                 |
+-------------+----------------+-----+---------------------------------+
| Desktop     | ``&#x016``     | No  | A monitor, or screen            |
+-------------+----------------+-----+---------------------------------+
| **Text editing**                                                     |
+-------------+----------------+-----+---------------------------------+
| Bold        | ``&#xe005;``   | No  | A bold **B**                    |
+-------------+----------------+-----+---------------------------------+
| Italic      | ``&#xe006;``   | No  | A italic *I*                    |
+-------------+----------------+-----+---------------------------------+
| Superscript | ``&#xe007;``   | No  | ``x²``                          |
+-------------+----------------+-----+---------------------------------+
| Subscript   | ``&#xe008;``   | No  | ``x₂``                          |
+-------------+----------------+-----+---------------------------------+
| Unlink      | ``&#xe009;``   | No  | A broken chain                  |
+-------------+----------------+-----+---------------------------------+
| Link        | ``&#xe00a;``   | No  | A chain                         |
+-------------+----------------+-----+---------------------------------+
| ``ul``      | ``&#xe00b;``   | No  | Unordered list icon             |
+-------------+----------------+-----+---------------------------------+
| ``ol``      | ``&#xe00c;``   | No  | Ordered list icon               |
+-------------+----------------+-----+---------------------------------+
| Indent      | ``&#xe00d;``   | No  | Indent list left                |
+-------------+----------------+-----+---------------------------------+
| Outdent     | ``&#xe00e;``   | No  | Indent list right               |
+-------------+----------------+-----+---------------------------------+
| Code        | ``&#xe00f;``   | No  | ``</>``                         |
+-------------+----------------+-----+---------------------------------+
| Table       | ``&#xe010;``   | No  |                                 |
+-------------+----------------+-----+---------------------------------+
| Paste       | ``&#xe011;``   | No  | A page and clipboard            |
+-------------+----------------+-----+---------------------------------+
| Undo        | ``&#x238c;``   | Yes |                                 |
+-------------+----------------+-----+---------------------------------+
| Redo        | ``&#x012;``    | No  |                                 |
+-------------+----------------+-----+---------------------------------+
| **Activity**                                                         |
+-------------+----------------+-----+---------------------------------+
| spinner     | ``&#xe619;``   | No  | Animated (see Loading_ below)   |
+-------------+----------------+-----+---------------------------------+

Enhance a word
--------------

Two data attributes can be used to add icons in order to enhance
a word.

.. code-block:: xml

  <button data-icon="&#x25c3;">Newer</button>
  <button data-icon-after="&#x25b9;">Older</button>

The first attribute is ``data-icon``. It take the character to
display (a left arrow in the above example) as its argument. That
character is displayed before the text within the element. By
using the ``data-icon`` attribute screen-readers do not "speak"
the icon, and older browsers degrade gracefully.

The second example above shows the ``data-icon-after``
attribute. It displays the icon after the text within the
element; it is mostly used for *Next* buttons.


Standalone icons
----------------

Standalone icons need additional markup so screen-readers can
"read" what the icon is, while visual browsers see the glyph. For
example, the following displays a Web feed icon:

.. code-block:: xml

  <a type="application/atom+xml" class="icon-alone" href="/some/feed.atom">
    <span aria-hidden="true" data-icon="&#xe003;"></span>
    <span class="screen-reader-text">Web feed</span>
  </a>

* The outer element is marked up with the ``icon-alone`` class.
* The second element provides the icon, using the same
  ``data-icon`` attribute that is used to `enhance a word`_. The
  ``aria-hidden`` attribute prevents screen readers from "saying"
  the icon.
* The third and final element provides the text for the
  screen-reader. It is given the ``screen-reader-text`` class so
  it is hidden to visual browsers.

Loading
-------

When loading data using AJAX it is desirable to show that
activity is taking place in the background. To do this the
Loading icon-character is provided with some CSS3 to animate the
icon so it spins. To create a Loading icon add a standalone icon
with the ``loading`` class:

.. code-block:: xml

  <span data-icon="&#xe619;" aria-hidden="true" 
        class="loading"> </span>

:Note: The space in the ``<span> </span>`` is important. Markup
       processors (such as TAL) can turn XHTML self-closed
       elements (``<span/>``) into unclosed elements. The side
       effect is the entire paragraph is spun.

.. _Two patterns from CSS Tricks:
   http://css-tricks.com/html-for-icon-font-usage/
