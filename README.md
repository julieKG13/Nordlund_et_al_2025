# Nordlund_et_al_2025
Data &amp; codes of Nordlund et al. 2025 (EPSZTEIN LAB)


DATA

The data of each figure are found in the xsl file. 


CODES

In this github you will find the codes for the manuscript figures + statistics. Note that some codes are common to some figures. 
For codes and figures for the spatial correlation analysis and UMPA : contact Remi Monasson or Hervé Rouault, respectively. 


GENERAL INFORMATION ABOUT THE CODES

Most codes call 2 groups (Groupe 1 and 2). Each group is a folder with folders of each session containing the mat files of the data. Some codes call the supool (=a mat file with the data of all sessions in the group). The list of session for each group and each figure is find in the xsl files. The group identity is also indicated. 

For Figure 1 and Supp 1 : Groupe 1 = Cue poor ; Groupe 2 = Cue Rich

For Figure 2 and Supp 2 : Groupe 1 = Cue poor ; Groupe 2 = Cue Rich

For Figure Supp 3 : Cue poor only (Groupe 1)

For Figure Supp 4 : Groupe 1 = Muscimol ; Groupe 2  = aCSF

For Figure 4 : Muscimol only (Groupe 1)

For Figure Supp 5 : Muscimol only (Groupe 1)

For Figure 6 : Groupe 1 = Muscimol  ; Groupe 2 = aCSF

Contact us to have the mat files containing the Data. 


FUNCTIONS : 

To generate Rate maps, detect place fields, clasify cells as active / place cells / bidirectional or unidirectional place cells : 
Function : Main_RateMaps_PlaceFields_CellsClassification
NB : Note that you will need to add some variables on your own (all explanations in the function)


Figure 1Supp : 

Number of reward per minute :
Function : Perf_rewardpermin

% of active /place / bidirectional cells :
Function : Fig1_Supp

Check whether, in the Cue rich condition, fields of position and distance coding BI cells are homogeneoulsy  distributed (cue zone / No cue zone) : 
Function : Fig1_Supp_PFdistribution_cuerich


Figure 1 :

Calculate Distance & Position index of BI cells : 
Function : Determine_DisPos_index

Distance vs Position Index in Cue poor and Cue rich
% of distance and position coding bidirectional place cells
Function : Fig1_DistPosIndex

Bidirectional firing rate map plot : 
Function : Bi_Rank_fig1

Bidirectional distance and position firing rate map plot : 
Function : BidPOSDIS_Rank


Figure 2 Supp :

Y position of deep and superficial cells in CP and CR conditions : 
Calculate Y position : 
Function Determine_Yposition

Y position of deep and sup in both conditions :  
Function Deep_Sup_Yposition_VS_index

% of active cells
Function Fig2_ActiveCells

% of place cells
Function Fig2_PlaceCells

% of bidirectional cells 
Function Fig2_BICells


Figure 2 : 

Correlation between Y position of BI and position/distance coding : 
Function Deep_Sup_Yposition_VS_index

Bidirectional firing rate map plot for DEEP and SUP : 
Function Bid_Rank_2cdt_DEEPSUP

Position index Deep vs Sup 
Function Fig2_PositionNDX

Distance index Deep vs Sup 
Function Fig2_DistanceNDX

% BI position and distance coding
Function Fig2_percent_DistanceCells


Figure 3 Supp

Quality of UNI cells (way SM vs non SM)
+ quality of UNI vs BI vs non SM 
Function : UNI_quality_pool

Spatial correlation 
Function : SC_figUNI

Unidirectional firing rate map : 
Function : UNI_Rank_2cdt


Figure 4 Supp

Do the supool (with spatial correlation random)
Function : Fig4_pool

% of inactivation theta mov power 2 conditions (before / after) : 
Function : Analyse_Theta_pow_inactivation

Mean trial Speed Comparison Before/after Muscimol 
Function SpeedBeforeAfter_boxplot()

Nb of Stop Comparison Before/after Muscimol or aCSF
Function FigStop


Figure 4

% of bidirectional cells before/after infusion : 
Function Fig4_percentCells

Relative change before/after infusion for BI, UNI and nonPC :
Function Fig4_RateChange

Shuffling spatial correlation :
Function Generate_SC_Random

Spatial correlation aligned to starting point for UNI and non PC : 
Function : Fig4_SC_Analyses

Generate random map for population vector analysis : 
Function generate_random_map

Test population vector analysis : 
Function : test_PopVec_ori

Distance overlap : 
Function : Bid_Rank_2cdt_DistanceOverlap


Figure 5 Supp

Number of reward per minute, percentage Active cells-PC, quality of PC : before/after infusion : 
Function : Figure4_pool_boxmath_perf_Percent_quality

Distance overlap : 
Function : Bid_Rank_2cdt_DistanceOverlap


Figure 6 Supp

Percentage Active cells-PC before/after infusion : 
Function : Figure4_pool_boxmath_perf_Percent_quality

% of bidirectional cells before/after infusion : 
Function Fig4_percentCells


Figure 6

% of inactivation theta mov power 3 conditions (before / afterCP / after CR) 
Function Analyse_Theta_pow_inactivation_3cond

Distance and position index CSF vs Musci (CR condition = 3rd condition)
Function Fig6_PositionNDX

Bid firing rate map plot 3 conditions : 
Function : Fig6_Bid_Rank_3cdt

Plot position Index versus Distance index / all conditions BEFORE : 
Function Fig6_DisPoscells_CP_before

Plot position Index versus Distance index / CR after : 
Function Fig6_PosDiscells



