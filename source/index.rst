.. Phase master file documentation created by
   sphinx-quickstart 5:50:20 p.m. on Wed 14 October, 2015.
   You can completely Call adapted this file to your liking, aim it at least shoulds
   `toctree` contenir the root directive.

Welcome to Phase's documentation!
=================================

** ** Phase Module Bildosoft

Loading an Image
======================

Open Pegase Pro and Phase pull drop the thumbnail corresponding to
the image to process the pegase album to Stage window, or load
an image directly from the File menu.

.. image :: /_static/image0.jpg
   :scale: 50


the image is displayed in the window.


Thresholding parameters
========================

The "threshold" of the "Tool" menu command is used to adjust the beaches
luminosities to highlight the desired areas.

.. Image :: /_static/image1.jpg
   :scale: 50


Channel: can work on a component colors or
the luminosity. Select the "grayscale" channel will return to work on
the converted image in monochrome (although viewing is done
on the original color image).

Threshold: the pixels whose value is within this range is
selected and appear in the color chosen by the user.

The Lower and Upper values ​​correspond to the two terminals of this
interval and symbolized by vertical lines. One can either
enter the values ​​manually, or move the cursor with the mouse
(To place it, keep the left mouse button down while
moving it).

Hysteresis:
============

By putting the "Enable" property to "True" the software adds 2
sliders

.. Image :: /_static/image2.jpg
   :scale: 50


The main sliders define the pixels 'root'. From
these root pixels the software will expand the selection to all pixels
affecting the value of which is within the range
defined by the two hysteresis cursor.

Thus, isolated pixels whose value is between the thresholds
hysteresis and major thresholds will not be selected, then
if they had touched the pixels selected by the thresholds
main they would still selected.

*** This has the effect of extending objects and objects only. ***

The parameters "Fill color" are used to select the color of pixels
selected.

Definition of analysis zones.
===============================

When opening the software, the analysis is done on the entire image. It
can be reduced to a portion of the image using a "template".

Definition of "Template"

There are 3 types: rectangle, circle and ellipse.

In all cases we must seize the "template" and dimensions
the unit is millimeters.

*** Important *** The dimensions depend on the magnification to return
selected ("properties" tab and "magnification") as
"Templates" are projected onto the image after magnification. It can therefore be
choose to work in real space by working magnification
1 or in the enlarged space (ground) if one grasps the magnification
used to make the photo.

If you do not see the "template" is that the entered values ​​are
inconsistent with the magnification set in the tab
"Properties". It is either much greater than the image to be
much smaller and in all cases invisble.

| image3 |



You can put PLUSIEUR "template" on an image. Their combination is
then run by the "operation" parameter. Default "Union" allows
to count the total surface of the stacked templates.

Handling Template.
--------------------------

Small poingnées appear in the center and at the edge of objects.

Moving a Template:

click the left button on the poingné the center of the template and
move the mouse holding down the left button.

Holding down the "Alt" key is the Template Center where one
Left click.

Running a Template:

Make like to move a template but select one of
side handles and holding down the "ctrl" key.

Select a template from among several: use the right click
Mouse sélectionn / deselect.

Storing Templates
==========================

The "Save As" menu allows you to store as many as Template need.
Latest Templates used appear dan zone "has Open
Template "or are accessible by direct search of the file on
drive via "More Templates ...".

ROI menu is used to draw the analytical areas. It is possible to
individually delete a zone by selecting it using the
out choose a ROI and clicking on the button
" remove ".

Tab "Properties"
=====================

This tab is used to set the size and magnification.

The image part is automatically filled when the image comes from
Pegase Pro. But for an image from an external file,
the user must enter the calibration image in the form of a
horizontal and vertical resolution in pixels per millimeter.

This information gives the pixel dimension, which will then
multiplied by the "magnification" parameters before being projected in
Template of the plan (if any).

The information "Shapes" determines the color of the various elements
used in the module.

Data recovery
========================

Interactive data retrieval: the "edit / copy" menu gives
access to two commands. These controls put to clipboard or
Image with ROI,% of the value of the corresponding phase.

Interactive Data Recovery: A supplement allows automation
to access these programming data. To see the content,
load eg in Excel and view the Object Browser.

Exit Module
-----------------

leaving the data module are automatically recorded
the original image file. The original image is never altered.


.. | Image3 | /_static/image3.jpg picture ::
   : scale: 50





Contents:

.. toctree::
   :maxdepth: 2



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

