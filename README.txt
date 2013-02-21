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
