# BIOMD0000000248: Lai2007_O2_Transport_Metabolism

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000248.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000248.git@20140916`


# Model Notes


This file describes the SBML version of the mathematical model in the
following journal article: Linking Pulmonary Oxygen Uptake, Muscle Oxygen
Utilization and Cellular Metabolism during Exercise, Ann Biomed Eng. 2007
Jun;35(6):956-69. (Pubmed ID: 17380394). This mathematical model simulates
oxygen transport and metabolism in skeletal muscle in response to a step
change from a warm-up steady state to a higher work rate corresponding to
exercise at different levels of intensity: moderate (M), heavy (H) and very
heavy (VH). The model parameter values are listed in the tables of this
article. The parameter values that are independent of the exercise level are
reported in Table 2. The parameter values that depend on the exercise level
are reported in Tables 1A, 3 and 4. The model simulations (Figures 2, 3, 4 and
5) were obtained for a representative subject with a set of parameter values
different from those in Table 1A, 3 and 4. In the sbml model, these model
parameters are used to simulate exercise at a very heavy (VH) intensity for
the representative subject. Additionally, the parameter values needed to
simulate exercise at moderate (M) and heavy (H) intensity are reported in the
list of parameters of the file. The model simulates dynamics of (1) the
concentrations of free (F) and total (T) oxygen concentration in blood (CFcap,
CTcap) and tissue (CFtis, CTtis), Adenosine Triphosphate (ATP), Adenosine
Diphosphate (ADP), Phosphocreatine (PCr) and Creatine (Cr); (2) the metabolic
flux of oxidative phosphorylation, creatine kinase and ATPase; (3) the oxygen
uptake in blood and oxygen transport rate from blood to tissue during
exercise. The simulation also computes muscle oxygen saturation (StO2m) and
relative muscle oxygen saturation (RStO2m) in order to compare simulated and
experimental responses of human muscle oxygenation during exercise. The model
was successfully tested with Roadrunner of the Systems Biology Workbench
(SBW). The model simulations obtained with Roadrunner match those obtained
with the mathematical model represented in Fortran and Matlab for relative and
absolute tolerance smaller than 10-7.

To allow for simulations at varying levels of exercise, the parameter
**exercise_level** was introduced. A value of 1 means medium, 2 heavy and 3
very heavy exercise. Setting this parameter assigns the parameters **Vmax**,
**KatpaseE**, **dQMm** and **tauQm** with the relevant parameters. The warmup
steady state is influenced by the parameter changes for this representative
subject and the model has to be brought into steady state after each change of
exercise level.

This model originates from BioModels Database: A Database of Annotated
Published Models. It is copyright (c) 2005-2010 The BioModels Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html).  
To cite BioModels Database, please use [Le Nov��re N., Bornstein B., Broicher
A., Courtot M., Donizelli M., Dharuri H., Li L., Sauro H., Schilstra M.,
Shapiro B., Snoep J.L., Hucka M. (2006) BioModels Database: A Free,
Centralized Database of Curated, Published, Quantitative Kinetic Models of
Biochemical and Cellular Systems Nucleic Acids Res., 34: D689-D691.](http://ww
w.pubmedcentral.nih.gov/articlerender.fcgi?tool=pubmed&pubmedid=16381960)


