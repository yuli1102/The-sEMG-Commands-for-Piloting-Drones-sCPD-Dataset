# Raw data

Folder “sEMG_lab1208” uploaded in Releases include all raw data from 11 subjects. In each Subject folder, there are two different types of files: “.adicht” and “.mat”.
![image](https://user-images.githubusercontent.com/44143351/232256491-9692cde8-e95c-462a-b7cd-7f6eef12a539.png)

##	“.adicht”  data
“.adicht” files can be opened with LabChart software, the interface of the software looks like this figure:
![image](https://user-images.githubusercontent.com/44143351/232256546-72b93a57-b373-4281-ba72-448ac82b309a.png)

Channel 1-7 were used to collect sEMG data, and Channel 8 was used to collect audio data.

##	“.mat”  data
Don’t worry if you don’t have LabChart software, because we have already converted all data from “.adicht” to “.mat”, so we can just use “mat” files. In “mat” file, “data” includes all data from 8 channels. There are 8 values in “dataend” and “datastart”. These 8 start and end values are indexes used to split channel data from the “data” file. For example, open the “Backward.mat“ from subject 2, variable “data” is a vector with 1*60112000 data shape, and the values of “datastart” and “dataend” are like this figure:
![image](https://user-images.githubusercontent.com/44143351/232256499-7f52fee3-934c-43b9-b1e5-986149e3873d.png)
 
It means data(1:7514000) are sEMG data from channel 1, and data(7514001:15028000) are channel 2 data. So on so forth, in the end, data(52598001:60112000) means the channel 8 data, which means the audio data. 
If the mat file includes two columns of start and end value, that means the recording was paused and continued. For example,  open the “Birds.mat“ from subject 2, variable “data” is a vector with 1*53184000 data shape, and the values of “datastart” and “dataend” are like this figure:
![image](https://user-images.githubusercontent.com/44143351/232256502-c3810450-7a56-4c2b-9abb-8ae8aa13873b.png)
 
In this case, indexes from 1 to 12736000 are the data before pausing, and 12736001 to 53184000 are the data after pausing. It means data(1:1592000) and data(12736001: 17792000)  are sEMG data from channel 1. Same, data(11144001:12736000) and data(48128001:53184000)  means the audio data. 

Note: Most recordings were not paused, which means most mat files only have one column and 8 start/end indexes. 
