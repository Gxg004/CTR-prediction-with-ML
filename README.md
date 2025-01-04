# CTR-prediction-with-ML
GCN model has been for both Regression and Classification on 2 different datasets to
 test its ability. Regression was performed on the Facebook-ad-campaigns dataset from
 kaggle while Binary classification was performed on Avazu dataset.
  The preprocessing steps focus on preparing a large dataset for efficient machine learn
ing. First, the data was initially reduced by taking a small sample of the original, which
 makes handling and processing quicker and more manageable. Key features were then
 engineered from existing columns, such as extracting specific time-related elements (hour
 of day and day of month) from a general timestamp. This allows the model to potentially
 learn patterns based on time-related user behavior. Following this, only a subset of rele
vant features was selected, ensuring the dataset includes only the information most likely
 to impact predictions, which minimizes noise and reduces the size of the dataset further.
 Additionally, the Facebook Ad Campaign dataset was used, with a separate CTR feature
 column calculated as (clicks / impressions) * 100. We normalized the dataset features
 using Min-Max scaling for consistent input across the model layers.
 Next, categorical features, such as user and app identifiers, were transformed into a
 numerical format to enable them to be used in a machine learning model, ensuring all
 data is in a consistent, usable structure. Finally, the data was organized into separate
 inputs and target labels, ready for training. This process results in a streamlined, efficient
 dataset that preserves meaningful information, reduces computational complexity, and
 optimizes it for accurate model learning and evaluation.
 Architecture: 
  For regression, The GCN model was initially trained on a 50/50 data split for computa
tional feasibility, using an increased model complexity to better capture the relationships
 within the graph structure. The training process involved forward and backward passes
 through the network with the Mean Squared Error (MSE) as the primary loss metric. In
 the context of this project, which aims to predict click-through rates using graph-based
 machine learning techniques, the code implements a method for constructing a sparse
 graph from the dataset. 
 For classification, the model’s performance was evaluated on a validation set using AUC, log loss, and
 accuracy. These metrics were tracked over epochs to visualize learning trends and assess
 model effectiveness. During the training process of the Enhanced GCN model, the loss
 values exhibited a general trend of improvement, indicating the model’s ability to learn
 from the training data.

 
