.. Automated Model Composition Documentation master file, created by
   sphinx-quickstart on Mon Dec 22 16:22:42 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

=====================================
    **Introduction**
=====================================

Complicated systems and pathways can be commonly seen in physiology and biology. Modelling these complicated systems from scratch is demanding. Using the concept of modularity helps to enhance our modelling methods. Most of these complicated systems consist of several sub-systems, operating in connection to others. Modelling the sub-systems separately and reusing them either in connection to other sub-systems or another sophisticated model can finally lead to achieving a realistic model of an organ or even the human body. 

Obstacles in model composition
###############################

* **Non-reusable models:** modellers cannot reuse the others’ models because of lack of consistency; not all the modelling formalisms can be converted to each other. 

* **Implausible models:** Even if the modelling schemes are the same, there is no guarantee that the final composed model will represent a real physiological system with acceptable behaviour. Not all the modellers follow the physical laws in their modelling approach.

* **Additional adjustments:** Combining different mathematical models often need some modifications in the computations and equations. This requires a vast knowledge of the system's operation and also spending a considerable amount of time (let alone occurring any human errors during the modifications). 

Solution
#########

To tackle the mentioned issues, we need an approach that meets all these requirements. Bond graphs approach is a physics-based modelling scheme that generates plausible models which are reusable and suitable for hierarchical modelling. However, we should bear in mind that although bond graphs are a great aid in model composition, many available models are not based on the bond graphs principles.
 












