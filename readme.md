Spacy provides an exceptionally efficient statistical system for NER in python, which can assign labels to groups of tokens which are contiguous. It provides a default model which can recognize a wide range of named or numerical entities, which include person, organization, language, event etc. Apart from these default entities, spaCy also gives us the liberty to add arbitrary classes to the NER model, by training the model to update it with newer trained examples.

1 Convert speech to Text transformer Wav2Vec2 module and model is used is 'facebook/wav2vec2-large-960h' and torach library to decode the text,  Wav2Vec models are available in the Hugging Face model repository. You can load a pre-trained Wav2Vec model using the transformers library.
2 Load the model spacy.load('en') --> Disable existing pipe line (nlp.disable_pipes) 1.2. spacy.blank('en') --> Added Entity Recognizer to Pipeline, 
3 Shuffle and loop over the examples --> update the model (nlp.update) , The nlp.update function in SpaCy is used to update the model's parameters and improve its performance by training it on custom data
4 Save the trained model (nlp.to_disk)
5 Test on transcript of audio file

libraries used speech to text conversion :-
transformers, soundfile, torch

libraries used for training :-
Spacy
