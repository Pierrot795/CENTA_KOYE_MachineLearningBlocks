

The Database contains a record of  5473 observations from 54 distinct documents.
The number of attributes is 11 and it contains the target variable.
All attributes are numeric and there are no missing values
Each observation concerns one block. The problem consists in classifying all the blocks of the page layout of a document that has been detected by a segmentation process. 
This is an essential step in document analysis in order to separate text from graphic areas.
 Indeed, the five classes are: text (1), horizontal line (2),picture (3), vertical line (4) and graphic (5).


the attributes are defined below :

 height:   integer.         | Height of the block.
   lenght:   integer.     | Length of the block. 
   area:     integer.    | Area of the block (height * lenght);
   eccen:    continuous.  | Eccentricity of the block (lenght / height);
   p_black:  continuous.  | Percentage of black pixels within the block (blackpix / area);
   p_and:    continuous.        | Percentage of black pixels after the application of the Run Length Smoothing Algorithm (RLSA) (blackand / area);
   mean_tr:  continuous.      | Mean number of white-black transitions (blackpix / wb_trans);
   blackpix: integer.    | Total number of black pixels in the original bitmap of the block.
   blackand: integer.        | Total number of black pixels in the bitmap of the block after the RLSA.
   wb_trans: integer.          | Number of white-black transitions in the original bitmap of the block.




Class Distribution: 

                                           Valid    Cum
   Class               Frequency  Percent  Percent  Percent
 
text                      4913     89.8     89.8     89.8
horiz. line                329      6.0      6.0     95.8
graphic                     28       .5       .5     96.3
vert. line                  88      1.6      1.6     97.9
picture                    115      2.1      2.1    100.0
                                -------  -------  -------
                        TOTAL      5473    100.0    100.0

Summary Statistics:

Variable      Mean    Std Dev   Minimum   Maximum   Correlation 

HEIGHT       10.47      18.96         1       804         .3510
LENGTH       89.57     114.72         1       553        -.0045
AREA       1198.41    4849.38         7    143993         .2343
ECCEN        13.75      30.70      .007    537.00         .0992
P_BLACK        .37        .18      .052      1.00         .2130
P_AND          .79        .17      .062      1.00        -.1771
MEAN_TR       6.22      69.08      1.00   4955.00         .0723
BLACKPIX    365.93    1270.33         7     33017         .1656
BLACKAND    741.11    1881.50         7     46133         .1565
WB_TRANS    106.66     167.31         1      3212         .0337

