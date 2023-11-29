# A Physics-Based Deep Learning Approach for Cross Domain Bearing Fault Detection
We have developed a physics-based deep learning approach to detect faults in the bearing across different working conditions. This work is published in IEEE conference proceedings [[1]](https://ieeexplore.ieee.org/abstract/document/10215413)

## Abstract
Bearing fault detection across varying rotational speeds of induction motors (cross-domain) is difficult due to challenges associated with different data distributions under different operating modes. To build a fault detection model, it is required to capture the domain invariant features not influenced by speed variations. Existing methods for bearing fault detection exploit data-driven deep learning models without considering any structural information of bearing. This paper proposes a physics-informed deep learning approach for bearing fault detection across different working conditions of the motor. The proposed method utilizes the power spectrum of the envelope signal (PSES) from the vibration data as an input feature for 1D CNN deep learning network. The proposed method is compared with the Random Forest and 1D CNN with raw data input and evaluated on two public bearing datasets to demonstrate its superior performance and robustness to speed variation. The proposed method is able to predict cross-domain bearing faults with an average accuracy of 94.2% which is 23% higher than the existing state-of-the-art data-driven approach.

## Dataset
The data set used in this work to evaluate the proposed model is the [Case Western Reserve University Bearing Dataset](https://engineering.case.edu/bearingdatacenter) and JNU dataset. Both datasets consist of ball bearing test data for normal and faulty bearings at different loading conditions. 

## Flowchart for the proposed model
<p align="center">
<img src="https://i.imgur.com/13TDkwo.jpg" width=50% height=50%>
</p>

## Contributions
1. We propose, for the first time, a physics information-based deep learning model for cross-domain bearing fault detection. We demonstrate its superior performance to the state-of-the-art data-driven method using tests on two public bearing datasets.

2. We highlight that the power spectrum of the envelope signal, which is used as input for the proposed deep learning model, shows negligible variance in the cross-domain conditions. So, this feature can be used to build a cross-domain bearing fault detection model.

Most of the approaches currently used for cross-domain bearing fault detection have been tested using motors with less speed variation, such as the well-known CWRU(Case Western Reserve University) dataset. This paper also discusses the disadvantages of employing such datasets.

## Feature Extraction
<p align="center">
<img src="https://i.imgur.com/WJcpG15.gif" width=100% height=100%>
</p>
Envelope spectrum of raw signal from JNU dataset at 800 rpm (a,b,c) and CWRU dataset at 3hp loading condition (d,e,f).

## 1D CNN 
<p align="center">
<img src="https://i.imgur.com/PPNPNii.jpg" width=70% height=70%>
</p>


## Results
<p align="center">
<img src="https://i.imgur.com/oEcLZCZ.jpg" width=80% height=80%>
</p>
<p align="center">
<img src="https://i.imgur.com/dLsmVYG.jpg" width=80% height=80%>
</p>




## References 
[1] S. Anbalagan, B. Natarajan and B. Srinivasan, "A Physics Based Deep Learning Approach for Cross Domain Bearing Fault Detection," 2023 IEEE Kansas Power and Energy Conference (KPEC), Manhattan, KS, USA, 2023, pp. 1-4, doi: 10.1109/KPEC58008.2023.10215413.


