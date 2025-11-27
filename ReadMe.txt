Multi-Manipulation Image Dataset (MMID) 

The Multi-Manipulation Image Dataset (MMID) is a collection of 2,000 images, each containing at least two types of image manipulations. These manipulations include splicing, copy-move, and removal. The original images are sourced from the COCO dataset and have been manually altered using Adobe Photoshop.
The process for each manipulation type is as follows:
•	Splicing: Two images with similar scenes are selected from COCO. An object is carefully chosen from one image, then rotated, scaled, and transplanted into the target image. Post-processing techniques such as brightness/contrast adjustment and color balancing are applied to enhance the visual coherence of the composite.
•	Copy-Move: An object within a single image is duplicated, then transformed and blended into another location within the same image.
•	Removal: Selected objects are removed from an image using tools such as the Clone Stamp and Healing Brush.

Any publication that uses the MMID must cite the following reference:
@ARTICLE{ALLINONE,
  author={Zhu, Ye and Ti, Chang and Yan, Gang and Guo, Yingchun and Li, Bin},
  journal={IEEE Transactions on Circuits and Systems for Video Technology}, 
  title={ALL-IN-ONE: Divide-and-Conquer Strategy for Multi-Manipulation Image Classification and Localization}, 
  year={2025},
  pages={1-13},
  doi={10.1109/TCSVT.2025.3603579}}


This dataset is the Multi-Manipulation Image Dataset （MMID), which Includes multiple tampered types,e.g. splicing, copy-move, and removal.
The files include:
[Number].jpg --> Original image
[Non-folder number].jpg --> Source image for spliced object
[Number+].png --> Tampered image
[Number+].json --> Tampered region annotations
[Number+mask].png --> Tampered region mask
[Number++mask].png --> Single-channel mask
[Number_aux].png --> Auxiliary image for annotation
[Number_aux].json --> Removal region annotations (Since removal regions are difficult to annotate directly in the tampered image, auxiliary information is used for annotation)

Mask numbering:
(0,0,0) -> Background
(255,255,255) -> Splicing 765
(0,125,125) -> Removal 250
(255,0,255) -> Copy-move tampered region 510
(255,0,0) -> Copy-move source region 255
