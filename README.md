## Training a QA model using Facebook's Babi Dataset for Single Supporting Fact.

- Read and parse the stories in the bAbi task format from the downloaded file.
- Vectorize the Story, Query and Answer and add padding.
- Embedd the Input Sequence and Question into a sequence of vectors.
- After all RNN is used.
- RMSProp optimizer is used and loss function is categorical_crossentropy.
- Model is fit on the training and validation context, question and answers.
- We pass in plot callbacks to see how training cost and validation cost varies as the
   number of epochs increases.
- Model is saved and then loaded and our test examples are vectorized and passed to the
   model to predict the answer for the question.

#### Below is an example:

**Story:** Daniel went back to the hallway .
Mary went back to the office .

**Question:** Where is Mary ?

**Original Ans:** office

**Predicted Ans:** office

References:
https://towardsdatascience.com/building-an-ai-chat-bot-e3a05aa3e75f

