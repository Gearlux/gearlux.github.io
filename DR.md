<a href="Tomosynthesis.html"><img src="images/prev.png" width="40" height="40"></a>
<a href="index.html"><img src="images/back.png" width="40" height="40"></a>
<a href="Mammo.html"><img src="images/next.png" width="40" height="40"></a>

<a href="https://gearlux.github.io/"><img src="images/Profile.png" width="200" height="150"></a>

# Portfolio

## DR Roadmap

### Task
Identify opportunities for Agfa to improve its portfolio within Direct Radiography.

### Action
Together with application and marketing, we contacted several radiographers and radiologists and interviewed them for their opinion on features, future vision, possible improvements and new technology. 

### Result
The result was a roadmap where key topics were identified: 
* mobile imaging
* workflow
* improved diagnosis 
* image consistency. 

This was the beginning of the development of 
* [Tomosynthesis](Tomosynthesis.md) (*improved diagnosis*)
* mobile tomosynthesis (*improved diagnosis*, *mobile imaging*)
* [SmartXR](Portfolio.md#smartxr) (*workflow*, *image consistency*, *mobile imaging*)
* [Deep learning projects](DeepLearning.md) (*workflow*, *image consistency*)

### Responsibilities
Innovation Manager, Software Architect, Team Lead

## Full Leg Full Spine
Automatic image stitching of DR images. 

![](images/dr600.png)

### Task
Develop a method for FLFS (Full Leg Full Spine) imaging for DR images with similar quality requirements as the one-shot CR FLFS.

![](images/dxd300.png)

### Action
I developed the interface to the modality, the module computing the optimal position of the images while keeping the X-ray source stable and the image processing module which stitches the images and detects possible patient movement during the acquisition. Because the old C R stitch grid, could not be used, I developed a new stitch grid which was enabled the correction of the patient movement and which was less disturbing for the radiologist. With the mechanical team in Munich, I co-designed a patient stand which ensures that the patient could stand still and protected the patient from the moving parts of the modality.

### Result
A new stitch grid, a new patient stand and new, more robust algorithms were designed, implemented and validated. 

![](images/grid.png)

[//]: # (Include a full leg full spine stitched image)


### Responsibilities
Project Lead, Software Developer

<a href="Tomosynthesis.html"><img src="images/prev.png" width="40" height="40"></a>
<a href="index.html"><img src="images/back.png" width="40" height="40"></a>
<a href="Mammo.html"><img src="images/next.png" width="40" height="40"></a>
