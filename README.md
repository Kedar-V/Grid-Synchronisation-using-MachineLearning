# Grid Synchronisation using Machine Learning

## Task :

Grid synchronisation is a crucial aspect in controlling grid-connected power electronic converters. To control energy transfers, the primary phase-angle and frequency at the point of common coupling needs to be tracked on-line. PLL is one of the most popular method for synchronisation it has several issues during adverse conditions. Primarily, it fails to track the the voltage and extract its phase properly. In case of power quality issues such as phase jump or frequency jump on the grid side, extra oscillations are caused due to strong coupling between phase and frequency in PLL. Moreover the design of PLL can be tricky - if a better distortion-rejection capability is desired, it will cause a sluggish response, and if a faster response is required, the system can be prone to instability. Lastly, power quality issues are observed when there is a delay in locking to the fundamental frequency. Fine-tuning of PLL parameters is also a very difficult task. From the machine learning (ML) perspective, the problem that the PLL is trying to solve is a regression task. Machine learning methods have been known to be useful in solving such problems. Thus looking into ML based approaches is a natural choice. The various advantages of Machine learning based solution over traditional methods are 
<li> Faster recognition of phase, amplitude and frequency </li>
<li> Better accuracy </li>
<li> Ease in deployment at any location with minor to no fine tuning </li>
