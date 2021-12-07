# Intent-Recognition-Using-BERT

## Intent Recognition
Voice user interfaces (e.g. Amazon Alexa, chatbots, and social robots) are becoming an essential part of everyday life. For these systems to carry out effective dialogue, they must be able to determine the intent behind a user’s spoken utterance. Intent recognition is the task of taking a written or spoken input, and determining which of several classes it matches in order to best respond or guide the interaction. Effective intent recognition is essential to building many kinds of conversational technologies, from chatbots, to automated phone systems, to social robots. In this notebook, you'll train an intent recognition model, and will explore how the amount of training data used effects performance.

## The Snips Dataset
For our intent recognition model, we'll use the Snips dataset, which was collected through crowdsourcing for the Snips personal voice assistant. There are 7 unique intent classes for the training set, on a variety of topics including playing music, restaurant reservations, and getting the weather (e.g. ‘Book an Italian place with a parking for my grand father and I’ and ‘Which movie theater is playing The Good Will Hunting nearby?’). The training set contains 13,084 utterances, and separate validation and test sets that contain 700 utterances each.
