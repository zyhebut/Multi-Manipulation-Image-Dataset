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



这个数据集是多篡改数据集,包括的篡改类型有：拼接，复制粘贴和移除.
文件包括:
[编号].jpg  -->  原始图片
[非文件夹编号].jpg  -->  拼接物体源图片
[编号+].png  -->  篡改图片
[编号+].json  -->  篡改区域标注
[编号+mask].png  -->  篡改区域mask
[编号++mask].png  -->  单通道mask
[编号_aux].png  -->  用于辅助标注的图片
[编号_aux].json  -->  remove区域标注（因为remove在篡改图片中不好标注，所以使用辅助信息进行标注）

mask编号：
（0,0,0）->背景
（255,255,255）->拼接 765
（0,125,125）->移除 250
（255,0,255）->复制粘贴 篡改部分  510
（255,0,0）->复制粘贴 源部分 255