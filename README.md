# AiQuizeCraft

AiQuizeCraft is an AI-powered tool developed as part of the TNSDC learning program, designed to assist learners in generating multiple-choice questions (MCQs) from textual content. Leveraging advanced natural language processing techniques such as BERT Extractive Summarization, WordNet, and ConceptNet, AiQuizeCraft analyzes given texts or articles to create comprehensive sets of MCQs that evaluate comprehension and reinforce learning.

## Features

- **Text Analysis**: AiQuizeCraft utilizes BERT Extractive Summarization to understand the main ideas and key points within the provided text.
- **Semantic Understanding**: The system leverages WordNet and ConceptNet to comprehend the semantic relationships between words, enhancing the accuracy of question generation.
- **MCQ Generation**: Based on the analyzed text, AiQuizeCraft formulates diverse sets of multiple-choice questions covering various aspects of the content.
- **Customization**: Users can adjust parameters and settings to tailor the generated MCQs according to their preferences and specific learning objectives.
- **Scalability**: AiQuizeCraft is designed to handle a wide range of textual inputs, making it suitable for educational content creation across different domains and levels of complexity.

## Installation

1. Clone the repository: `git clone https://github.com/TNSDC/AiQuizeCraft.git`
2. Navigate to the project directory: `cd AiQuizeCraft`
3. Install dependencies: `pip install -r requirements.txt`

## Usage

1. Import the `aiquizecraft` module into your Python environment.
2. Use the provided functions to analyze textual content and generate MCQs.
3. Customize settings and parameters as needed to fine-tune the question generation process.

```python
from aiquizecraft import AiQuizeCraft

# Initialize AiQuizeCraft
aiquizecraft = AiQuizeCraft()

# Analyze text and generate MCQs
text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit..."
mcqs = aiquizecraft.generate_mcqs(text)

# Print generated MCQs
for question, options, answer in mcqs:
    print("Question:", question)
    print("Options:", options)
    print("Answer:", answer)
    print()
