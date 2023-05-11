![Neo4j-logo_color](https://github.com/alexoliveros92/Collaboration_prediction/assets/108631269/522386c8-0d72-4b40-bf1b-4d92a006da96)

# Relationship prediction in Neo4j (Graph Analysis)

* Objective: use graph features to predict future collaboration between actors based on previous collaboration.

* 4 models are trained and tested using different set of graph features.

* The last section presents the importance of each of the features used on the prediction performance.

* The graph parameters used are: Common neighbors, preferential attachment, total neighbors, triangles count, clustering coefficient, Louvain coefficient, and partition community detection.

## Installation

Neoj4 configuration
To interact with Neo4j, you need a Sandbox Neo4j. For this project, I am using the Neo4j desktop version and running the sandbox in my localhost browser, you can install Neo4j following the instruction in this [link](https://neo4j.com/download/). An online sandbox can be launched for 3 days [here](https://neo4j.com/sandbox/), you just have to sign in. In this notebook, I am connecting with my localhost running Neo4j installed in my desktop.

**Steps to connect Neo4j desktop and Jupiter notebook:**

* Run the neo4j desktop app
* Create a new project (+new button)
* Within the project, create a new Graph DBMS (+add button)
* Select the 'Local DBMS' option in the menu
* When creating the Graph DBMS, select a password and write it down as you will need it later.
* This notebook is using the 5.3.0 neo4j version 5.3.0
* Once created, click it to open the option toolbar on the right hand side, select the Plugins option and install APOC and Graph Data Science Library
* Then, click on the three dots next to the open button, and select settings
* Go to the button of the text file and change the memory.heap.max_size by 6G

![eeee](https://github.com/alexoliveros92/Collaboration_prediction/assets/108631269/fc88ebef-24c8-4247-826e-21e4ed7dfd8d)

### Import the dataset to Neo4j

To import the dataset to neo4j first:

* Open the import folder
![zzz](https://github.com/alexoliveros92/Collaboration_prediction/assets/108631269/e434ebca-b763-418e-88d4-5e41150c57e3)

* Copy and past the dataset in the import folder
* Press the start button to run the neo4j sandbox
* When running, you will receive a notification that the process was successful
* Finally, open the virtual sandbox by selecting the open button and Neo4j Browser option.
* At this point, you should have neo4j running in your localhost and ready to start coding in your notebook

This is the last step in neo4j. The rest of the code is in Jupyter Notebook, you can find the code and explanations [here](https://github.com/alexoliveros92/Collaboration_prediction/blob/main/relationship-prediction-in-neo4j-graph-analysis.ipynb).

## Usage

The algorithm predicts the relationships between a pair of nodes based on their behaviour and relationship with other nodes within the net. We could, for example, predict the interaction between two strangers based on their behaviour and relationships in a social network, or in the case explored in the notebook, the possibility of a future collaboration between two actors based on the cast of their previous film.

## Acknowledgment

Note: this paper is based on the notebook ‘Analyze netflix data using graphs (neo4j)’ published by [Yann Claudel.](https://www.kaggle.com/code/yclaudel/analyze-netflix-data-using-graphs-neo4j)

## License
This Notebook has been released under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) open source license.
