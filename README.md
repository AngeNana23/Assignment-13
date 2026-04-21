# Assignment-13

# Generative AI Transformer Text Generation Project

## Overview

This project demonstrates a simplified Generative Pre-trained Transformer (GPT)-style model for text generation using TensorFlow.

The aim is to explore Generative AI fundamentals, Transformer architecture, and practical text generation using deep learning techniques.

The model is trained on a public domain dataset and generates text based on a user-provided seed prompt.

---

## Dataset

- Source: Project Gutenberg  
- Book used: *Alice in Wonderland*  
- Type: Public domain text dataset  

### Preprocessing steps:
- Lowercasing text  
- Tokenization using Keras Tokenizer  
- Conversion into sequences  
- Padding sequences for uniform input length  

---

## Model Architecture

The model is a simplified Transformer-based architecture inspired by GPT models.

It includes:

- Embedding Layer (word representation)
- Multi-Head Self-Attention (context learning)
- Residual Connections (stability improvement)
- Layer Normalization (training stability)
- Feedforward Neural Network
- Softmax Output Layer (next-word prediction)

This architecture allows the model to learn relationships between words and generate coherent text sequences.

---

## Technologies Used

- Python  
- TensorFlow / Keras  
- NumPy  
- Requests  

---

## How the Model Works

### 1. Data Processing
Text is cleaned, tokenized, and converted into numerical sequences. These sequences are padded to ensure consistent input size.

### 2. Training
The model learns to predict the next word in a sequence using:
- Sparse categorical cross-entropy loss
- Adam optimizer
- Multiple training epochs

### 3. Text Generation
The model generates text by:
- Accepting a seed input
- Predicting the next word probabilistically
- Repeating the process to form sentences

Temperature sampling is used to control randomness in output.

---

## Example

Input:
the future of artificial intelligence

Output:
the future of artificial intelligence the chapter delight kind chapter party chapter puzzling the “oh all feet moment way struck curtseying chapter the was be chapter the opened gutenberg ever next on alice the they get the is likely the grow be the off the

---

## Applications of Generative AI

- Content writing (blogs, articles, emails)
- Chatbots and virtual assistants
- Code generation tools
- Educational assistants
- Creative writing support

---

## Ethical Considerations

Generative AI raises several ethical concerns:

### Bias
Models may learn biased patterns from training data.

### Misinformation
AI may generate incorrect or misleading information.

### Privacy
Sensitive or private data must not be used in training datasets.

### Copyright
Only public domain or properly licensed data should be used.

### Mitigation Strategies
- Use clean and balanced datasets  
- Apply human review for outputs  
- Ensure transparency in AI systems  
- Validate generated content  

---

## Limitations

- Simplified Transformer architecture (not full GPT-3 level)
- Limited dataset size
- May produce repetitive outputs
- Limited contextual understanding compared to large-scale models

---

## Future Improvements

- Implement full GPT-style decoder with causal masking
- Use larger datasets (The Pile, WikiText)
- Improve sampling techniques (top-k, nucleus sampling)
- Add training visualizations
- Build a web-based interface using Streamlit or Gradio

---

## Conclusion

This project demonstrates the fundamental principles of Generative AI using a Transformer-based model. It shows how machine learning systems can learn patterns from text data and generate meaningful sequences.

While simplified, it provides a strong foundation for understanding modern GPT-style architectures and their real-world applications.

---

## Author
Ange Nana
