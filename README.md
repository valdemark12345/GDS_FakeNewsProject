# GDS FakeNewsProject
Students: Lasse Helmer Larsen (rmj762), Oskar Thorvald Andersen (grf587) og Valdemar Kragh (lnk952)

To get our environment use:
```
conda env create -f environment.yml
```
This will install all needed dependencies and provide a kernel that can be used to run our code.

### If something is updated in the venv, we should use to update:

conda env export > environment.yml

### After pulling, to update the environment use:

conda env update -f environment.yml --prune

Before running our code, ensure that the file '995,000_rows.csv' from the fake news corpus is in your working repository.  

In order to run our code, first run the notebook Code_2_processing_chunks.ipynb this will apply our processing pipeline to the data and create parquet files with chunks of 10000 rows (you should have 100 chunk files). https://absalon.ku.dk/courses/89126/files/10468050?wrap=1

To train and run our simple logistic model go to code logistic and run all cells. This will train on all the chunks created in the previous step.

To get the word embeddings for the model trained on distilbert and look at the kaggle code https://www.kaggle.com/code/lassehelmer/bert-binary. Afterwards to look at the gradient boosting model and the evaluation on the liar dataset, look at https://www.kaggle.com/code/lassehelmer/bert-binary-gb . We do not recommend running the code on your own machine, as extracting the embeddings took upwards of 9 hours.



