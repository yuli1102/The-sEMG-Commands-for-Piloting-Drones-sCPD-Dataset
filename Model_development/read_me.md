# inference_time_0419.ipynb
This notebook is used to evaluate the inference time after developing the final model. It includes measurements of inference time using the raw .mat data, as well as tests with variations in image scale and downsampling.
The raw .mat dataset used in this code can be downlaoded: [sCPD](https://drive.google.com/drive/folders/1ZUkjGaJ490aIn4ibi_ocKNpsL6zRkMee) and [NinaPro DB1](https://ninapro.hevs.ch/instructions/DB1.html)
The developped model used in this code can be downloaded: [Final models](https://drive.google.com/drive/folders/151cyDhoXvrLAFq7iDqYMWgZjaR_37s9i?usp=drive_link)

# unfreeze_vs_freeze_sCPD_0412.ipynb and unfreeze_vs_freeze_sCPD_tiny_0414.ipynb
These notebooks are used to develop models on the sCPD dataset by comparing the performance of freezing vs. unfreezing the pre-trained model layers.
The converted Scaleogram images can be download [here](https://drive.google.com/drive/folders/1yvobQDLeBAkvNWtwp86-UeuDjkwbJCGH).

# unfreeze_vs_freeze_NinaProDB1_0412.ipynb
This notebook is used to develop models on the NinaPro DB1 dataset, also by comparing freezing and unfreezing strategies on pre-trained model layers.
The converted Scaleogram images can be download [here](https://drive.google.com/drive/folders/1z45hrx9GgVlabqyUZVAuV2KQIsBrjDHw).

# weight_sCPD_0419.ipynb and weight_sCPD_tiny_0421.ipynb
These notebooks evaluate model performance using different values of the weighting factor ηₐ in Equation (12) of the paper.
The converted Scaleogram images can be download [here](https://drive.google.com/drive/folders/1yvobQDLeBAkvNWtwp86-UeuDjkwbJCGH).