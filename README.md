#### Vahid Mousavinezhad

Named Entity Recognition (NER) is a crucial NLP task that identifies and classifies named entities in text, including names, organizations, locations, and more. It plays a vital role in various applications like information retrieval, question answering, translation, sentiment analysis, and summarization. The main objective of NER is to precisely recognize and categorize named entities present in a text. This process entails two essential steps: detecting the boundaries of the entities, which involves identifying the starting and ending positions of the named entities and classifying the entities by assigning a predetermined label or category to each one. For example, in the sentence "Elon Musk has a plan to go to Mars." NER would classify "Elon Musk" as a person and "Mars" as a location.


NER is important because it enables machines to understand and extract meaningful information from unstructured text. By identifying named entities, NER helps in organizing and structuring textual data, which can be further used for various downstream tasks. For example, in information retrieval systems, NER can improve search results by allowing users to search for specific entities. In question-answering systems, NER helps in identifying the entities relevant to the question. In sentiment analysis, recognizing named entities can provide additional context to determine the sentiment expressed towards them.


Nevertheless, the NER task has several challenges. One major difficulty is that named entities can be ambiguous and vary in different contexts. For example, the word "Jaguar" can refer to an animal or a company. To solve these ambiguities, we need a deep understanding of the context and general knowledge. Additionally, named entities can have complex structures like compound names or nested entities, which makes their detection and classification more difficult. Another challenge in NER is the lack of labeled training data. Annotated datasets are often limited, especially for specialized domains or languages. Collecting and labeling large-scale datasets for NER can be time-consuming and expensive. This scarcity of labeled data can affect the performance of NER models, especially for less common or emerging entities.


In this project, I will explore two approaches for the NER problem: the CRF (Conditional Random Fields)  as a machine learning model and using the Transformers as a deep learning model. I aim to enhance the performance of these models by addressing the challenges they encounter and finding effective solutions.


### References

[1] T. K. Sang, F. Erik, and D. M. Fien, “Introduction to the CoNLL-2003 shared task: Language-independent named entity recognition,” In Proceedings of the Seventh Conference on Natural Language Learning at HLT-NAACL, pages 142–147., 2003.

[2] R. Weischedel, M. Palmer, M. Marcus, E. Hovy, and S. Pradhan, “Ontonotes release 5.0 ldc2013t19,” Web Download. Philadelphia: Linguistic Data Consortium, 2013.

[3] A. Arun, C. Dyer, and P. Koehn, “Monte carlo inference and maximization for phrase-based translation.,” In Proceedings of the Thirteenth Conference on Computational Natural Language Learning, pages 102–110, 2009.

[4] J. Laﬀerty, A. McCallum, and F. Pereira, “Conditional random felds: Probabilistic models for segmenting and labeling sequence data.,” In Proceedings of the 18th International Conference on Machine Learning (ICML), pp. 282-289), 2001.

[5] V. Singh, “Named entity recognition using transformers and data from conll 2003 shared task.,” Keras Documentation, 2021
