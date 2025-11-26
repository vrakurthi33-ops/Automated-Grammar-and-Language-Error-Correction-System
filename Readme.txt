 Automated Grammar and Language Error Correction System

 Team Number:ÊTeam-8
 Course:ÊAIT 526 - Natural Language Processing, Section 001
 Professor:ÊDuoduo Liao
Team Members
1. Sai Avinash Polina
2. Chandana Gangaraju
3. Akshitha Komatireddy
4. Venkatesh Rakurthi

Project Overview

Problem Statement
Develop an advanced automated system for detecting and correcting grammatical errors in English sentences, leveraging state-of-the-art transformer models.
Approach
The project utilizes two powerful transformer models for grammar correction:
 T5 (Text-to-Text Transfer Transformer)
 BART (Bidirectional and Auto-Regressive Transformer)
Primary Model:ÊT5 was selected as the primary implementation due to its superior performance and versatility in sequence-to-sequence tasks.
Key Features
1. Grammar Correction
 Real-time detection and correction of grammatical errors
 Supports multiple transformer models (T5 and BART)
 Advanced text generation techniques
2. Intelligent Feedback Generation
 Detailed grammatical feedback using OpenAI's GPT-3.5 API
 Comprehensive error analysis and improvement suggestions
3. Model Performance Evaluation
 Comparative analysis of T5 and BART models
 GLEU (Generalized Language Evaluation Understanding) score assessment
4. Interactive User Interface
 Command-line interface for sentence correction
 Option to receive detailed grammatical feedback

Technical Specifications

Datasets
 Primary Dataset:ÊJFLEG (Johns Hopkins Fluency-Extended GEC Dataset)
 Used for fine-tuning T5 and BART models

Models
1. T5 (Base Model)
o Text-to-text transformer for sequence generation
o Optimized for grammar correction tasks
o State-of-the-art performance in sequence generation
2. BART (Base Model)
o Bidirectional transformer
o Used for comparative model analysis

Evaluation Metric

 GLEU Score:ÊMeasures grammatical correctness and sentence fluency

Technology Stack

Tools & Libraries
 Machine Learning Framework:ÊPyTorch
 NLP Libraries:
 Hugging Face Transformers
 Hugging Face Datasets
 NLTK
 API Integration:ÊOpenAI GPT API
 Programming Language:ÊPython

 System Requirements

 Hardware
- CUDA-enabled GPU (recommended)
- Minimum 16GB RAM
- Python 3.8+

 Dependencies
- torch
- transformers
- datasets
- nltk
- matplotlib
- wordcloud
- openai
- pandas

 
 Usage

 Training Models
The script automatically handles:
- Dataset loading and preprocessing
- Model fine-tuning
- Performance evaluation

 Evaluation Metrics
- GLEU score calculation
- Comparative performance analysis between T5 and BART models

 Limitations and Considerations
- Requires stable internet connection
- OpenAI API usage incurs potential costs
- Performance varies based on input complexity
- Fine-tuning requires significant computational resources

 Future Improvements
- Expand training dataset
- Implement more advanced sampling techniques
- Integrate additional language models
- Develop a web/desktop application interface



Dataset:
We used the JFLEG dataset,
 The JFLEG (JHU Fluency-Extended GUG) corpus is a benchmark for English grammatical error correction (GEC) systems. It serves as a gold standard for evaluating and developing GEC systems based on fluency (how natural the text sounds) and grammatical correctness. Each source document in the corpus includes four human-generated corrections.

Link to dataset : https://huggingface.co/datasets/jhu-clsp/jfleg

Examples of input and outputs:

1.
Original Sentence: i have an idea to visit the europe next summer.
Corrected Sentence (T5): I have an idea to visit Europe next summer.
Feedback: The sentence 'I have an idea to visit Europe next summer.' is grammatically correct. Here are the elements in focus:

- Incorrect use of articles: The sentence is accurately using the article 'an' before 'idea,' which is a singular, non-specific countable noun. Moreover, 'Europe' usually does not take an article, which is correct here.
   
- Subject-verb agreement: The subject 'I' correctly matches with the verb 'have.' It is correct for singular first-person use.

- Tense consistency: The sentence remains in the present tense throughout ('I have an idea'), and there is no change of tense that could cause inconsistency.

- Preposition misuse: There are no prepositions misused in this sentence. 'To' correctly indicates direction or intended result in the context it is used in the sentence.


2.
Original Sentence: he is a honest person.
Corrected Sentence (T5): He is an honest person.
Feedback: The sentence 'He is an honest person.' is grammatically correct considering all the factors you've listed.

- Regarding the use of articles: The indefinite article 'an' is correctly used before 'honest', which starts with a vowel sound.
- Regarding subject-verb agreement: The singular subject 'He' correctly matches the third person singular form 'is'. 
- Regarding tense consistency: The sentence is in the present tense all throughout, making it consistent.
- Regarding preposition misuse: There are no prepositions used in this sentence, therefore, there is no misuse. 

This sentence doesn't require any improvements as it is perfectly correct in its current form.

3.

Enter an incorrect sentence (or type 'exit' to quit): she was cooking and eat.
Original Sentence: she was cooking and eat.
Corrected Sentence (T5): She was cooking and eating.
Feedback: The sentence 'She was cooking and eating.' is grammatically correct. Here's the analysis based on your description:

- Incorrect use of articles: The sentence does not require the use of any articles (a, an, the). Therefore, there are no errors in this category.
- Subject-verb agreement: The subject 'She' properly agrees with the verb 'was cooking' and 'eating'. Both actions refer to the same subject which is singular.
- Tense consistency: The sentence is consistent in the past continuous tense; 'was cooking' and 'eating' both suggest ongoing actions in the past.
- Preposition misuse: There are no prepositions in this sentence, hence there's no misuse.

There are no suggestions for improvement because the sentence is grammatically accurate. It correctly presents two activities that were occurring at the same time in the past.
================================================================================
Enter an incorrect sentence (or type 'exit' to quit): exit
Exiting the interactive prompt.
