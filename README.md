# Capstone_Project

I created a capstone project with python using machine learning to help predict future tennis match outcomes by taking data from the past 10 years. 
I collected the data from http://tennis-data.co.uk/alldata.php. 

I downloaded spreadsheets that are separated by each of the past 10 years and merged them all into one 
spreadsheet.

To perform the machine learning, I created an algorithm by first reviewing the outcome of each match. The spreadsheets presents the winner and loser of each match. 
Since the outcomes are already known, in order to remove biasness, I created a third column with a binary outcome.

If the player in the winner column's last name comes alphabetically before the player in the loser column, this binary column gets a 0.

If the player in the loser column's last name comes alphabetically before the player in the winner column, this binary column gets a 1.

The point was to have an arbitrary result between winners and losers. Turned out a balanced classification of the results came back 50/50. From there, I trained the
algorithm to review data such as the player's ranking, betting odds and player points to figure out who the accurate winner was in each match.

I used random forest models, decision trees and KNN models find the percentage of times the algorithm could accurate get correct winner of each match. These models
were accurate around 65%-70% of the time. 

To increase accuracy, I could add more years to the data. Fine tuning the hyperparameters of the other classifiers and adding more feature engineering could improve
the quality of predictions as well.

