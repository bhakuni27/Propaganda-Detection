# Propaganda Detection
Propaganda is a pervasive issue in today’s digital age, especially with the rise of social media, where information spreads rapidly and often without verification. Detecting propaganda is crucial for promoting media literacy, enabling informed decision-making, and curbing the spread of misleading or harmful content.

This project builds a **binary text classification system** to determine whether a given piece of content contains propaganda. We leverage two state-of-the-art transformer-based models, **BERT** and **RoBERTa**, to perform this task.

## Prerequisites

Ensure you have **Python 3** and **pip** installed. If not, you can download Python from [python.org](https://www.python.org/).

To run this project, you’ll need the following libraries:

- PyTorch
- Transformers (by HuggingFace)
- scikit-learn
- pandas
- numpy
- seaborn
- matplotlib

To install the required libraries, run:

```
pip install torch transformers scikit-learn pandas numpy matplotlib seaborn
```
#### Additional Requirements

- **GPU** (recommended for faster training)
- **Jupyter Notebook** or any environment that supports `.ipynb` files


## Usage

#### 1. Clone the repository:

```
git clone https://github.com/bhakuni27/Propaganda-Detection.git
cd Propaganda-Detection
```
#### 2. Open the notebook:

Launch `PropagandaDetection.ipynb` using Jupyter or any compatible IDE.

#### 3. Run all cells sequentially.

## Results

Below is a summary of the classification performance for both models. 

| Model   | Accuracy | Class          | Precision | Recall | F1-Score |
| ------- | -------- | -------------- | --------- | ------ | -------- |
| BERT    | 95%      | Propaganda     | 93%       | 96%    | 95%      |
|         |          | Not Propaganda | 96%       | 93%    | 95%      |
| RoBERTa | 94%      | Propaganda     | 95%       | 94%    | 94%      |
|         |          | Not Propaganda | 94%       | 95%    | 95%      |

Both models achieve strong performance, with slight trade-offs in recall vs. precision.

#### Final Recommendation
Opt for **BERT** when the priority is to detect as much propaganda as possible (higher recall).
Choose **RoBERTa** if it’s more important to avoid incorrectly flagging non-propaganda as propaganda (slightly higher precision).
