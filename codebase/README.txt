# Project title: Super 11
# Team members: Guneet (gkhosla3), Pranit (pkaul9), Karthik (kanil3), Prithvi (psuresh38)
# Graduate team
         
# Files in the CODE directory
-   codebase (contains all the code)
    - aggregate_stats.py 
    - eda.py 
    - EDA.ipynb
    - Helper Files (contains helper files to run the notebook)
    - player_stats_for_match.py
    - CSVs: output csv files after running scripts

-   data (2 csv files) (Contains the dataset imported from Kaggle: https://www.kaggle.com/manasgarg/ipl) 
    - deliveries.csv
    - matches.csv


# Code and Instructions to run

NOTE - If the code throws an error, "package not found", please pip install the respective packages.

Visualization (for exploratory data analysis)

0. Enter into the directory "codebase"

1. Run the Jupyter Notebook EDA.ipynb
	- to generate visualizations for our Exploratory Data Analysis

2. (Optional) Run the python file eda.py
	- generates an output dir 'generated_plots' containing the visualizations (same plots as step 1) 

# Player statistics

3. Run aggregate_stats.py
	- generates player_stats.csv in CSVs dir containing player stats (e.g runs scored , no of wickets taken etc..) 

4. Run player_stats_for_match.py 
	- generates player rewards for four teams after simulating on the test data (matches in 2017) 

# Team Prediction and Evaluation

  We will Run Super11.ipynb on Google Collab . (We avoid local execution and run on Google Collab as our code uses recent version of GLPK package , that is not compatible with Windows)

5. Zip the folder "CSVs" and "Helper Files"

6. Open Google colab on the browser and upload the file 'Super_11.ipynb'

7. Next, on the left pane go to File -> upload and select the zip files "CSVs.zip" and "Helper_Files.zip"
	- CSVs.zip contains data about player statistics, each player's cost, and match details as well. Helper_Files.zip contain utility python files used by the Super_11.ipynb notebook.

8. Click on Runtime -> Run all.
	- It will run both the cells in Super_11.ipynb. The first cell unzips CSVs.zip and Helper_Files.zip. The second cell computes and outputs the Predicted Team, Optimal Team 
	  and result plots for the selected match. It takes about 20 seconds to run.

9. To run code for any match , select from the drop down and run ONLY the second cell.
	- (Running the first cell again will generate prompts for replacing the already existing files, which is unnecessary effort) 

10. The results are displayed in the Google Colab Console. You can analyze the final ouput (Feel free to select different matches to generate results) 


Note: In case you want to reset the entire environment to re-analyse the project (or any potential errors while following these steps), click Runtime -> Reset all runtimes.
      Now again follow the steps 7-10. 


#### All the files and folders included in the CODE folder are absolutely necessary to replicate results.













