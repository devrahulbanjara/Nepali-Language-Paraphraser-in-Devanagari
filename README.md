# Nepali Language Paraphraser in Devanagari

## Introduction
The **Nepali Language Paraphraser** is a state-of-the-art platform designed to generate contextually accurate paraphrases of text written in the Devanagari script. Leveraging Transformer-based models and Natural Language Processing (NLP) techniques, the system can process Nepali text to produce varied and meaningful paraphrases. The platform includes a user-friendly interface for easy text input and output.

## Goals
- **Contextual Paraphrasing**: Utilize advanced NLP models to generate contextually relevant paraphrases of Nepali text.
- **User-Friendly Interface**: Provide an intuitive interface for users to input text and receive paraphrased results.
- **Model Performance**: Ensure high-quality paraphrasing through the use of Transformer-based models.
- **Scalable Infrastructure**: Design the system to handle increasing user demands while maintaining performance.

## Contributors
- **Rahul Dev Banjara**
- **Shubham Raj Joshi**

## Project Architecture
1. **Frontend**:  
   - Provides a simple interface for users to input Nepali text and view paraphrased results.
   - **Text Input**: Users can enter Nepali text in Devanagari script.
   - **Paraphrasing Output**: Displays the paraphrased version of the input text.

2. **Backend**:  
   - Handles core functionalities such as text processing, model inference, and response generation.
   - **Text Processing**: Manages the input text and prepares it for the Transformer model.
   - **Model Inference**: Utilizes pre-trained Transformer models to generate paraphrases.
   - **Response Generation**: Formats and delivers the paraphrased text to the frontend.

3. **Model Training**:  
   - **Transformer-Based Models**: Implements models fine-tuned for Nepali paraphrasing tasks.
   - **Training Data**: Uses a dataset of Nepali text for model training and evaluation.

4. **Security Layer**:  
   - Ensures data privacy and secure access to the application.

## Status

### Known Issues
- **Model Accuracy**: The quality of paraphrases may vary with complex or ambiguous input texts.
- **Resource Consumption**: High computational requirements for Transformer models might impact performance.

### High-Level Next Steps
1. **Model Enhancement**: Improve model accuracy and handle more complex paraphrasing scenarios.
2. **Performance Optimization**: Optimize system performance to handle higher loads and reduce latency.
3. **User Feedback Integration**: Collect and integrate user feedback to enhance the system's usability and functionality.
4. **Additional Features**: Explore adding more features, such as language style customization or contextual adjustments.


# Usage
## Installation
To begin this project, use the included `Makefile`

#### Creating Virtual Environment

This package is built using `python-3.10`. 
We recommend creating a virtual environment and using a matching version to ensure compatibility.

#### pre-commit

`pre-commit` will automatically format and lint your code. You can install using this by using
`make use-pre-commit`. It will take effect on your next `git commit`

#### pip-tools

The method of managing dependencies in this package is using `pip-tools`. To begin, run `make use-pip-tools` to install. 

Then when adding a new package requirement, update the `requirements.in` file with 
the package name. You can include a specific version if desired but it is not necessary. 

To install and use the new dependency you can run `make deps-install` or equivalently `make`

If you have other packages installed in the environment that are no longer needed, you can you `make deps-sync` to ensure that your current development environment matches the `requirements` files. 

## Usage Instructions


# Data Source
## Code Structure
## Artifacts Location

# Results
## Metrics Used
## Evaluation Results
