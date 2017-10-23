# FreelyMovingBehaviorAnalysis

-Instructions of how bout analysis work -

-Running analysis of datasets that have already been added
1) Copy FreelyMovingBehaviorAnalysis_13/ folder to your computer
2) Open the freelyMovingKinAnalysisWithBoutCat_28.m
3) In line 15 of freelyMovingKinAnalysisWithBoutCat_28.m change the path to where the boutmap is in your computer. 
It is located in the subfolder \FreelyMovingBehaviorAnalysis_13\assignBoutTypesUsingMap\BoutMap\
4) Make master folder where the matfile data will reside - can have any name
5) Inside master folder make a folder for each dataset to be analysed- it should have the name of the dataset
6) Add matfiles to each dataset subfolder
7) Add FishMap file to master folder if unique numbers are to link to previous datasets
8) Run freelyMovingKinAnalysisWithBoutCat_28.m and a UI will pop up. The user should click on the master folder.

-Adding new datasets to the analysis
1) Go to the folder \FreelyMovingBehaviorAnalysis_13\kinParFunctions\filesToChangeToAddDataset\.
2) Update the EnumeratorDataSet with the name of your dataset
3) Update the EnumeratorProtocol if you are using a new protocol
4) Open the DataBaseDetector with your name and add the new dataset. Be careful to copy from a previous dataset
of the same behaviour set up and version of the tracking program. Also be careful to update in this file 
the EnumeratorDataSet and the EnumeratorProtocol 
5) Send the \FreelyMovingBehaviorAnalysis_13\kinParFunctions\filesToChangeToAddDataset\ folder to Joao so that the 
analysis remains one and updated. 

-Updating old bout files
Note - I can't guarantee this will work with data analysed by all previous versions of the program, but it should be 
much faster than creating new bout files from scratch.
1)  Go to \BehaviorDataAnalysis_161111\FreelyMovingBehaviorAnalysis_13\fixBoutFiles\ folder. Inside there are 3 folders that 
have scripts that will fix different things.
2) If unique numbers got screwed because you were not careful with adding fish maps. Add the correct fish mat to the master
folder where the bout files are. Erase wrong fish map. Run correctUniqueNumbersAndSeqBug_4.m and pick the master folder. 
3) If you want distance to cluster measure and new eye kin pars. Run addDistToClusterAndEyeConvDiff_1.m
4) If you want to fix the max angular speed kinematic parameters. Run correctMaxAngularSpeed_1.m 

-Applying new bout map to old bout files - this will also include in the bout file the distance to the cluster and new kin pars of the eyes. 
It will not correct the max angular speed kin pars.
1) Go to \FreelyMovingBehaviorAnalysis_13\assignBoutTypesUsingMap\
2) Run assignBoutsOnBoutFilesAndDistToCenterAndUpdateKinPars_5.m
3) Choose master folder with bout files.

Doubts - email me: jcbmarques@gmail.com







