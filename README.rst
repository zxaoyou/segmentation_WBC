=============================
WBC Image Dataset
=============================

This is two datasets of white blood cell (WBC) images used for “Fast and Robust Segmentation of White Blood Cell Images by Self-supervised Learning”, which can be used to evaluate cell image segmentation methods. 

These two datasets are significantly different from each other in terms of the image color, cell shape, background, etc., which can better evaluate the robustness of WBC segmentation approach. The ground truth segmentation results are manually sketched by domain experts, where the nuclei, cytoplasms and background including red blood cells are marked in white, gray and black respectively. We also submitted the segmentation results by our approach, where the whole WBC region are marked in white and the others are marked in black.

**Dataset 1** was obtained from `Jiangxi Tecom Science Corporation, China <https://http://en.tecom-cn.com/>`_. It contains three hundred 120×120 images of WBCs and their color depth is 24 bits. The images were taken by a Motic Moticam Pro 252A optical microscope camera with a N800-D motorized auto-focus microscope, and the blood smears were processed with a newly-developed hematology reagent for rapid WBC staining. The overall background of most of the images of Dataset 1 looks yellow.


.. image:: https://raw.githubusercontent.com/zxaoyou/segmentation_WBC/master/Dataset%201.png
   :alt: Images from Dataset 1.
   :align: center

**Dataset 2** consists of one hundred 300×300 color images, which were collected from  `the CellaVision blog <https://http://blog.cellavision.com/>`_. The cell images are generally purple and may contain many red blood cells around the white blood cells.

.. image:: https://raw.githubusercontent.com/zxaoyou/segmentation_WBC/master/Dataset%202.png
   :alt: Images from Dataset 2.
   :align: center

As you use  **Dataset 2**,  please cite  `the CellaVision blog <https://http://blog.cellavision.com/>`_ (http://blog.cellavision.com). 

As you use **Dataset 1** or both datasets, please cite `Jiangxi Tecom Science Corporation, China <https://http://en.tecom-cn.com/>`_.
