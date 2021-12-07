# Intent-Recognition-Using-BERT

## Intent Recognition
Voice user interfaces (e.g. Amazon Alexa, chatbots, and social robots) are becoming an essential part of everyday life. For these systems to carry out effective dialogue, they must be able to determine the intent behind a user’s spoken utterance. Intent recognition is the task of taking a written or spoken input, and determining which of several classes it matches in order to best respond or guide the interaction. Effective intent recognition is essential to building many kinds of conversational technologies, from chatbots, to automated phone systems, to social robots. In repository an intent recognition model was built, and experiment on how the amount of training data used effects performance was carried out.

## The Snips Dataset
For our intent recognition model, we'll use the Snips dataset, which was collected through crowdsourcing for the Snips personal voice assistant. 
There are 7 unique intent classes for the training set, on a variety of topics including playing music, restaurant reservations, and getting the weather (e.g. ‘Book an Italian place with a parking for my grand father and I’ and ‘Which movie theater is playing The Good Will Hunting nearby?’).
The training set contains 13,084 utterances, and separate validation and test sets that contain 700 utterances each.


## BERT
For our intent recognition model, we'll use BERT, which is a transformer-based model that has been pre-trained on an enormous amount of English data. Through this pre-training, BERT learns to represent language very effectively, and can then be fine-tuned for a specific task. It is possible to train an entire model end-to-end starting from random model weights, but with BERT, we will start with the pre-trained weights, and then do additional training to adapt BERT to our intent recognition task.

To learn about BERT in more detail, you should watch this [video](https://www.youtube.com/watch?v=xI0HHN5XKDo).
Don't worry if BERT's architecture feels too complex, the key things to takeaway are how it is pre-trained, and how we can fine-tune it for our application.

Before BERT was introduced in 2018, most machine learning models for NLP were trained from scratch. Since then, huge success has been found in many NLP applications by fine-tuning pre-trained models like BERT instead. The other most well-known models that are used in this way are the GPT models (GPT, GPT2, GPT3, and GPT Neo).

We'll use a fantastic package called [Hugging Face](https://huggingface.co/) for our BERT model. Hugging Face has tons of pre-trained BERT models for different applications, among many other great models and datasets. Specifically, we'll be using the [BERT Base Uncased model](https://huggingface.co/bert-base-uncased), which contains 110M parameters, and is pre-trained on both the BookCorpus (800M words) and on English Wikipedia (2,500M words).
