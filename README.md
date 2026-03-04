# Exploring Transformer Models with Hugging Face

This project is a set of small experiments with modern Transformer models using the Hugging Face `transformers` library. It focuses on inspecting token embeddings, attention patterns, and text generation behavior. 

## Models and Experiments

### 1. DistilBERT Token Embeddings

- Load a pretrained DistilBERT model and tokenizer.
- Tokenize sample text and extract last hidden state embeddings for each token.
- Inspect embedding tensor shapes to understand the representation structure (sequence length × hidden size). 

### 2. BERT Attention Visualization

- Load a BERT model with `output_attentions=True` to return attention weights.
- Run a sentence through the model, select a specific layer and head.
- Visualize the attention matrix with a heatmap (rows and columns are tokens; cell intensity shows attention weight). 

### 3. GPT-2 Text Generation

- Load a GPT-2 language model and tokenizer.
- Provide a math-related or technical prompt.
- Use `model.generate()` to produce text continuations, then decode and inspect the generated text. 

## Skills Demonstrated

- Using Hugging Face `transformers` to load and run pretrained NLP models (DistilBERT, BERT, GPT-2). 
- Working with tokenization, hidden states, and attention tensors.
- Visualizing attention weights with Python plotting libraries.
- Generating text and interpreting model behavior. 

## How to Run

1. Clone or download this repository.
2. Open `Transformer_Experiments.ipynb` in Google Colab or Jupyter.
3. Ensure `transformers`, `torch`, and visualization libraries (e.g., `matplotlib`, `seaborn`) are installed.
4. Run all cells from top to bottom to reproduce embeddings, attention visualizations, and GPT-2 generations. 
