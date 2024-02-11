# SLIM-Models-by-LLMWare
SLIM Models by LLMWare. A streamlit app showing the capabilities for AI Agents and Function Calls.


![alt text](https://github.com/yashraj-96/Small-Language-Models-LLMware/blob/main/repo_pic.jpg)

Script [ app.py ]

The provided code is a Streamlit web application that allows users to input text and select various language analysis tools to apply to the text. After clicking the "Analyze" button, the selected tools are executed, and the results are displayed in JSON format.

In summary:

1. The code sets up a Streamlit app with a title and a text input field.
2. Users can select multiple language analysis tools using a multiselect widget.
3. When the "Analyze" button is clicked, the selected tools are executed on the input text, and the results are displayed in JSON format.

This application is designed to interact with the "llmware_module," which presumably contains functions for sentiment analysis, emotion detection, tag generation, topic identification, intent analysis, ratings retrieval, category extraction, named entity recognition (NER), and natural language inference (NLI).


Script [llmware_module.py]

This code defines a set of functions that perform various natural language processing tasks using models from the "llmware" library. Here's an explanation of each function:

classify_sentiment(text): Loads a sentiment analysis model named "slim-sentiment-tool" from the ModelCatalog and applies it to the input text. The result is returned.

detect_emotions(text): Loads an emotion detection model named "slim-emotions-tool" from the ModelCatalog and applies it to the input text. The result is returned.

generate_tags(text): Loads a tag generation model named "slim-tags-tool" from the ModelCatalog and applies it to the input text. The result is returned.

identify_topics(text): Loads a topic identification model named "slim-topics-tool" from the ModelCatalog and applies it to the input text. The result is returned.

perform_intent(text): Loads an intent analysis model named "slim-intent-tool" from the ModelCatalog and applies it to the input text. The result is returned.

get_ratings(text): Loads a ratings retrieval model named "slim-ratings-tool" from the ModelCatalog and applies it to the input text. The result is returned.

get_category(text): Loads a category extraction model named "slim-category-tool" from the ModelCatalog and applies it to the input text. The result is returned.

perform_ner(text): Loads a named entity recognition (NER) model named "slim-ner-tool" from the ModelCatalog and applies it to the input text. The result is returned.

perform_nli(text): Loads a natural language inference (NLI) model named "slim-nli-tool" from the ModelCatalog and applies it to the input text. The result is returned.

Each function follows a similar structure: it loads a specific pre-trained model from the ModelCatalog and then applies that model to the provided text using the function_call method. The get_logits=False argument suggests that the functions are not requesting the raw model logits but rather the processed output. The processed output, which includes the results of the respective natural language processing tasks, is then returned.

------------------------------------------------------------------------------------------------------------------------------------

To run the application, clone the repository, navigate to the cloned library and run the below command:

streamlit run app.py

