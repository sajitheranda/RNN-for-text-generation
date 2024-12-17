# Recurrent Neural Networks

## Table of Contents

1. [Project Overview](#project-overview)
2. [Objective](#objective)
3. [Project Tasks](#project-tasks)
   1. [Section 1: Preparing the Vocabulary](#section-1-preparing-the-vocabulary)
   2. [Section 2: Implementing the Autocomplete Model](#section-2-implementing-the-autocomplete-model)
   3. [Section 3: Using and Evaluating the Model](#section-3-using-and-evaluating-the-model)
4. [Installation and Setup](#installation-and-setup)
5. [Running the Project](#running-the-project)
6. [Evaluation and Results](#evaluation-and-results)
7. [Contributions](#contributions)
8. [License](#license)

---

## Project Overview

This project focuses on implementing a Recurrent Neural Network (RNN) model to build an **Autocomplete System**. The system suggests word completions based on partially typed words, such as suggesting "university" or "universal" when the input is "univ". This is achieved using an **LSTM-based RNN** built with **PyTorch**.

The project consists of **10 tasks/questions**. Some tasks involve coding, while others require written answers. All written questions are marked in **blue fonts** in the notebook. Written answers should be added in markdown cells immediately following the respective question.

---

## Objective

The goal is to:
1. Preprocess a vocabulary of **10,000 common English words**.
2. Train an LSTM-based RNN to predict word completions.
3. Experiment with model parameters such as **embedding dimensions**, **hidden layer size**, and **learning rate** to achieve optimal performance.
4. Evaluate the model on partially typed words to analyze its performance.

---

## Project Tasks

### **Section 1: Preparing the Vocabulary**
- Load the wordlist (`wordlist.txt`) containing 10,000 common English words.
- Filter out words shorter than 4 characters and longer than a defined maximum length (`WORD_SIZE`).
- Convert all words to lowercase and pad them to a uniform length using underscores (`_`).

### **Section 2: Implementing the Autocomplete Model**
- Implement an LSTM-based RNN for autocompletion.
- The model consists of:
  - **Embedding Layer**
  - **LSTM Layer**
  - **Fully Connected Layer**
- Implement necessary methods such as:
  - `char_to_num` to convert characters to numbers.
  - `num_to_char` to convert numbers back to characters.
  - `word_to_numlist` and `numlist_to_word` to handle word conversion for training.
- Train the model using **cross-entropy loss** and an **Adam optimizer**.

### **Section 3: Using and Evaluating the Model**
- Train the model on the filtered vocabulary with different parameters like **embedding dimensions**, **hidden layer size**, **learning rate**, and **batch size**.
- Evaluate the model on test inputs such as "univ", "math", "neur", and "engin".
- Comment on the results, including any successful predictions and improvements.

---

## Installation and Setup

### Prerequisites:
- Python 3.7+
- PyTorch
- Numpy
- Matplotlib

### Install Dependencies:

```bash
pip install torch numpy matplotlib
```

### Clone the Repository:

```bash
git clone https://github.com/sajitheranda/RNN-for-text-generation.git
cd RNN-for-text-generation
```

### Running the Project
- Clone this repository to your local machine.
- Run the provided notebook to complete the tasks. The notebook contains code for training the model, making predictions, and evaluating the results.
- After completing the project, export the notebook as a PDF and submit it via Moodle.

### Evaluation and Results
In this section, you can provide details of the results of running the model on sample inputs such as "univ", "math", "neur", and "engin". You can discuss the success of the model in predicting common word completions and suggest improvements.

``` bash
Input: "univ"
Output: ["university", "universal", "unified"]
```
