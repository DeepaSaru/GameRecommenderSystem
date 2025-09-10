Building a Recommender System with Steam Dataset

In this task, we will work with a dataset extracted from Steam, an online video game distribution platform. 
The dataset is provided as steam-200k.csv and contains information about members’ purchase and play behaviors.

The dataset has four columns:

    Column 1: Unique identifier for each member
    Column 2: Name of the game purchased or played
    Column 3: Member behavior — either purchase or play
    Column 4: Value = 1 if the behavior is purchase; if play, the value corresponds to the number of hours played

Because games must be purchased before they can be played, some member–game combinations have multiple entries. 
Both purchase and play behaviors can be treated as implicit feedback, making this dataset suitable for recommender system training.

Our tasks:

  1. Load & Explore the Dataset
  2. Load the dataset into a Spark DataFrame.
  3. Optionally perform exploratory analysis using Spark SQL, DataFrames, Databricks visualizations, or other visualization libraries.
  4. Train a Recommender System
  5. Use MLlib to train a collaborative filtering model (ALS matrix factorization).
  6. Carry out preprocessing steps such as train/test splitting.
  7. Decide whether to include both purchase and play behaviors or only one — and experiment with different approaches.
  8. Generate & Evaluate Recommendations
  9. Evaluate the model’s performance.
  10.Explore and present some of the resulting recommendations.

Important Note:

ALS in MLlib requires integer IDs for both users and items. Since the dataset does not provide IDs for games, you will need to generate unique integer IDs for each game.

You may use the additional file games.csv, but higher marks will be awarded if you generate IDs programmatically within Databricks instead of relying on the extra file.
