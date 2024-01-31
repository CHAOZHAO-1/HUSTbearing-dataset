# HUSTbearing dataset (实验室自采开源数据集)

We release a open-source bearing fauliure dataset. We hople this dataset can benifit your research.

data link: https://pan.quark.cn/s/0c7578963014

## Dataset overview


This dataset comprises vibration signals from bearings in nine different health states under four distinct operating conditions. These datasets are publicly available, and anyone can use them to validate diagnosis algorithms for rolling element bearings. Publications making use of the HUSTbearing datasets are requested to cite the following paper.

Chao Zhao, Enrico Zio, Weiming Shen, Domain Generalization for Cross-Domain Fault Diagnosis: an Application-oriented Perspective and a Benchmark Study, Reliability Engineering and System Safety (2024), doi: https://doi.org/10.1016/j.ress.2024.109964.

 
Fig. 1. (a) Test rig of HUSTbearing dataset.

## Brief introduction to experiments

2.1	Bearing testbed
The bearing fault tests were conducted using a Spectra-Quest Mechanical Fault Simulator, as depicted in Fig. 1. From left to right on the test rig are speed control, motor, shaft, acceleration sensor, bearing, and data acquisition board. 
The bearings in nine health states are illustrated in Fig. 2, representing (1) normal, (2) medium inner race fault, (3) severe inner race fault, (4) medium outer race fault, (5) severe outer race fault, (6) medium ball fault, (7) severe ball fault, (8) medium combination fault, and (9) severe combination fault. 
It's important to note that combination fault denotes a fault in both the inner race and outer race. All faults are artificially preset.

 
Fig. 2. Photographs of the failure bearings.

2.2	Tested bearing

The type of tested bearings is ER-16K, and the detailed parameters are given in Table 1.

Table 1. Parameters of the tested bearings
Parameter	Value
Shaft Diameter	38.52 mm
Ball Diameter	7.94 mm
Number of Balls	9

2.3	Operating Condition

A total of 4 different operating conditions were set in experiments. The operating conditions include:
1) 65 Hz
2) 70 Hz
3) 75 Hz
4) 80 Hz
2.4	Sampling setting
   
The sampling frequency is set to 25.6 kHz. As shown in Fig. 3, a total of 262144 data points (i.e. 10.2s) are recorded for each sampling.
 
Fig. 3 Illustration of file
## Dataset details
The raw data file comprises 36 files (9 health states multiplied by 4 working conditions), each in Excel format.
For instance, the filename "0.5X_B_65Hz" indicates a medium ball fault under the 65 Hz working condition, where 0.5X denotes medium damage.
The health states are represented by the following codes:
H: healthy
I: inner race fault
O: outer race fault
B: ball fault
C: combination fault
For example, "O_80Hz" signifies a severe ball fault under the 80 Hz working condition.
## Contact
If you have any questions or suggestions, do not hesitate to contact:  
Mr. Chao Zhao, zhaochao734@hust.edu.cn
