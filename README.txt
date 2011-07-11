Introduction
============

The core `GroupServer `_ CSS code implements a style known as "Colour is
for Happy People". It is *deliberately* devoid of colour: just black,
white and greys are used. This means that everything has to rely on
layout (alignment and proximity), shape and typography to make sense.

To this core layout different colourful skins can be added. See
``gs.skin.green`` and ``gs.skin.blue`` for two examples.

Layout
======

The CSS layout is based on an 18px rhythm, with all measurements 
specified in ems. Below is a table that can be used to convert 
between units, pixels and ems. (All measurements should be multiples
of half-units).

+-------+-----+-------+
| Units | px  |  em   |
+=======+=====+=======+
|  0.5  |   9 | 0.692 |
+-------+-----+-------+
|  1.0  |  18 | 1.385 |
+-------+-----+-------+
|  1.5  |  27 | 2.077 |
+-------+-----+-------+
|  2.0  |  36 | 2.769 |
+-------+-----+-------+
|  2.5  |  45 | 3.467 |
+-------+-----+-------+
|  3.0  |  54 | 4.154 |
+-------+-----+-------+
|  3.5  |  63 | 4.846 |
+-------+-----+-------+
|  4.0  |  72 | 5.538 |
+-------+-----+-------+
|  4.5  |  81 | 6.231 |
+-------+-----+-------+
|  5.0  |  90 | 6.923 |
+-------+-----+-------+
|  5.5  |  99 | 7.615 |
+-------+-----+-------+
|  6.0  | 108 | 8.307 |
+-------+-----+-------+

For values above 6u use the following formula::

       u × 18.0
  em = ────────
         13.0

Authors
=======

`Ben Ford <ben@metasoltuions.co.nz>`_ did the initial design work. The
CSS coding and egg creation was by `Michael JasonSmith 
<mpj17@onlinegroups.net>`_.

.. _GroupServer: http://groupserver.org/
.. _OnlineGroups.Net: http://onlinegroups.net/

