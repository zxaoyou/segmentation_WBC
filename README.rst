=============================
WBC Image Dataset
=============================

This is two datasets of white blood cell (WBC) images used for “**Fast and Robust Segmentation of White Blood Cell Images by Self-supervised Learning**”, which can be used to evaluate cell image segmentation methods. 

These two datasets are significantly different from each other in terms of the image color, cell shape, background, etc., which can better evaluate the robustness of WBC segmentation approach. The ground truth segmentation results are manually sketched by domain experts, where the nuclei, cytoplasms and background including red blood cells are marked in white, gray and black respectively. We also submitted the segmentation results by our approach, where the whole WBC region are marked in white and the others are marked in black.

**Dataset 1** was obtained from `Jiangxi Tecom Science Corporation, China <http://en.tecom-cn.com/>`_. It contains three hundred 120×120 images of WBCs and their color depth is 24 bits. The images were taken by a Motic Moticam Pro 252A optical microscope camera with a N800-D motorized auto-focus microscope, and the blood smears were processed with a newly-developed hematology reagent for rapid WBC staining. The overall background of most of the images of Dataset 1 looks yellow.


.. image:: https://raw.githubusercontent.com/zxaoyou/segmentation_WBC/master/Dataset%201.png
   :alt: Images from Dataset 1.
   :align: center

**Dataset 2** consists of one hundred 300×300 color images, which were collected from `the CellaVision blog <http://blog.cellavision.com/>`_. The cell images are generally purple and may contain many red blood cells around the white blood cells.

.. image:: https://raw.githubusercontent.com/zxaoyou/segmentation_WBC/master/Dataset%202.png
   :alt: Images from Dataset 2.
   :align: center

The class labels of each image in Dataset 1 and Dataset 2 are shown in the files **Class Labels of Dataset 1.csv** and **Class Labels of Dataset 2.csv**. The labels (1- 5) represent neutrophil, lymphocyte, monocyte, eosinophil and basophil, respectively.

If you use **Dataset 1** in your paper, please acknowledge `Jiangxi Tecom Science Corporation, China <http://en.tecom-cn.com/>`_.

If you use **Dataset 2** in your paper, please acknowledge `the CellaVision blog <http://blog.cellavision.com/>`_ (http://blog.cellavision.com/).

If you use **Dataset 1** or **Dataset 2** in your paper, please cite the paper::

    @article{Zheng2018,
      title={Fast and Robust Segmentation of White Blood Cell Images by Self-supervised Learning},
      author={Xin Zheng and Yong Wang and Guoyou Wang and Jianguo Liu},
      journal={Micron},
      volume={107},
      pages={55--71},
      year={2018},
      publisher={Elsevier}
      doi={https://doi.org/10.1016/j.micron.2018.01.010},
      url={https://www.sciencedirect.com/science/article/pii/S0968432817303037}
    }


Warning on the Class Labels
^^^^^^^^
The class labels of some of the WBC images are manually added by the authors themselves, as not every WBC image has a ground-truth label when the authors gained the original images. Since the main focus of this work is WBC segmentation, the authors did not ask domain experts to help double check the class labels. So it is at your own risk if you need to use the class labels of the provided datasets in your research.
