# Transformer-QA-Pipeline-Sentiment-Analysis

•	Part One (Context based response) – It tackles the need of first parameter which is “Issue Identification” defined by the question ‘Did the employee understand customer requirements?’ Here, we have used ‘transformers question-answer’ pipeline using 2 different models ('DistilBertForQuestionAnswering' and ‘bert-large-uncased-whole-word-masking-finetuned-squad’) to identify if the response provided is as per the context / query received from customer. If the model can throw a score & answer, we consider it as a contextual answer otherwise we treat it as not a direct answer to the customer query and hence would require manual intervention and understanding.

•	Part Two (Sentiment Analysis) – This part tackles the question of ‘Did the employee display courteousness / empathy?’ while responding to customer query. Here we have used ‘transformers sentiment-analysis’ pipeline using the pre-trained model ‘distilbert-base-uncased-finetuned-sst-2-english’. However, one noticeable limitation of this approach is repeated use of negative words like ‘not’, ‘no’, ‘cannot’, and ‘unable’ in one sentence can give a different result. 
