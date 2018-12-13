# README #

This repository contains details about the CropCUHK03[1]  dataset.

To manually the CropCUHK03[1]  dataset, download and unzip the following file:

[CropCUHK03](https://imperialcollegelondon.box.com/s/ul13qrju3xfkgkp3baq058ko2d0qxaqi)

## Dataset Description

CropCUHK03[1] is our proposed synthetic dataset with partial crops from CUHK03 of different size and overlap between views.

Originally the dataset contains 14,097 frames of 1467 pedestrians, taken with 2 different camera views and collected at CUHK campus. 
Several settings are generated maintaining the same number of individuals and frames as in CUHK03, which we refer to as:
<a href="" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\small&space;CropCUHK03_{(s,o)}:s\in\{0.25,0.5\}&space;\land&space;o_{\min}&space;\in\{0.0,0.5\}" title="" /></a>
where s is  the fraction of the area cropped from CUHK03 labeled frames i.e. the maximum possible overlap between camera views, and o is the minimum overlap. 
Note that two crops from different views do not need to fully overlap. The crops are generated from random locations by keeping the aspect ratio the same as the original frame and making sure that the overlap between crops is at least o. This typically corresponds to less overlap between cropped parts as they come from different views.

### References

[1] Partial Person Re-identification with Alignment and Hallucination, Sara Iodice and Krystian Mikolajczyk

@InProceedings{iodice2018partial,
  title={Partial Person Re-identification with Alignment and Hallucination},
  author={Iodice, Sara and Mikolajczyk, Krystian},
  booktitle={Asian Conference on Computer Vision},
  year={2018}
}

s.iodice16@imperial.ac.uk
