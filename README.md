# EmoSumm

The goals of this paper are: (1) can we use LLMs like GPT-4/Chat GPT to generate synthetic data for the emotion disgust and (2) can we fine-tune BART and T-5 models on this data along with the original COVIDET dataset for the task of emotion trigger summarization? We experiment with prompt-engineering strategies. We then test these strategies against each other and analyze the resulting performance of the BART and T-5 models. We compare the model performance with and without the additional LLM-generated dataset.

1. The data generation using GPT is in the GPT_DataGeneration.ipynb file. This file includes the prompting and usage of the Open AI API to generate Reddit posts and summaries.
2. The main code for loading the data, tokenizing the data, and training BART on this data is in emotion_summarization.py.
3. The BART_and_T5_TrainingModel.ipynb is the notebook that loads the data and then calls emotion_summarization.py to generate the results.
   Note: The train_bart_model.ipynb is the same as the BART_and_T5_TrainingModel.ipynb but just without the T5 results.
