# NLP-Unsupervised-Learning

![Process](https://github.com/user-attachments/assets/55903eb5-e71f-4f87-91ae-396a15f93249)


- The organization which collects this data is focused on Improving decisions and getting better results with the Simulation tool built 
- The simulation played by the client's employees would capture several aspects of the individuals which serve as inputs to understand the overall organizational culture 
- The simulation tool built in collates the inputs from the end users(usually client’s employees) and presents several reports 
- The project assigned to me would be to optimize one of these reports as part of the tool
- The focus of the analysis is to classify each user into 4 Quadrants based on the inputs 
- One Axis measures a candidate’s Competitiveness vs Collaborativeness
- Another Axis measures the same person’s Stability vs Change focus approach 
- Each individual is different and the overall picture of where the test takers lie on this graph, represents the working style of the employees and would serve as a reality check if the organization’s target approach is on the right path


Axis Projection Steps:

All the words inputted by users were considered as corpus 
The redundant and the stop words were cleaned
The cleaned words were mapped with definitions from Cymorg Team 
The words which had a match were retained 
The words which did not have a text match were mapped using the best Fuzzy Score 
Then the Glove Score from is normalized per words used 
X and Y coordinates are calculated and projected  


Clustering Steps:

Utilizes the cleaning and Word Embedding of the 'Axis Projection' Step
Avg. of the Glove vector is utilized understand a user vector in the 50 dimensional glove vector space
Then the Euclidean distance helps us to actually identify the user's distance from the origin 
This distance is used as an input for the clustering
DBScan, K-Means aren' published in the Notebook(As they were already within the system)
Heirarchical Clusterig was done to test the data to see new clusters 


FInal Takeaways:

The 2 outputs we had should go hand in hand to identify clusters and user patters


