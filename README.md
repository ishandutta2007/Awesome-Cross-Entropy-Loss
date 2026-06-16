<!-- SEO Tags -->
<div align="center">
  <meta name="description" content="Awesome Cross-Entropy Loss: A curated list of Cross-Entropy Loss variants, formulas, and resources for Machine Learning and Deep Learning.">
  <meta name="keywords" content="Cross-Entropy, Machine Learning, Deep Learning, AI, Loss Functions, Log Loss, Computer Vision, NLP, Awesome List">
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=900&size=40&pause=1000&color=F72C00&center=true&vCenter=true&width=800&lines=Awesome+Cross-Entropy+Loss;The+Definitive+Guide+to+Loss+Functions" alt="Awesome Cross-Entropy Loss Banner" />
</div>

<div align="center">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome" />
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License" />
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome">
    <img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome" />
  </a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007label=Follow" /></a>
</div>

<br/>

<div align="center">
  <img src="https://media.giphy.com/media/l41YtZOb9EUABnuqA/giphy.gif" alt="AI and Machine Learning GIF" width="400" />
</div>

# 🚀 Awesome-Cross-Entropy-Loss

## 🧠 Understanding Cross-Entropy Loss

Cross-Entropy Loss is the standard metric used in machine learning to measure the dissimilarity between true probability distributions and the ones predicted by a model. It heavily penalizes confident but incorrect predictions, acting as the backbone for almost all modern classification algorithms.

---

## 🏆 Top Cross-Entropy Loss Examples

### 1. [Binary Cross-Entropy (Log Loss)](binary-cross-entropy.md) 📉
Used for problems with exactly two output classes (e.g., Yes/No, Spam/Ham).

| Example Application | The Math / Logic | Scenario | Year | Original Paper |
| :--- | :--- | :--- | :--- | :--- |
| Determining whether a credit card transaction is fraudulent (True = Fraud, False = Legitimate). | `Loss = -[y * log(ŷ) + (1 - y) * log(1 - ŷ)]` | If a transaction is fraudulent (`y = 1`), and the AI predicts an 80% chance of fraud (`ŷ = 0.8`), the loss is low. If the AI predicts a 10% chance (`ŷ = 0.1`), the penalty skyrockets. | 1958 | [The Regression Analysis of Binary Sequences](https://www.jstor.org/stable/2983890) |

### 2. [Categorical Cross-Entropy (Multi-Class)](categorical-cross-entropy.md) 📊
Used when an input belongs to exactly **one** category out of three or more possible options.

| Example Application | The Math / Logic | Scenario | Year | Original Paper |
| :--- | :--- | :--- | :--- | :--- |
| Classifying an image of a handwritten digit from 0 to 9. | `Loss = -Σ (y_c * log(ŷ_c))` | True label is "7". If your AI predicts a 90% chance for "7" and 10% scattered across other digits, the loss will be near zero. | 1989 | [Probabilistic Interpretation of Feedforward Classification Network Outputs](https://proceedings.neurips.cc/paper/1989/file/8f14e45fceea167a5a36dedd4bea2543-Paper.pdf) |

### 3. [Sparse Categorical Cross-Entropy](sparse-categorical-cross-entropy.md) ⚡
Mathematically identical to categorical cross-entropy, but more memory-efficient when your classes are labeled as integers instead of large one-hot arrays.

| Example Application | The Math / Logic | Scenario | Year | Original Paper |
| :--- | :--- | :--- | :--- | :--- |
| A large-scale animal classifier with 1,000 distinct species classes. | Memory-efficient implementation using integer labels instead of one-hot arrays. | The target is simply the integer `45` (for cheetah). Instead of storing 999 zeros and a one, the framework uses the index directly, saving massive RAM. | 2015 | [TensorFlow: Large-Scale Machine Learning on Heterogeneous Distributed Systems](https://arxiv.org/abs/1603.04467) |

### 4. [Sequence/Language Modeling](sequence-language-modeling.md) 📝
Used in autoregressive models to predict the likelihood of the next token in a sequence.

| Example Application | The Math / Logic | Scenario | Year | Original Paper |
| :--- | :--- | :--- | :--- | :--- |
| Next-word prediction in a transformer model (e.g., ChatGPT, Llama). | Autoregressive prediction of the next token probability in a sequence. | The model evaluates probabilities over the entire vocabulary, penalizing incorrect grammatical or factual sequences with Cross-Entropy Loss. | 2003 | [A Neural Probabilistic Language Model](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf) |

### 5. [Image Segmentation](image-segmentation.md) 🖼️
Evaluating classification on a **pixel-by-pixel** level instead of whole-image categorization.

| Example Application | The Math / Logic | Scenario | Year | Original Paper |
| :--- | :--- | :--- | :--- | :--- |
| A medical imaging AI identifying cancer cells on an X-ray. | Pixel-wise cross-entropy loss applied to every individual pixel. | Every single pixel is individually classified as either "tumor" or "healthy tissue", allowing for precise semantic localization. | 2015 | [Fully Convolutional Networks for Semantic Segmentation](https://arxiv.org/abs/1411.4038) |

## 📈 Star History
<div align="center">
   <a href="https://www.star-history.com/repos=ishandutta2007%2FAwesome-Cross-Entropy-Loss&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chartrepos=ishandutta2007/Awesome-Cross-Entropy-Loss&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chartrepos=ishandutta2007/Awesome-Cross-Entropy-Loss&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chartrepos=ishandutta2007/Awesome-Cross-Entropy-Loss&type=date&legend=bottom-right" />
    </picture>
   </a>
</div>
