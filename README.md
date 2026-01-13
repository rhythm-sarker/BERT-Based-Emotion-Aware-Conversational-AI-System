This project implements an intelligent chatbot that moves beyond simple keyword matching by utilizing Natural Language Processing (NLP) to understand the emotional sentiment behind user inputs. Built on top of the Hugging Face Transformers library, this application fine-tunes a pre-trained BERT (Bidirectional Encoder Representations from Transformers) model to classify text into specific emotional categories and deliver appropriate, empathetic responses in real-time.

Key Features

Emotion Classification: Accurately categorizes user input into four distinct labels: happy, sad, angry, and neutral.

State-of-the-Art NLP: Utilizes bert-base-uncased for deep contextual understanding of language.

Confidence Scoring: The chatbot displays the model's confidence score alongside its prediction to ensure transparency in the AI's decision-making process.

Dynamic Response System: Maps predicted emotions to pre-defined empathetic responses (e.g., offering comfort for sadness, sharing joy for happiness).

Technical Implementation The project follows a rigorous machine learning pipeline:

Data Preprocessing: Tokenization using BertTokenizer with dynamic padding and truncation to a max length of 64.

Model Training: Fine-tuning the BERT model using the Hugging Face Trainer API over 5 epochs.

Evaluation: Metrics include Accuracy and Weighted F1-Score to ensure balanced performance across classes.

Deployment: A persistent CLI loop that saves the trained model and label encoders for inference.
