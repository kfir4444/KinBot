[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/zadorlab/KinBot)

# KinBot: Automated reaction pathway search for gas-phase molecules

<p>
    <img src="graphics/kinbot_logo_V2.png" width="220" height="240" />
</p>

## Description
This repository contains the KinBot code version 2.0,
a tool for automatically searching for reactions on the potential energy surface.

If you are using this tool in scientific publications, please reference this git repo and the following publication:

Ruben Van de Vijver, Judit Zádor: KinBot: Automated stationary point search on potential energy surfaces, Computer Physics Communication, 2019, 106947 https://doi.org/10.1016/j.cpc.2019.106947

We appreciate if you send us the DOI of your published paper that used KinBot, so we can feature it here below.

## How to Install
Make sure all dependencies are correctly installed. The dependencies are lister here https://github.com/zadorlab/KinBot/wiki/Setting-Up-KinBot-on-Your-System 

Clone the project to the place where you want to run it. Make sure you switch to the latest version, e.g., 2.0.5:

    git branch 2.0.5

You can find the latest stable version's tag if you click on the Branch button above on this page.

In your local space go into the KinBot/ directory. Run the following:

    python setup.py build
    python setup.py install
    
If you do not have admin priveleges, you might have to run

    python setup.py build
    python setup.py install --user
    
Moreover, if you plan to modify the code, you need to install it as:

    python setup.py build
    python setup.py develop --user
    
Please note that you will need the ase version linked to at https://github.com/zadorlab/ase installed
and linked to in your path during the installation of KinBot. This version of ase has changes within it that
are local to KinBot, using any other ase versions will likely result in errors when trying to run reaction searches.

## How to Run
To run KinBot (which will only explore one well), make an input file (e.g. input.json) and run:

    kinbot input.json

To run a full PES search, make an input file (e.g. input.json) and run:

    pes input.json

You can find additional command line arguments in the manual. 

## Documentation
See [wiki](https://github.com/zadorlab/KinBot/wiki).

## List of files in this project
See [list](https://github.com/zadorlab/KinBot/wiki/KinBot-file-structure).

## Authors
* Judit Zador (jzador@sandia.gov)
* Ruben Van de Vijver (Ruben.VandeVijver@UGent.be)
* Amanda Dewyer (adewyer@sandia.gov)

## Papers using KinBot
* Doner, A. C., Zádor, J., Rotavera, B.: Stereoisomer-dependent unimolecular kinetics of 2,4-dimethyloxetane peroxy radicals. Faraday Discussions, **2022**, https://doi.org/10.1039/D2FD00029F
* Ramasesha, K., Savee, J. D., Zádor, J., Osborn, D. L.: _A New Pathway for Intersystem Crossing: Unexpected Products in the O(3P) + Cyclopentene Reaction._ J. Phys. Chem. A, **2021**, 125 9785-9801. https://doi.org/10.1021/acs.jpca.1c05817
* Rogers, C. O, Lockwood, K. S., Nguyen, Q. L. D., Labbe, N. J.: _Diol isomer revealed as a source of methyl ketene from propionic acid unimolecular decomposition._ Int. J. Chem. Kinet., **2021**, 53, 1272–1284. https://doi.org/10.1002/kin.21532
* Lockwood, K. S., Labbe, N. J.: _Insights on keto-hydroperoxide formation from O2 addition to the beta-tetrahydrofuran radical._ Proceedings of the Combustion Institute, **2021**, 38, 1, 533. https://doi.org/10.1016/j.proci.2020.06.357
* Sheps, L., Dewyer, A. L., Demireva, M., and Zádor, J.: _Quantitative Detection of Products and Radical Intermediates in Low-Temperature Oxidation of Cyclopentane._ J. Phys. Chem. A **2021**, 125, 20, 4467. https://doi.org/10.1021/acs.jpca.1c02001
* Zhang, J., Vermeire, F., Van de Vijver, R., Herbinet, O.; Battin-Leclerc, F., Reyniers, M.-F., Van Geem, K. M.: _Detailed experimental and kinetic modeling study of 3-carene pyrolysis._ Int. J. Chem. Kinet., **2020**, 52, 785-795. https://doi.org/10.1002/kin.21400
* Van de Vijver, R., Zádor, J.: _KinBot: Automated stationary point search on potential energy surfaces._ Computer Physics Communications, **2020**, 248, 106947. https://doi.org/10.1016/j.cpc.2019.106947
* Joshi, S. P., Seal, P., Pekkanen, T. T., Timonen, R. S., Eskola, A. J.: _Direct Kinetic Measurements and Master Equation Modelling of the Unimolecular Decomposition of Resonantly-Stabilized CH2CHCHC(O)OCH3 Radical and an Upper Limit Determination for CH2CHCHC(O)OCH3+O2 Reaction._ Z. Phys. Chem., **2020**, 234, 1251. https://doi.org/10.1515/zpch-2020-1612


Older Version of KinBot:
* Van de Vijver, R., Van Geem, K. M., Marin, G. B., Zádor, J.: _Decomposition and isomerization of 1-pentanol radicals and the pyrolysis of 1-pentanol._ Combustion and Flame, **2018,** 196, 500. https://doi.org/10.1016/j.combustflame.2018.05.011
* Grambow, C. A., Jamal, A., Li, Y.-P., Green, W. H., Zádor, J., Suleimanov, Y. V.: _Unimolecular reaction pathways of a g-ketohydroperoxide from combined application of automated reaction discovery methods._ J. Am. Chem. Soc., 2018, 140, 1035. https://doi.org/10.1021/jacs.7b11009
* Rotavera, B., Savee, J. D., Antonov, I. O., Caravan, R. L., Sheps, L., Osborn, D. L., Zádor, J., Taatjes, C. A.: _Influence of oxygenation in cyclic hydrocarbons on chain-termination reactions from R + O2: tetrahydropyran and cyclohexane._ Proceedings of the Combustion Institute, **2017,** 36, 597. https://doi.org/10.1016/j.proci.2016.05.020
* Antonov, I. O., Zádor, J., Rotavera, B., Papajak, E., Osborn, D. L., Taatjes, C. A., Sheps, L.: _Pressure-Dependent Competition among Reaction Pathways from First- and Second-O2 Additions in the Low-Temperature Oxidation of Tetrahydrofuran._ J. Phys. Chem. A, **2016,** 120 6582. https://doi.org/10.1021/acs.jpca.6b05411
* Antonov, I. O., Kwok, J., Zádor, J., Sheps, L.: OH + 2-butene: A combined experimental and theoretical study in the 300-800 K temperature range. J. Phys. Chem. A, **2015,** 119, 7742. https://doi.org/10.1021/acs.jpca.5b01012
* Zádor, J., Miller, J.A.: _Adventures on the C3H5O potential energy surface: OH + propyne, OH + allene and related reactions._ Proceedings of the Combustion Institute, **2015,** 35, 181. https://doi.org/10.1016/j.proci.2014.05.103
* Rotavera, B., Zádor, J., Welz, O., Sheps, L., Scheer, A.M., Savee, J.D., Ali, M.A., Lee, T.S., Simmons, B.A., Osborn, D.L., Violi, A., Taatjes, C.A.: _Photoionization mass spectrometric measurements of initial reaction pathways in low-temperature oxidation of 2,5-dimethylhexane._ J. Phys. Chem. A, **2014,** 44, 10188. https://doi.org/10.1021/jp507811d

## Acknowledgement
This research was supported by the Exascale Computing Project (ECP), Project Number: 17-SC-20-SC, a collaborative effort of two DOE organizations, the Office of Science and the National Nuclear Security Administration, responsible for the planning and preparation of a capable exascale ecosystem including software, applications, hardware, advanced system engineering, and early test bed platforms to support the nation's exascale computing imperative. RVdV was also supported by the AITSTME project as part of the Predictive Theory and Modeling component of the Materials Genome Initiative. Sandia National Laboratories is a multimission laboratory managed and operated by National Technology and Engineering Solutions of Sandia, LLC., a wholly owned subsidiary of Honeywell International, Inc., for the U.S. Department of Energy’s National Nuclear Security Administration under contract DE-NA0003525. 
