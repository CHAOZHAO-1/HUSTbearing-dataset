![GitHub visitors](https://visitor-badge.laobi.icu/badge?page_id=CHAOZHAO-1.HUSTbearing-dataset&color=blue&style=flat-square)

# HUSTbearing dataset (实验室自采开源数据集，包含稳定转速和时变转速)

**Update (2026-10-29):**

1.Files at different speeds under the same fault state were all collected from the same bearing.  
2.The frequency indicated in the file name is the motor’s set frequency.  
3.The moderate and severe damage were machined on separate bearings.  
4.Each file corresponds to one independent acquisition.  
5.X, Y, and Z in the data denote vibration directions. For their exact definitions, please refer to the test rig photo and the sensor description figure.  


**Important Note. The second column of the file represents speed. However, since we collected the data at a constant speed, this column is redundant and holds no meaningful value. You can ignore it. The correct speed is indicated in the filename.**

We released an open-source bearing failure dataset and hope this dataset can benefit your research

Data of quark disk: https://pan.quark.cn/s/0c7578963014  

Data of Google Drive: https://drive.google.com/drive/folders/1UMOvyfstYJRyR0rPw0OfH-tIjJg2_0aN?usp=sharing

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**更新（2026-10-29）：**
1.同一故障状态下，不同转速的文件均采自同一只轴承。  
2.文件名中标注的频率为电机设定频率。  
3.中度损伤与严重损伤分别加工在不同的轴承上。  
4.每个文件对应一次独立采集。  
5.数据中的 X、Y、Z 为振动方向，具体定义请参见试验台图片及传感器介绍图。  

**重要注释:**
文件中的第二列表示转速。然而，由于振动信号是在恒定转速条件下的，该列是冗余的，没有实际意义，可以忽略。实际的转速信息请以文件名为准。

我们发布了一个开源的轴承故障数据集，希望该数据集能够对您的研究有所帮助。


夸克网盘数据下载：
[https://pan.quark.cn/s/0c7578963014](https://pan.quark.cn/s/0c7578963014)

Google Drive 数据下载：
[https://drive.google.com/drive/folders/1UMOvyfstYJRyR0rPw0OfH-tIjJg2_0aN?usp=sharing](https://drive.google.com/drive/folders/1UMOvyfstYJRyR0rPw0OfH-tIjJg2_0aN?usp=sharing)


## Dataset overview （数据集概述）


This dataset comprises vibration signals from bearings in **9** different health states under **11** distinct operating conditions. These datasets are publicly available, and anyone can use them to validate diagnosis algorithms for rolling element bearings. Publications making use of the HUSTbearing datasets are requested to cite the following paper.

**Chao Zhao, Enrico Zio, Weiming Shen, Domain Generalization for Cross-Domain Fault Diagnosis: an Application-oriented Perspective and a Benchmark Study, Reliability Engineering and System Safety (2024), doi: https://doi.org/10.1016/j.ress.2024.109964.**

---------------------------------------------------------------

该数据集包含在 **11** 种不同工况下、**9** 种不同健康状态的轴承振动信号。这些数据集是公开可获取的，任何人都可以使用它们来验证滚动轴承故障诊断算法。凡是使用 HUSTbearing 数据集发表的研究成果，请引用以下论文：

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
 
Fig. 3. Time-varying speed. （时变转速示意图）

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



<img src="https://github.com/CHAOZHAO-1/HUSTbearing-dataset/blob/main/IMG/F4.jpg" style="transform: rotate(-180deg);" width="600" height="800"/>

 
Fig. 4. Drive motor information (驱动电机信息).


## Contact
If you have any questions or suggestions, do not hesitate to contact:  

Mr. Chao Zhao, zhaochao0612@gmail.com
