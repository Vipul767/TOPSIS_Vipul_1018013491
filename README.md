# TOPSIS_Vipul_1018013491 #
TOPSIS-Vipul-101803491 is an implementation of Technique of Order Preference Similarity to the Ideal Solution(TOPSIS).
It will help you to place your data acc to preference that is by looking at the data and performing some Maths it will tell you the Preference in which you will be most benefitted. 
If you want to run the code from command line use the following format: 
python topsis.py <InputDataFile> <Weights> <Impacts> <ResultFileName>
Example: python topsis.py inputfile.csv “1,1,1,2” “+,+,-,+” result.csv
 
## Remember!!!! ##
### When you create the .py file (topsis.py in this case) ###
### Just Import the package and call the function just_import_this_fxn_for_whole_topsis_result() by writing :- ###

### import TOPSIS_Vipul_101803491 ###
### TOPSIS_Vipul_101803491.just_import_this_fxn_for_whole_topsis_result() ###

And you will see the desired result!!!

Now let's see the whole thing with the help of an example

Sample dataset
The decision matrix (`a`) should be constructed with each row representing a Model alternative, and each column representing a criterion like Accuracy, Rseq, Root Mean Squared Error, Correlation, and many more.

Model | Corr | Rseq | RMSE | Accuracy
------------ | ------------- | ------------ | ------------- | ------------
M1 |	0.79 | 0.62	| 1.25 | 60.89
M2 |  0.66 | 0.44	| 2.89 | 63.07
M3 |	0.56 | 0.31	| 1.57 | 62.87
M4 |	0.82 | 0.67	| 2.68 | 70.19
M5 |	0.75 | 0.56	| 1.3	 | 80.39

Weights (`w`) is not already normalised will be normalised later in the code.

Information of benefit positive(+) or negative(-) impact criteria should be provided in `I`.

## Result of our input dataset (or example) ##
Model | Corr | Rseq | RMSE | Accuracy | TOPSIS SCORE | RANK
------------ | ------------- | ------------ | ------------- | ------------ | ------------ | ------------
M1 |	0.79 | 0.62	| 1.25 | 60.89 | 0.639133
M2 |  0.66 | 0.44	| 2.89 | 63.07 | 0.212592
M3 |	0.56 | 0.31	| 1.57 | 62.87 | 0.407846
M4 |	0.82 | 0.67	| 2.68 | 70.19 | 0.519153
M5 |	0.75 | 0.56	| 1.3  | 80.39 | 0.828267

The rankings are displayed in the form of a table using a package 'tabulate', with the 1st rank offering us the best 
decision, and last rank offering the worst decision making, according to TOPSIS method.
