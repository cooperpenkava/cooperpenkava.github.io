---
layout: page
title: CNC Mill Paper Punch
---

_**Skills Used:**_
 - **_CNC Milling_**
 - **_Fit Need Analysis_**
 - **_High Efficiency Milling - 30 Minute Time Constraint_**
 - _**Tolerance Stackups**_
 - _**Technical Drafting**_

For my Design for Manufacturing class, I and another student made a star shaped paper punch, comprised of a negative and positive feature that went together via two dowel pins.

Given that the two pieces came together to act as a paper punch, we build design requirements around this. Our design needed to:
 - have a positive and negative feature close enough to punch the paper
 - align easily, such that you could slam the top to punch the paper without interference  
Additionally, as part of the class, we had additional given requirements. Our design also needed to:
 - be manufacturable from two pieces of 3"x3"x1.25" Aluminum square stock
 - be manufacturable entirely on the CNC Mill
 - have an elapsed milling time of 30 minutes or less per part
 - Consist of only two distinct pieces after assembly (any dowel pins used must be permanently fixed to a block
 - External parts (i.e. dowel/diamond pins) may only be fixed with fits - no adhesives.

The design worked! The press fit on the bottom piece was executed correctly, and the locational tolerancing of the dowels was effective in ensuring our sliding fit held true. The level of clearance selected and perpendicularity of the star positive and negative features was effective in cutting paper.
    Photograph of the final product
    Photographs of the manufacturing process
    CAD/renderings of your design
    CAM tool paths
    Exploded assembly drawing (see this tutorial for more on exploded views)
    Dimensioned drawings of final parts using GDT principles
    Any graphs or other analysis you completed
    
There were three main challenges we faced in designing this punch.
1. Locational Tolerancing  
As part of assembly, we needed locational features that would allow us to align the top and bottom pieces effectively. We were recommended a diamond and dowel pin approach by the class (the base assignment was just to make any box top and bottom that fit together), but those pins were not long enough to effectively align the two before punching out the paper, so we had to design around longer dowel pins from a cabinet of leftover pins. This meant that the locational tolerancing for all features (the star positive and negative, the center of the press fit hole for the dowel pins, and the center of the running fit hole for the pins had to be very good. Our sliding fit on the upper piece allowed for 0.2 thousandths on either side at MMC (more on this later). The x-y resolution of the CNC mill is 0.1 thou, so even if both holes were off, they would have worked effectively. We made sure to be extremely exact with the Heimer to prevent any user-added error on this.

2. Dowel Pin Force Fit/Sliding Fit  
Part of the requirements for the class was for us to use a force fit for any dowel pins we used. This meant that we had to have precision in our manufacturing of the holes. For this, we spot drilled the holes to ensure a surface for the drill bit to bite into, then used a 0.246" drill bit (~3% under reamer size), and finally used a 0.2495" reamer to bring our force fit to a level that would hold the dowel pin permanently but at a level that we could still press in the dowel pin with just an arbor press. For the sliding fit above, we did the same process, but ended with the 0.2505" reamer to ensure we were above the dowel pin's maximum diameter spec. According to McMaster, the dowel pins we had could be maximum 0.0003" over nominal (0.25"), so our hole needed to have a running fit that could accomodate this 0.3 thou, plus the +/- 0.1 thou for each hole at absolute MMC. This brought us to our 0.2505" hole sizing.

3. Star Positive/Negative Feature Clearance and Effectiveness  
In order to make a geometry that actually could cut paper put between the two box halves, we needed a fit that was very close. However, due to various factors - the locational deviation from the holes, the deflection of the end mill on both halves, and the locational deviation while making the star geometry - we could not make it too close, or else we would risk interference between the positive and negative geometry. Accounting for the potential locational deviation for each feature along with the tool deflection (calculated with this tool), we determined that a H8/f7 fit was the closest running fit we could achieve confidently. For the sake of CAD, we treated the negative feature as the hole, and just offset its shape by the upper bound of the offset for the hole (the upper bound because tool deflection should leave material behind, so the feature will most likely be smaller than in CAD). We did the opposite for the positive feature (offset by the lower bound of the offset for the shaft).
