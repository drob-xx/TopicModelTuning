# TopicModelTuning
The has code that parrallels the article [Using Metrics to Determine The Right LDA Topic Model Size](https://drob707.medium.com/use-metrics-to-determine-lda-topic-model-size-1a1feaa1ff3c). Users can run the notebook and step-by-step re-create the procedures described in the article.

To run the code presented here, follow this outline (details in the cells below):

1. Download two csv files from the GitHub repository into a directory accessible to the notebook.
1. Download the text DB csv file from Kaggle.
1. Assign the global directory value to the location of the above files.
1. Install the required packages.
1. Execute the imports.
1. Run the cells containing Python function definitions used in the notebook.
1. Generate the six models used in the evaluation. This shold take about 15 minutes on a standard Google Colab account. You can save the models for later use if desired.
1. Run the evaluation code.
1. Download CSV Files

There are three csv files that are needed to run this notebook:

In the GitHub repository:

- ExcludelistDF.csv
- ModelRunMetrics.csv

On [Kaggle](https://www.kaggle.com/datasets/danrobinson707/newsdf)

- NewsDF.csv
- ExcludelistDF is a list of stop words which can be used when building models based on the sample text.

*ModelRunMetrics* are the metrics from 90 runs of the LDA and can be used to re-create and explore the data from the article.

*NewsDF* is a copy of the 30,000 article DB that has both the original text as well as pre-processed versions of the articles. You will need this if you want to run your own models AND if you want to explore the text that the models are built on.

It is recommended that you place all of these files in a location accessible to the Colab notebook and referenced in the DATA_DIR variable
