# Finetuned U-Net segmentation model for neuron detection
A finetuned model to segment c-fos-immunostained neurons

### This finetuned model is based on an established pre-trained 2D model, which can be downloaded here:
https://lmb.informatik.uni-freiburg.de/resources/opensource/unet/2d_cell_net_v0_model.zip

### For details, please read the original publication by Thorsten Falk and colleagues:
Thorsten Falk, Dominic Mai, Robert Bensch, Özgün Çiçek, Ahmed Abdulkadir, Yassine Marrakchi, Anton Böhm, J. Deubner, Z. Jäckel, K. Seiwald, A. Dovzhenko, O. Tietz, C. Dal Bosco, S. Walsh, D. Saltukoglu, T. Tay, M. Prinz, K. Palme, M. Simons, I. Diester, Thomas Brox & Olaf Ronneberger. U-Net – Deep Learning for Cell Counting, Detection, and Morphometry. Nature Methods, 16, 67-70, 2019

### For further information:
https://github.com/lmb-freiburg/Unet-Segmentation

https://lmb.informatik.uni-freiburg.de/resources/opensource/unet/#detection


### This finetuned model has been used to detect c-fos-immunostained neurons (both by IHC and IF) in brain slices. It is also possible to segment neurons labeled by other markers (e.g., EGFP). However, for accurate detection of neurons, manual correction is needed.

### Examples:
An immunostained brain section showing c-fos-positive neurons in the piriform cortex from a mouse exposed to environmental enrichment.
<p align="center">
   <img src="https://github.com/Finetuned-unet-model-for-neuron-detection/raw/master/Original_preview.png" width="300" height="375">
   Original_preview.png

The original image superimposed with segmented neurons (shown in red).
<p align="center">
   <img src="https://github.com/Finetuned-unet-model-for-neuron-detection/raw/master/Merge_preview.png" width="300" height="375">
   Merge_preview.png
