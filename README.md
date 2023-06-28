EBSysMLSec is a translation tool that takes a SysML model as an input and generates the corresponding Event-B model. The tool is used only in the context of networked control systems (NCS) i.e., the input must agree with a specific style of modeling adopted for specifying an NCS using SysML. This repository contains the source code of EBSysMLSec that support integrating HAZOP with SysML modeling. 

To develop EBSysMLSec, we use ATL- a model transformation language. ATL provides a way to generate several target models from a source model. An ATL transformation program consists of several rules that specify how source model elements are matched with target model elements. The implementation of EBSysMLSec contains four programs (.atl files). Each program takes the input SysML model and generates an Event-B component (either a Machine or a Context). All generated Event-B components form the output of EBSysMLSec.

Run:

Install the Eclipse modeling tool.
Install the ATL plugin.
Create an Atl project
For each program, create an atl file. Creating the file, choose UML ecore as an input metamodel and eventbcore as an output metamodel. UML metamodel exists as a registered package, but eventbcore need to be downloaded from https://sourceforge.net/projects/rodin-b-sharp/files/.
For each program, configure a run and specify the input SysMl model and a directory for the generated .xmb model. An example of an input model is provided in the repository (MovingBlockSysml).
Run the configurations and open the generated files with the rose editor in Rodin.
Specify the refinement chain.
