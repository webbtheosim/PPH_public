# DATA ON ENZYME ACTIVITY RETENTIOON IN GLUCOSE OXIDASE, LIPASE, AND HORSERADISH PEROXIDASE
This repository contains data and code necessary for constructing machine learning models that facilitated the design of new polymer-protein hybrid materials.

The content is available under CC BY NC 4.0 License

# REFERENCES
The specific application, data, and machine learning models are described in 
1. ^Tamasi, M. J.; ^Patel, R.A., ^Borca, C. H.; ^Kosuri, S.; Mugnier, H.; Upadhya, R.; Murthy, N.S.; *Webb, M.A.; *Gormley, A.J (^ denotes equal contributions, * denotes corresponding authors), Advanced Materials, 2022, DOI: 10.1002/adma.20220180

The featurization method used for the machine learning models is described in 
2. Patel, R. A.; Borca, C. H. & Webb, M. A. "Featurization strategies for polymer sequence or composition design by machine learning"  Molecular Systems Design & Engineering, 2022, DOI: 10.1039/d1me00160d

The data itself is assigned the following DOI: 

# DIRECTORIES
A description of files/directories appears below

# data
The `data' directory includs three .csv files that contain data specific for three enzymes: gox.csv, hrp.csv, and lip.csv. These respectively correspond to the enzymes glucose oxidase, horseradish peroxidase, and lipase. 

Each .csv file has the same format with thirteen columns as described below:
A.) Polymer Number - numerical index identifier for a given copolymer. This is not generally used.
B.) DP - This is the target degree of polymerization for copolymer synthesis. Synthetic procedures are constructed so as to achieve this number of monomers in a given copolymer.
C.-J.) Each column here indicates the target fraction of incorporation for the given monomer type assigned to that column. There are eight monomer types: 2-(diethylamino)ethyl methacrylate, 2-hydroxypropyl methacrylate, 2-sulfopropyl methacrylate, butyl methacrylate,3-(dimethylamino)propyl methacrylate, methyl methacrylate, poly(ethylene glycol) methyl ether methacrylate, trimethylammonium chloride ethyl methacrylate 
K. REA - This is "retained enzyme activity" for the copolymer plus enzyme system that is registered in an enzyme-specific experimental assay. The assays are described in Ref. 1
L. Generation - This is a label that indicates when the copolymer was synthesized during the active learning process described in Ref. 1. '0' indicates that the copolymer was synthesized as part of the "seed" dataset. The set of copolymers in the "seed" dataset are the same in all .csv files. Subsequent generations are enzyme-specific and chosen according to procedures described in Ref. 1. 
If G represents the generation of a given set of copolymers, then these polymers are proposed using machine learning models that are trained on data from data collected from generations 0 through (G-1).

Gelation - This is a binary variable that signifies whether gelation was experimentally observed post synthesis. `0' indicates no gelation while `1' indicates gelation. Samples that undergo gelation are addressed using procedures described in Ref. 1, but generally, data for copolymers that are observed to gel are not included in machine learning trained to predict REA.

# HELP, SUGGESTIONS, CORRECTIONS?
If you need help, have suggestions, identify issues, or have corrections, please send your comments to Prof. Mike Webb at mawebb@princeton.edu

