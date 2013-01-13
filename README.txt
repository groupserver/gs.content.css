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

The CSS layout is based on an 18px rhythm, with all measurements specified
in ems. Below is a table that can be used to convert between units, pixels
and ems. (All measurements should be multiples of half-units).

+-------+-----+-------+-----------------------------------------+
|       |     |       | Without Border Width (in em)            |
+-------+-----+-------+------------+--------------+-------------+
| Units |  px |   em  | Thin (1px) | Medium (3px) | Thick (6px) |
+=======+=====+=======+============+==============+=============+
|  0.5  |   9 | 0.692 |      0.615 |        0.462 |       0.231 |
+-------+-----+-------+------------+--------------+-------------+
|  1.0  |  18 | 1.385 |      1.308 |        1.154 |       0.923 | 
+-------+-----+-------+------------+--------------+-------------+
|  1.5  |  27 | 2.077 |      2.000 |        1.846 |       1.615 | 
+-------+-----+-------+------------+--------------+-------------+
|  2.0  |  36 | 2.769 |      2.692 |        2.538 |       2.308 | 
+-------+-----+-------+------------+--------------+-------------+
|  2.5  |  45 | 3.467 |      3.385 |        3.231 |       3.000 | 
+-------+-----+-------+------------+--------------+-------------+
|  3.0  |  54 | 4.154 |      4.077 |        3.923 |       3.692 |
+-------+-----+-------+------------+--------------+-------------+
|  3.5  |  63 | 4.846 |      4.769 |        4.615 |       4.385 |
+-------+-----+-------+------------+--------------+-------------+
|  4.0  |  72 | 5.538 |      5.462 |        5.308 |       5.077 |
+-------+-----+-------+------------+--------------+-------------+
|  4.5  |  81 | 6.231 |      6.154 |        6.000 |       5.769 | 
+-------+-----+-------+------------+--------------+-------------+
|  5.0  |  90 | 6.923 |      6.846 |        6.692 |       6.462 |
+-------+-----+-------+------------+--------------+-------------+
|  5.5  |  99 | 7.615 |      7.538 |        7.385 |       7.154 |
+-------+-----+-------+------------+--------------+-------------+
|  6.0  | 108 | 8.307 |      8.231 |        8.077 |       7.846 |
+-------+-----+-------+------------+--------------+-------------+

For values above 6u use the following formula::

       u × 18.0
  em = ────────
         13.0

The only complication are borders. They can throw out the rhythm, so must
be taken off the margin or padding. The last three columns in the above
table have the border widths taken out. For values above 6u take away one
of the following three values:

+--------+-----+-------+
| Size   | px  |  em   | 
+========+=====+=======+
| Thin   |   1 | 0.077 |
+--------+-----+-------+
| Medium |   3 | 0.231 |
+--------+-----+-------+
| Thick  |   6 | 0.462 |
+--------+-----+-------+


Authors
=======

`Ben Ford <ben@metasoltuions.co.nz>`_ did the initial design work. The
CSS coding and egg creation was by `Michael JasonSmith 
<mpj17@onlinegroups.net>`_.

Resources
=========

- Code repository: https://source.iopen.net/groupserver/gs.content.css
- Questions and comments to http://groupserver.org/groups/development
- Report bugs at https://redmine.iopen.net/projects/groupserver

.. _GroupServer: http://groupserver.org/
.. _OnlineGroups.Net: http://onlinegroups.net/
