# Project report METL 2023


## 1. Introduction

Named Entity Recognition (NER) is a crucial NLP task that identifies and classifies named entities in text, including names, organizations, locations, and more. It plays a vital role in various applications like information retrieval, question answering, translation, sentiment analysis, and summarization. The main objective of NER is to precisely recognize and categorize named entities present in a text. This process entails two essential steps: detecting the boundaries of the entities, which involves identifying the starting and ending positions of the named entities and classifying the entities by assigning a predetermined label or category to each one. For example, in the sentence "Elon Musk has a plan to go to Mars." NER would classify "Elon Musk" as a person and "Mars" as a location.


NER is important because it enables machines to understand and extract meaningful information from unstructured text. By identifying named entities, NER helps in organizing and structuring textual data, which can be further used for various downstream tasks. For example, in information retrieval systems, NER can improve search results by allowing users to search for specific entities. In question-answering systems, NER helps in identifying the entities relevant to the question. In sentiment analysis, recognizing named entities can provide additional context to determine the sentiment expressed towards them.


Nevertheless, the NER task has several challenges. One major difficulty is that named entities can be ambiguous and vary in different contexts. For example, the word "Jaguar" can refer to an animal or a company. To solve these ambiguities, we need a deep understanding of the context and general knowledge. Additionally, named entities can have complex structures like compound names or nested entities, which makes their detection and classification more difficult. Another challenge in NER is the lack of labeled training data. Annotated datasets are often limited, especially for specialized domains or languages. Collecting and labeling large-scale datasets for NER can be time-consuming and expensive. This scarcity of labeled data can affect the performance of NER models, especially for less common or emerging entities.


In this project, I will explore two approaches for the NER problem: the CRF (Conditional Random Fields)  as a machine learning model and using the Transformers as a deep learning model. I aim to enhance the performance of these models by addressing the challenges they encounter and finding effective solutions. By studying and improving these approaches, I hope to contribute to the advancement of NER technology and its applications in natural language processing. 


## 2. State of the art

To train effective NER models, a high-quality dataset with annotated examples of named entities is essential. The dataset creation process consists of data collection from diverse sources such as news articles, books, and web pages to ensure broad coverage. Clear annotation guidelines are defined, specifying entity types, boundaries, and conventions. Annotators mark the named entities manually or with automated tools, followed by a quality assurance process to ensure accuracy and consistency.

After annotation, the dataset is typically divided into training, validation, and test sets. The training set is used to train the NER model, while the validation set aids in fine-tuning hyperparameters and evaluating model performance. The test set is then employed to assess the model's generalization ability. Several notable NER datasets are widely used in research and development, for instance, CoNLL-2003, OntoNotes, and WikiNER. These datasets serve as invaluable resources for training and evaluating NER models, advancing the field of NLP. Additionally, efforts are being made to create and share larger annotated datasets to train NER models. Crowdsourcing and active learning techniques can help in the efficient collection and labeling of data.

Machine learning and deep learning methods have been extensively explored for NER, each with its own strengths and characteristics. In the Machine Learning Approach, Conditional Random Fields (CRFs) are widely used in NER as probabilistic machine learning models. In this approach, relevant features such as word embeddings, part-of-speech tags, and contextual information are extracted from the input text. These features are then fed into a CRF model, which learns the dependencies between words and their corresponding entity labels. During training, the model is optimized to maximize the likelihood of the observed entity labels given the input features. Once trained, the model can make predictions by decoding the most likely label sequence based on the learned dependencies. The strength of this approach lies in its ability to capture dependencies between neighboring words, enhancing the accuracy of entity recognition.

According to this approach, significant contributions have been made by Lafferty, McCallum, and Pereira in their seminal work. The authors address the limitations of Hidden Markov Models (HMMs) by introducing Conditional Random Fields (CRFs) as a powerful probabilistic modeling framework. They emphasize the ability of CRFs to capture rich dependencies between labels and input features, allowing for the modeling of long-range interactions. The work presents the mathematical formulation of CRFs as exponential models and discusses feature function design, parameter estimation, and regularization techniques. The effectiveness of CRFs is demonstrated through their application in various sequence labeling tasks, including named entity recognition. 

In the Deep Learning Approach, Recurrent Neural Networks (RNNs) and Transformers have shown great promise in NER, particularly with sequential data. In this approach, recurrent neural networks (RNNs), often utilizing Long Short-Term Memory (LSTM) cells, are employed. The input text is tokenized, and each token is represented as a word embedding. These token embeddings are then processed by the LSTM-based RNN, which captures contextual dependencies. The output of the LSTM is fed into a softmax layer to predict the entity labels for each token. Another powerful deep learning architecture, the transformer model, has also gained popularity in NER. Transformers leverage attention mechanisms to capture global dependencies in the input sequence, eliminating the need for recurrent connections. They have achieved remarkable results in various NLP tasks, including NER.

This approach demonstrated in the Keras documentation example, involves tokenizing the input text, encoding labels, and training the BERT model using TensorFlow's Keras API. The trained model can then predict entity labels for new text by assigning the most probable label to each token. By leveraging transformers, known for capturing contextual information and long-range dependencies, this deep learning approach showcases the effectiveness of NER in accurately identifying named entities.



## 3. Your approach (1 pages)

> - define your goal as precise as possible
> - how do you plan to achieve your goal? give a short overview of your project, high-level scenario
> - how did you come up with your plan?  
> - how do you evaluate if your solution works


## 4. Data and methods (3 pages)

> - describe the data sets that you use and explain why 
> - how you organise the collected data
> - what tools you use to solve your problem, how you used them (be very detailed)
> - what steps do you take to evaluate your solution? (be very detailed)


## 5. Evaluation (1.5 page)

> - what is the output of your project?
> - describe all the outcomes of all the tests 
> - include tables and graphs and describe carefully their content


## 6. Interpretation (0.5 page)

> - did you fix the problem? 
> - does your solution work? 


## 7. Discussion (1 page)

> - any unexpected observations?
> - what are the limitations of your solution? 
> - any ideas what could be done differently in the future? 


## 8. Conclusion (0.5 page)

> - synthesis, what do we learn from your project


## 9. References (not included in the page count)


## FEEDBACK 

