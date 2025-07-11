# High-Speed ADC Signal Restoration via Temporal Distortion Learning

<center>Yan Liu, Xiang Gao, Mengyao Yan, Mingyu Hao, and Haiyong Zheng</center>
  
![](https://github.com/OUCIClab/ADC-Res/blob/main/tcn.png "The overall framework of temporal distortion learning for high-speed ADC signal restoration.")
## Abstract
High-speed analog-to-digital converters (ADCs) are
crucial for modern signal processing systems, but they often
suffer from signal distortions due to the use of nonlinear devices
in internal circuits and external interference. Previous studies
typically addressed these distortions separately, neglecting their
actual overlapping and interrelated effects. In this letter, we
delve into and compensate for ADC signal distortions from a
data cascade perspective, aiming to achieve comprehensive signal
restoration. Specifically, we first conduct an integrated analysis
of ADC signal distortions considering static and dynamic aspects.
Furthermore, we proposed a temporal distortion learning framework that incorporates co-designed extraction and fitting components to learn multi-scale distortions and restore ADC signals.
Notably, we designed an FPGA-based accelerator architecture for
the proposed neural network model, enabling real-time signal
restoration of the pipelined ADC. Measurements on a silicon-proven 12-bit 750 MS/s pipelined ADC and a silicon-proven
3000 MS/s 4-channel TIADC reveal significant improvements in
spurious-free dynamic range (SFDR) and signal-to-noise-plus-distortion ratio (SNDR), with maximum SFDR values increasing
from **56.94 dB** to **74.55 dB** and from **36.76 dB** to **73.76 dB**,
respectively.

## 1 The impact of different structures within each block based on 16 channels
![](https://github.com/OUCIClab/ADC-Res/blob/main/table1.png)


## 2 Ablation Study
### 2.1 The results of channel changes under 4 blocks and 16 FC

![](https://github.com/OUCIClab/ADC-Res/blob/main/table2.png)


### 2.2 The results of block changes under 7 channels and 16 FC

![](https://github.com/OUCIClab/ADC-Res/blob/main/table3.png)

### 2.3 The results of FC changes under 7 channels and 4 blocks

![](https://github.com/OUCIClab/ADC-Res/blob/main/table4.png)
