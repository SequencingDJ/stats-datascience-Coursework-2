This repo is for Statistics and Data Science - Coursework 2. 
For Birkbeck Collge, University of London. 

Datasets have been merged:
The pkas dataset and their sequences have been obtained, from their pdb ids.

Initially planned to have 10k sequences, we instead have a merged total of 9962 (unique ids).
The remaining discarded sequences would require additional data cleaning but this was deemed unimportant.

We will therefore use the following ML ratio of:  
Testing:Training  
7:3  
6973:2989  


Next steps: 
- Assign which uniqueIDs will go into training/testing
- Figure out method to specify POSITIONS of residue for calculation of pkas.
- Build ML model.
- Evaluate ML model.
- Possible refinement of model.

- Interactive dashboard to visualise results? (stretch goal)




Reminder of the criteria for marking:  
• <del>Acquire data  
• <del>Parse data  
• <del>Write a ‘clean’ dataset  
• Make a classifier or a regressor  
• Train it  
• Predict values with it  
• Visualise the results  
• Remember code should be commented. 



Specifying positions:
Will first use one hot encoding to specify positions. Using a windowed frame or slice of the sequence, to then give that to the model. 