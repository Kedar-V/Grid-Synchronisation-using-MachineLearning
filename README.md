# Grid Synchronisation using Machine Learning

## Task :

Grid synchronisation is a crucial aspect in controlling grid-connected power electronic converters. To control energy transfers, the primary phase-angle and frequency at the point of common coupling needs to be tracked on-line. PLL is one of the most popular method for synchronisation it has several issues during adverse conditions. Primarily, it fails to track the the voltage and extract its phase properly. In case of power quality issues such as phase jump or frequency jump on the grid side, extra oscillations are caused due to strong coupling between phase and frequency in PLL. Moreover the design of PLL can be tricky - if a better distortion-rejection capability is desired, it will cause a sluggish response, and if a faster response is required, the system can be prone to instability. Lastly, power quality issues are observed when there is a delay in locking to the fundamental frequency. Fine-tuning of PLL parameters is also a very difficult task. From the machine learning (ML) perspective, the problem that the PLL is trying to solve is a regression task. Machine learning methods have been known to be useful in solving such problems. Thus looking into ML based approaches is a natural choice. The various advantages of Machine learning based solution over traditional methods are: 
<li> Faster recognition of phase, amplitude and frequency </li>
<li> Better accuracy </li>
<li> Ease in deployment at any location with minor to no fine tuning </li>

## Dataset:

The lack of large scale, well curated datasets which can accurately model the real world scenarios is one of the limiting factors in the large scale adoption of machine learning based solutions in the electrical domain. To solve this issue a new dataset titled ”GridSync” is prepared. The algorithm used for data generation is **_NOT INCLUDED IN THIS REPOSITORY DUE TO PRIVACY REASONS (UNTIL PUBLISHED)

## MY APPROACH : 
 **_NOT INCLUDED IN THIS REPOSITORY DUE TO PRIVACY REASONS (UNTIL PUBLISHED)
 
## Results :
The model is evaluated on its ability to predict the am- plitude, phase and frequency of the grid signal. The waveform in blue represents the original signal, and the one in red represents the predicted signal. From these graphs, we are able to gauge that the model is able to precisely predict the desired values even during severe fault conditions and is quickly synced with the input signal. The mean average error for the three predictions is of the order 10<sup>3</sup> after <b>200 epochs</b> as shown in the Table.

<img src="https://github.com/Kedar-V/Grid-Synchronisation-using-MachineLearning/blob/main/images/res.png" width="350"/>

|   | Traning Mae | Validation Mae |  
| ----- | ------- | --- | 
| Amplitude | 0.004 | 0.0011 |
| Frequency | 0.004 | 0.00378 |
| Phase | 0.0097 | 0.0082 |
