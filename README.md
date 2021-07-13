# Fracture-Statistics
Descriptive statistics about BHI fractures; Critically stressed faults

 <p style='text-align: justify;'> 

Faults and fractures are the most abundant visible structural features on earth’s crust, and at the same time this is probably the least understood one as well. Most reservoirs in subsurface contains natural fractures, and for all practical purposes one should take “All reservoirs as fractured unless it is proven otherwise“. Fractures have profound effect on reservoir management and field economics, and the severity of the effect becomes multifold in low permeability reservoirs. Characterization of naturally fractured reservoirs and predicting their behaviour is usually difficult both from perspectives of both engineers and geologists. Python, with its powerful statistical and data visualization packages, can be used to access the impact of fracture on well production. 
As with any other subsurface problem, the key to successfully tackle this elusive element is to collect and systematically analyze the data. There are direct evidences of reservoir fracturing like abrupt loss of circulating fluid, petrophysical data like stoneley wave and resistivity and sonic based image logs. Apart from these, there are indirect evidences from production data like khwell/khcore>>1. The acquired data, post analysis by image log specialists, are still sometimes beyond comprehension. And a good statistical interpretation of the data gives an idea about variation of fracture intensity, aerial and vertical direction. 
In figure 1, the hypothetical field has 3 fracture sets. The relative impact of these 3 sets are variable, sets with higher aperture and length have the maximum impact. The 3 wells drilled in the structural high have variable production rates, a function of intersected fracture sets. Well A higher WGR then well B, though B has intersected 2 sets. Whereas well C in structurally low region, has higher WGR with lower production rate.  NNE dipping fracture plane, a set also intersected by well A, is drawing water from GWC. The water column in the well resulted in lower drawdown and lesser production. 

![alt text](https://github.com/Shubhodip-Konar/Fracture-Statistics/blob/main/Readme_Figures/Figure%201.jpg)

Figure 1: Successful development campaign in NFR is dependent on the closer understanding of fracture characteristics of the field.

Though bore hole image (BHI) log can indentify the total population of fractures that intersect the well, but most contribute very little to the flow. Marking those fractures, which enhance production or act as water conduits, is the key factor in developing naturally fractured reservoirs. Complexity on identification increases with higher number of fracture sets.  
In addition to that, the resolution of resistivity based image logs and PLT analysis is vastly different. Only 10-15% faults identifiable by BHI account to production enhancement (Figure 2).

![alt text](https://github.com/Shubhodip-Konar/Fracture-Statistics/blob/main/Readme_Figures/Figure%202.jpg)

Figure 2: Comparison of fractures as seen by BHI and PLT log

This python code snippet will give a preliminary idea about the P10 or the 1D analysis of fractures, through various plots (Figure 3). The same study can be used to create P21 or aerial distribution of the fractures. Post understanding the P10, one can prefix the factors controlling their distribution. A forward prediction algorithm can be used to identify fractures incorporating other information like wireline, drilling or production data.

![alt text](https://github.com/Shubhodip-Konar/Fracture-Statistics/blob/main/Readme_Figures/Figure%203.jpg)

Figure 3: Typical graphical outputs from the code snippet to be used for fracture analysis.

The code is straightforward and heavily dependent on circular data analytics and standard data distribution plots. The user has the liberty to use the analytics for the complete well data or separately for each formation. However, a bottoms-up approach starting with the entire well before delving into each formation was found to be useful by the author.  To capture the stress aspect, a Mohr’s circle analysis of the faults present is given as an output. Figure 4 shows flow chart of the code for better understanding. The Mohr circle analysis (Figure 5) calculates the shear stress/ normal stress acting on the individual planes using Cauchy’s Law, given 2 of the principal stresses are horizontal. For further reading, one can refer to Cornell University structural lab manual (link).  
 

![alt text](https://github.com/Shubhodip-Konar/Fracture-Statistics/blob/main/Readme_Figures/Figure%204.jpg)
 
Figure 4: Flow chart for fracture statistics analysis and outputs
 
![alt text](https://github.com/Shubhodip-Konar/Fracture-Statistics/blob/main/Readme_Figures/Figure%205.jpg)

 Figure 5: Mohr circle analysis of the faults observed in BHI
 
The exported excel files, in TVDSS depth, can be used in standard petroleum geology software. These include calculated µ (shear/normal stress) for all fault planes, 5m frequency plot for fracture set, dip-wise classified fracture frequency data, and frequency plot for specific fracture orientation. 
These trivial looking analyses can give insights on the field development. Average dip and dip azimuth can point to specific fracture set with impact on well production. Fracture classification based on dip value point to genetic origin of the most import set in the location, and point to sweet spot based on structural analysis. Likewise, an overall higher average µ for all the wells in a certain part of the field can be used to plan hydrofrac design. 


</p>
