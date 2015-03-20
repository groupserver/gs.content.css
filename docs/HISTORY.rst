Changelog
=========

2.6.1 (2015-03-20)
------------------

* Improving the rendering of posts on small screens, with thanks
  to Piers_
* Truncating the name of the author on the Image page when it is
  wider than the containing box.

.. _Piers: http://groupserver.org/r/post/7hAninwloIp51mDkbk183F

2.6.0 (2015-03-10)
------------------

* Adding the CSS for the *Verify* page
* Adding the CSS for the *Verify wait* page

2.5.0 (2015-03-03)
------------------

* Stopping the scroll-bar from appearing in the header of the
  *Post* page
* Moving the *Group email settings* button to the right of the
  *Member information* box on the Group page
* Naming all the reStructuredText files as such
* Pointing at GitHub_ as the primary repository

.. _GitHub: https://github.com/groupserver/gs.content.css

2.4.2 (2014-06-24)
------------------

* Removing the margin form the ul at the bottom of the
  `gs.group.member.active`_ viewlet

.. _gs.group.member.active:
   https://github.com/groupserver/gs.group.member.active

2.4.1 (2014-05-15)
------------------

* Fixing some CSS errors

2.4.2 (2014-03-05)
------------------

* Fixing the clipping of the filename on the *Image* page
* Fixing the profile images in *Reply to topic* and *Start a new
  topic*, closing `Bug 4082`_

.. _Bug 4082: https://redmine.iopen.net/issues/4082

2.4.1 (2014-02-17)
------------------

* Fixing the URL to the EOT version of the icon-font

2.4.0 (2014-01-27)
------------------

* Adding support for the *Invite by CSV* page
* Fixing some clipping in posts

2.3.1 (2013-11-27)
------------------

* Fixing Chrome and Safari so they animate the loading icon

2.3.0 (2013-11-26)
------------------

* Turning the editor back on for *content editor* pages
* Added the animated swirl icon
* Added new glyph icons: 

  + Install
  + Archive
  + Linux
  + GroupServer
  + Devices (mobile, tablet, laptop, desktop)
  + Text editing

* Dealing with corner-cases with search, closing `Feature 4038`_
* Fixing the Group page for an *announcement* group
* Removing the bitmap icons from the Bootstrap code

.. _Feature 4038: https://redmine.iopen.net/issues/4038

2.2.3 (2013-11-05)
------------------

* Adding a *minified* version of the CSS

2.2.1 (2013-10-15)
------------------

* Adding a new break-point at 460px

2.2.0 (2013-09-24)
------------------

* Turning a menu into an inline list on small screens, closing
  `Feature 3909`_
* Hiding the breadcrumbs on pages with a context-menu

.. _Feature 3909: https://redmine.iopen.net/issues/3909

2.1.0 (2013-09-11)
------------------

* Adding support for the *Members* page, closing `Feature 3862`_
* Fixing some boxes when they overflow
* Adding a ``print`` style
* Making the header-links generic

.. _Feature 3862: https://redmine.iopen.net/issues/3862

2.0.2 (2013-07-24)
------------------

* Removing a hack from the *About* box on the Group page

2.0.1 (2013-07-08)
------------------

* Fixing a gap on the *Topics* list of the Group page

2.0.0 (2013-06-07)
------------------

* Updating to the new GroupServer user interface

  + Implementing a *flat* design aesthetic, designed by Mike
    Harding from `Cactus Lab`_
  + Switching to `Twitter Bootstrap 2`_ for the core CSS
  + Adding icon-fonts

.. _Cactus Lab: http://cactuslab.com/
.. _Twitter Bootstrap 2: http://getbootstrap.com/2.3.2


1.4.1 (2012-06-13)
------------------

* Fixing the sticky-topic icons

1.4.0 (2012-06-06)
------------------

* Adding support the *One true search* system (see
  `gs.search.base`_)

.. _gs.search.base: https://github.com/groupserver/gs.search.base

1.3.0 (2012-05-30)
------------------

* Adding support for the *Encouragement* for a group
  administrator
* Refactoring the *About* tab on the group page

1.2.0 (2012-05-16)
------------------

* Adding the support for the *Topics* tab, the *Posts* tab, and
  the *Files* tab on the Group page

1.1.1 (2011-12-05)
------------------

* Adding the style for the ``<cite>`` element back
* Tweaking the style for nested lists

1.1.0 (2011-07-26)
------------------

* Adding the CSS for sign-up methods

1.0.0 (2011-07-14)
------------------

Initial commit. Prior to the creating of this product the CSS was
provided as a *file-system site* component by the
`Products.GroupServer`_ product.

.. _Products.GroupServer:
   https://github.com/groupserver/Products.GroupServer

..  LocalWords:  CSS Changelog Refactoring minified reStructuredText GitHub
