# Analyzing Effects of Aspect Features on Bert Performance on SentimentClassification on Financial Microblog and Headlines Dataset
we plan to leverage Bert for aspect-based sentiment classification, using data presented as subtask I of Financial Opinion Mining and Question Answering Open Challenge. We will focus on two questions:
1. How does different levels of aspect data influence the performance in the Bert model?
2. How does aspect data helps in sentiment classification?

We will first provide a comparative study using different methods of feeding the sentence and aspect data into different models. And then study the effect by manipulating the input with random, noisy aspect data, and study its effect.

## Basic Setup and Data Preprocessing
We follow the instruction after building up transformers and run the example on prince. After downloading data, we modify data by running [data_preprossessing.ipynb](data/data_preprossessing.ipynb) to feed in bert model under transformers. After the modification, the training data should look like in this form:
>{'question': 'Royal Mail chairman Donald Brydon set to step down', 'passage': 'Corporate/Appointment', 'idx': 0, 'label': '0'}

## Running the Program
We modify the code mainly by modifying code offered in the course Machine Learning for Language Understanding at NYU. Thus we are unable to provide the full code. By using the Transformer library with small small changes and sbatch files we archived in the sbatch folder, the result can be regenerated. Please contact us at yd1158@nyu.edu if you need more clarification.
In the archived sbatch file, the files are named in the format of <index>_<aspects_used>_as_<model_name>_<randomized>.sbatch

## Results
Results are in the paper MLLU_Final_Paper_Yuhao&Oscar.pdf
