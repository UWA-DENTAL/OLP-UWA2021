# Computer-assisted machine-learning algorithm can reliably identify oral lichen planus cases 
![DIAGRAM](https://user-images.githubusercontent.com/81205303/112099558-b7591000-8bde-11eb-8a3b-91df0d5381aa.png)
An automated artificial neural network as a machine-learning method was trained to identify and quantify mononuclear cells and granulocytes within the inflammatory infiltrates in digitalized hematoxylin and eosin microscopic slides. 
# Software specifications
QuPath version: 0.2.3, Java version: 14.0.2, Operating system: Windows 10  -  10.0
# apply "stain vector" scribt
# Cell detection
(1) setup parameters (detection image: hematoxylin OD, requested pixel size: 0.5 μm), (2) nucleus parameters (background radius: 8 μm; median filter radius: 0 μm, sigma: 1.5 μm, minimum cell area: 10 μm2, maximum cell area: 400 μm2), (3) intensity parameters (threshold: 0.1, maximum background intensity: 2), and (4) cell parameters (cell expansion: 0 µm, include cell nucleus). 
# calculate features
(1) add smoothened features: 5um, 15um, 25um, 50um (2) compute intensity features: resolution: 2um, tile diameter: 5um, optical density sum: yes, hematoxylin: yes, eosin: yes, residual: yes, red: yes, green: yes, blue: yes, hue: yes, saturation: yes, brightness: yes, mean: yes, sd: yes, min & max: yes, median: yes, compute haralick features: yes, haralick distance: 1 (3) add shape features: area, length, circularity, solidity, max diameter, min diameter, N/C ration
# apply OLP-UWA2021 classifier 
![artificial neural network (ANN-MLP)](https://user-images.githubusercontent.com/81205303/112100290-dad08a80-8bdf-11eb-9edc-df903338e4c4.jpg)
