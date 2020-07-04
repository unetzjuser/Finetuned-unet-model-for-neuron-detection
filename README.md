# Finetuned U-Net segmentation model for neuron detection
A finetuned model to segment c-fos-immunostained neurons

### This finetuned model is based on an established pre-trained 2D model, which can be downloaded here:
https://lmb.informatik.uni-freiburg.de/resources/opensource/unet/2d_cell_net_v0_model.zip

This finetuned model has been used to detect c-fos-immunostained neurons (both by IHC and IF) in brain slices. It is also possible to apply this model to segment neurons labeled by other markers (e.g., EGFP, RFP). However, for accurate cell detection, manual correction may be needed.

### How to use?
* Download and install Fiji: https://imagej.net/Fiji/Downloads
* Setup the backend (caffe_unet) and the frontend (Fiji with the U-Net plugin). Please follow the installation instructions: https://lmb.informatik.uni-freiburg.de/resources/opensource/unet/#detection
* Download the "2d_cell_net_v4-cfos.modeldef" file and the "2d_cell_net_v4-cfos.caffemodel.zip" file from this repository. Move the .modeldef file and the unzipped .caffemodel file to a folder.
* Open image(s) in Fiji and run the U-Net plugin.
* Note that the scale in the image (if there is any) should be removed before running the U-Net plugin: Fiji--Plugins--Set Scale--Click to Remove Scale. Otherwise the image will be wrongly scaled during segmentation and the results are not optimal.

<p align="center">
   <img src="https://raw.githubusercontent.com/unetzjuser/Finetuned-unet-model-for-neuron-detection/master/Fiji%20screenshot.jpg?raw=true" />

### For further information:
https://github.com/lmb-freiburg/Unet-Segmentation

https://lmb.informatik.uni-freiburg.de/resources/opensource/unet/#detection

### Examples:
* An immunostained section from an adult mouse exposed to environmental enrichment shows c-fos-expressing neurons in the piriform cortex.
<p align="center">
   <img src="https://raw.githubusercontent.com/unetzjuser/Finetuned-unet-model-for-neuron-detection/master/Original_preview.png?raw=true" width="300" height="375" title="Original_preview.png" />

* The original image superimposed with segmented neurons (shown in red).
<p align="center">
   <img src="https://raw.githubusercontent.com/unetzjuser/Finetuned-unet-model-for-neuron-detection/master/Merge_preview.png?raw=true" width="300" height="375" title="Merge_preview.png" />

### Reference:
Thorsten Falk, Dominic Mai, Robert Bensch, Özgün Çiçek, Ahmed Abdulkadir, Yassine Marrakchi, Anton Böhm, J. Deubner, Z. Jäckel, K. Seiwald, A. Dovzhenko, O. Tietz, C. Dal Bosco, S. Walsh, D. Saltukoglu, T. Tay, M. Prinz, K. Palme, M. Simons, I. Diester, Thomas Brox & Olaf Ronneberger. U-Net: deep learning for cell counting, detection, and morphometry. Nature Methods, 16, 67-70, 2019.
