# HUSTbearing dataset (实验室自采开源数据集，包含稳定转速和时变转速)

**important updata 2024-05-19. The second column of the file represents speed. However, since we collected the data at a constant speed, this column is redundant and holds no meaningful value. You can ignore it. The correct speed is indicated in the filename.**

We released an open-source bearing failure dataset. 

We hope this dataset can benefit your research

data of quark disk: https://pan.quark.cn/s/0c7578963014  

data of Google Drive: https://drive.google.com/drive/folders/1UMOvyfstYJRyR0rPw0OfH-tIjJg2_0aN?usp=sharing

## Dataset overview


This dataset comprises vibration signals from bearings in **9** different health states under **11** distinct operating conditions. These datasets are publicly available, and anyone can use them to validate diagnosis algorithms for rolling element bearings. Publications making use of the HUSTbearing datasets are requested to cite the following paper.

**Chao Zhao, Enrico Zio, Weiming Shen, Domain Generalization for Cross-Domain Fault Diagnosis: an Application-oriented Perspective and a Benchmark Study, Reliability Engineering and System Safety (2024), doi: https://doi.org/10.1016/j.ress.2024.109964.**



![image](https://github.com/CHAOZHAO-1/HUSTbearing-dataset/blob/main/IMG/F1.png)

Fig. 1. (a) Test rig of HUSTbearing dataset.

## Brief introduction to experiments

###	Bearing testbed
The bearing fault tests were conducted using a Spectra-Quest Mechanical Fault Simulator, as depicted in Fig. 1. From left to right on the test rig are speed control, motor, shaft, acceleration sensor, bearing, and data acquisition board. 
The bearings in nine health states are illustrated in Fig. 2, representing

(1) normal,   
(2) medium inner race fault,  
(3) severe inner race fault,  
(4) medium outer race fault,   
(5) severe outer race fault,  
(6) medium ball fault,  
(7) severe ball fault,  
(8) medium combination fault, and  
(9) severe combination fault.   

It's important to note that combination fault denotes a fault in both the inner race and outer race. All faults are artificially preset.

| Fault size       	| severe 	| medium  	|
|------------------	|--------	|---------	|
| Inner/outer race 	| 0.3 mm 	| 0.15 mm 	|
| Ball             	| 0.5 mm 	| 0.25 mm 	|


![image](https://github.com/CHAOZHAO-1/HUSTbearing-dataset/blob/main/IMG/F2.png)
 
Fig. 2. Photographs of the failure bearings.

### Tested bearing

The type of tested bearings is ER-16K, and the detailed parameters are given in Table 1.

Table 1. Parameters of the tested bearings

 Parameter 	| Value 	| 
|-------	|------	|
| Shaft Diameter     	| 38.52 mm 	| 
| Ball Diameter    	| 7.94 mm 	|
| Number of Balls     	| 9 	|


### Operating Condition

A total of 4 different operating conditions were set in experiments. The operating conditions include:
1) 20 Hz  
2) 25 Hz  
3) 30 Hz  
4) 35 Hz  
5) 40 Hz  
6) 60 Hz  
7) 65 Hz  
8) 70 Hz  
9) 75 Hz  
10) 80 Hz  
11) 0-40-0 Hz,

![image](https://github.com/CHAOZHAO-1/HUSTbearing-dataset/blob/main/IMG/F3.png)
 
Fig. 3. Time-varying speed.

### Sampling setting
   
The sampling frequency is set to 25.6 kHz. A total of 262144 data points (i.e. 10.2s) are recorded for each sampling.
 
## Dataset details

The raw data file comprises 99 files (9 health states multiplied by 11 working conditions), each in Excel format.

For instance, the filename "0.5X_B_65Hz" indicates a medium ball fault under the 65 Hz working condition, where 0.5X denotes medium damage.

The health states are represented by the following codes:

H: healthy

I: inner race fault

O: outer race fault

B: ball fault

C: combination fault

For example, "O_80Hz" signifies a severe outer race fault under the 80 Hz working condition.



<img src="https://github.com/CHAOZHAO-1/HUSTbearing-dataset/blob/main/IMG/F4.jpg" style="transform: rotate(90deg);" width="600" height="800"/>

 
Fig. 4. Drive motor information.


## Contact
If you have any questions or suggestions, do not hesitate to contact:  

Mr. Chao Zhao, zhaochao0612@gmail.com
