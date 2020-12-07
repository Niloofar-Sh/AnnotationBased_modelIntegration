.. Automated Model Composition documentation master file, created by
   sphinx-quickstart on Mon Dec 1 16:22:42 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. _The_approach:

================
**The Approach**
================

To be able to reuse and compose models in online repositories such as PMR, we need a tool to first, convert a non-bond-graph model into an equivalent bond graph one; second, automatically assign the parameters in the models to the bond graph components; third, identify the same entities in the models as the merging points and make the necessary changes to join the models without any loss of information.  

The automation in the model composition can be achieved by adding information (standard meaningful names) to the variables. Ontologies are databases which contain standard descriptive names (annotations) in domains of physics, biology, genes, chemistry, and so forth. By annotating the models' variables, similar entities can be detected among the models and considered as potential merging points.

To improve our model composition method towards automation and to reuse the models in other formalisms, we employed the idea of having symbolic bond graph templates along with their connectivity matrices. For the identification of the merging points between the models, we still need the variables and parameters of the models to be fully annotated. To summarize, the prerequisites of this automated model composition method are as follows:

* Bond graph symbolic templates of the models,
*  Connectivity matrix of each template defining whether the components are connected to the other ones or not by '1's and '0's,
* Ontologies required for matching the annotations, and
* Annotated models.

In a given biological/physiological/physical context, our tool can detect the type of bond graph template required for substituting the original annotated model. Thereafter, by finding similar annotations in the models, the merging points will be selected. Based on this, the required changes in the bond graph components (deleting the duplicates) and the connectivity matrices (adding/deleting rows and columns or inserting '1's) will be made. Ultimately, the final model will be produced based on the connection/non-connection relationships between all the components. This approach generated a model of signalling pathways (MAPK cascades), and the simulation results were verified. The flowchart of this approach is given in Figure 1. 

.. figure:: _images/flowchart.jpg
    :width: 700px
    :align: center
    :height: 900px
    :alt: alternate text
    :figclass: align-center

    Figure 1. The flowchart of the model composition automation.


        