..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the main branch.

.. note::

   **This technote is not yet published.**

   The on sky pointing accuracy of the Auxiliary Telescope (AuxTel) is checked in this tech note. The world coordinate system (WCS) solution of the AuxTel images provides a pointing within 0.25 arcesc of the telescope. In this manner, we compare the WCS sky positing with the one reported on the boresight. We derived angular offset of these sky coordinates for images from Feb 2020 up to Mar 2022. And we report an overall pointing accuracy of 57 arcesec. Since the pointing model was edited monthly during most of this time period the pointing offset also changes significantly monthly. In the note you can find the pointing angular offset timeline and distribution, the elevation and azimuth offsets as a function of the elevation and a correlation plot with environmental conditions. 

Pointing Model Verification 2022/03
##########################
    
Iin this tech note, the on sky pointing accuracy of the Auxiliary Telescope (AuxTel) images is checked. 

The notebook of this analysis can be found here: https://github.com/estevesjh/ComScratchStuff/tree/main/AuxTel/pointingTracking

Last Revision: 2022-03-30

..  _Pointing-Model-Verification-202203-Summary:

Summary
============

Here we check the pointing ability of the AuxTel telescope to slew to a given sky coordinate for the night runs from Feb 2020 up to Mar 2022.

The pointing coordinate given by the boresight is compared to the world coordinate system (WCS) solution of the AuxTel images. 

The WCS solutions were taken from the DM Stack Pipeline images that passed the `calibration task`, which provides a pointing accuracy within ~0.25 arcesc. 

Comparing the angular offset of the two sky coordiantes we report an overall pointing precision of 57arcsec. 

The pointing offset changes signficantly with the changes on the pointing model. 

The best pointing model found on this analysis is the one from Oct 2021, [link]. 

The pointing model from Nov 2021 was not updated for the observations runs of Feb and Mar 2202. 

Looking into these months we found an initial offset on the AlAz of (-0.1, 0.5) arcmin on Feb 2022 which involved to be (-0.5, 0.) arcmin in Mar 2022.
 
Finally, we looked for correlations of the pointing offset with the some metadata properties, we didn't find any signficant correlation. 


..  _Pointing-Model-Verification-202203-Data-Acquisition:

Data-Acquisition
============

..  _Pointing-Model-Verification-202203-Pointing-Offset-Timeline:

Pointing-Offset-Timeline
============

..  _Pointing-Model-Verification-202203-Elevation-Offsets:

Elevation-Offsets
============

..  _Pointing-Model-Verification-202203-Correlations:

Correlations
============

.. Add content here.
.. Do not include the document title (it's automatically added from metadata.yaml).

Pointing Model Verification
=======================
The accuracy of the pointing is cross-checked using the World Coordinate Solutions (WCS) for each image processed by the dm stack pipeline. 


.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
