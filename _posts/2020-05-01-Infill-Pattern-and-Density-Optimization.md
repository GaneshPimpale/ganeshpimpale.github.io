---
layout: page
title: "Infill Pattern and Density Optimization for 3D Printing with Analytical Physics"
subtitle: "A novel approach to provide fused deposition modeling printers software to create stronger, lighter and faster to print parts"
date:   2020-05-01 21:21:21 +0530
categories: ["3D Printing"]
---

Created with Andrew Dang.

# Abstract
This project intends to optimize infill patterns of 3D printed objects to provide the highest ratio of force withstood to the mass of the 3D printed object through the means of different algorithms. The first algorithm is area based optimization where the part’s infill density changes depending on the relative area of a section of an area compared to the entire layer. The second is simulation based infill where the part’s infill depends will be determined by simulation data. The final algorithm is a generative support structure algorithm where a part’s infill design is generated as a result of the part’s shape and its points of high stress. 

The algorithms were tested by printing test parts in polylactic acid (PLA) 1.75mm filament through a 0.4mm nozzle. Parts created performed three different tests: top down compression, torquing, and tension. The area based algorithm had mixed results that greatly varied on the design of the shape and the precision of the voxel meshing value. As this value approaches zero, the average infill density of the part reaches it’s optimized value. However, the areas of higher density do not always relate to areas that go under more stress when tested and sometimes may not contribute to the structural integrity of the object. The results of the simulation based algorithm were much more repeatable and only minutely varied based on the precision that the calculations were performed with. The generative support structure algorithm was theoretically tested through calculations that determined its possible loads and computation complexity when creating an object. The current implementation of the algorithm makes it the most optimal for object strength to mass ratio, however, the calculation process is very computationally heavy.

Further research in this topic would involve the incorporation of calculating the flexibility of certain materials. These types of calculations allow for the algorithms to compute the amount of movement, if any, when an object is under load. There are also other methods of a generative support algorithm that could lower its time complexity during the creation. Other possible solutions are to incorporate deep learning with physics to further investigations in the field and create a faster and more in-depth algorithm.

# Paper
[Gallery](https://drive.google.com/drive/folders/1h0pZx0iCYm8NND-cR01aBG_UOFA_Q5Ps?usp=sharing)
<object data="{{'/assets/pdf/(IPDO)Paper.pdf' | prepend: site.baseurl}}" type="application/pdf" width="800px" height="1100px">
    <embed src="{{'/assets/pdf/(IPDO)Paper.pdf' | prepend: site.baseurl}}">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="{{'/assets/pdf/(IPDO)Paper.pdf' | prepend: site.baseurl}}">Download PDF</a>.</p>
    </embed>
</object>

# Poster
<object data="{{'/assets/pdf/(IPDO)Poster.pdf' | prepend: site.baseurl}}" type="application/pdf" width="800px" height="600px">
    <embed src="{{'/assets/pdf/(IPDO)Poster.pdf' | prepend: site.baseurl}}">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="{{'/assets/pdf/(IPDO)Poster.pdf' | prepend: site.baseurl}}">Download PDF</a>.</p>
    </embed>
</object>