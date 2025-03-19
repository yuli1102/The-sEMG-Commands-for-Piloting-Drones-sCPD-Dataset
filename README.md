## Citation
If you use this repository, please cite the following paper. This paper is submiting to the CACAIE. The citation will be updated later. 

Li, Y., Zhang, D., Dong, P., Yao, S., & Qin, R. (2025). S2CNet: An sEMG-based Deep Learning Model for Guiding Semi-autonomous Drones in Road Infrastructure Inspection. 

~~~~  
@article{li2025S2CNet,
  title={S2CNet: An sEMG-based Deep Learning Model for Guiding Semi-autonomous Drones in Road Infrastructure Inspection},
  author={Li, Yu and Zhang, David and Dong, Penghao and Yao, Shanshan and Qin, Ruwen},
  year={2025},
}
~~~~


# Data
## sCPD
sEMG commands for piloting drones (sCPD) dataset comprises sEMG and audio data of 23 keywords gathered from 11 subjects. The 11 subjects contributed their data to this study, which ages ranged from 19 to 46 years old. Of these participants, four were male, and the remaining seven were female. All subjects spoke English fluently, and four of them were native English speakers. 
In this project, we collected sEMG data and audio data synchronously at a rate of 40000. There were 7 channels for sEMG data, and their locations were attached around the mouth as shown in the figure. Additionally, there were 8 ground electrodes attached to the bones.
<p align="center">
  <img src="https://user-images.githubusercontent.com/44143351/235980630-704e6b55-a051-41ab-b480-e82fb8b82dc6.png" alt="sEMG sensor" width="50%" height="auto">
</p>

Raw data can be downloaded from [here](https://drive.google.com/drive/folders/1ZUkjGaJ490aIn4ibi_ocKNpsL6zRkMee?usp=drive_link), the following image is an example of the collected sEMG and audio data. Instruction of the raw data can be found in "Raw data instruction.md" in this project.

<p align="center">
  <img src="https://user-images.githubusercontent.com/44143351/232256546-72b93a57-b373-4281-ba72-448ac82b309a.png" alt="sEMG sensor" width="50%" height="auto">
</p>

The final converted Scaleogram data can be downloaded from [here](https://drive.google.com/drive/folders/1yvobQDLeBAkvNWtwp86-UeuDjkwbJCGH?usp=drive_link). The following image is an example of final converted Scaleogram.
<p align="center">
  <img src="https://github.com/yuli1102/Robotic-Inspection-Command-Keywords-RICKs-v2.0/assets/44143351/f780ae39-957c-4acc-bada-cf9bd5b857f5" alt="scaleogram" width="50%" height="auto">
</p>

Example code in folder of [Data Processing](./Data_Processing/) shows how we process the raw data to final scaleogra data. 

## NINAPro DB1
We also used a public dataset of NINAPro DB1, which can be found [here](https://ninapro.hevs.ch/instructions/DB1.html). The converted Scaleogram of this dataset can be downloaded [here](https://drive.google.com/drive/folders/1z45hrx9GgVlabqyUZVAuV2KQIsBrjDHw?usp=drive_link).

# Experiment Results
Experiment results analysis code is concluded in the paper, details can be found from "Experiment Results/[Experiments_performance_1213.ipynb](https://github.com/yuli1102/Robotic-Inspection-Command-Keywords-RICKs-v2.0/blob/main/Experiment%20Results/Experiments_performance_1213.ipynb)" in this repository.

# Note
Raw data and data processing code can be downloaded now, but the code for the model will be uploaded after acceptance.
