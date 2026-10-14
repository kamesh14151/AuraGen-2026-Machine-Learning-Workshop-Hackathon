# 🚀 Advanced Machine Learning — GPU Track

Welcome to the **Advanced-need-gpu** track for **AuraGen 2026**. These notebooks introduce deeper model-training workflows, including transfer learning, transformer fine-tuning, and training a neural network from scratch.

> **Compute note:** A CUDA-enabled GPU is recommended for practical training times. Google Colab or another GPU-enabled notebook environment is a convenient option. The notebooks may run on CPU, but training can be much slower.

## 📘 What's inside?

### 1. Vision Transformer — Bean Leaf Image Classification
**Notebook:** [`01_ViT_Bean_Leaf_Image_Classification_GPU.ipynb`](./01_ViT_Bean_Leaf_Image_Classification_GPU.ipynb)

- Load the bean-leaf image dataset
- Start from a pretrained Vision Transformer (ViT)
- Fine-tune the model for image classification
- Evaluate on held-out data using classification metrics
- Inspect a confusion matrix and save the trained model

**Dataset:** [AI-Lab-Makerere/beans on Hugging Face](https://huggingface.co/datasets/AI-Lab-Makerere/beans)

### 2. DistilBERT — Emotion Text Classification
**Notebook:** [`02_DistilBERT_Emotion_Text_Classification_GPU.ipynb`](./02_DistilBERT_Emotion_Text_Classification_GPU.ipynb)

- Load and tokenize text data
- Fine-tune a pretrained DistilBERT language model
- Classify text into emotion categories
- Evaluate using metrics such as accuracy and macro-F1
- Inspect a confusion matrix and save the trained model

**Dataset:** [dair-ai/emotion on Hugging Face](https://huggingface.co/datasets/dair-ai/emotion)

### 3. CNN — CIFAR-10 Image Classification from Scratch
**Notebook:** [`03_CIFAR10_CNN_Train_From_Scratch_GPU.ipynb`](./03_CIFAR10_CNN_Train_From_Scratch_GPU.ipynb)

- Load and normalize CIFAR-10 images
- Build a convolutional neural network (CNN)
- Train the model from random initialization
- Review training/validation curves
- Evaluate on test data and save a checkpoint

**Dataset:** [CIFAR-10 via torchvision](https://www.cs.toronto.edu/~kriz/cifar.html). The notebook downloads it using `torchvision.datasets.CIFAR10`; a Kaggle account is not required.

## 🖼️ Notebook overview

![Advanced ML examples — overview 1](./Images/Advanced-1.jpg)

![Advanced ML examples — overview 2](./Images/Advanced-2.jpg)

## ⚙️ Recommended environment

- Python 3.10 or newer recommended
- Google Colab with **GPU runtime enabled**, or a CUDA-compatible local environment
- Internet access to download datasets and pretrained model weights
- Enough disk space for datasets, model checkpoints, and caches

### Google Colab setup
1. Open a notebook from this folder on GitHub.
2. Upload it to [Google Colab](https://colab.research.google.com/).
3. In Colab, select **Runtime → Change runtime type → T4 GPU** (or another available GPU).
4. Run the notebook cells from top to bottom.
5. If using a different environment, follow the package-install instructions in the notebook.

## 🧰 Common libraries

Depending on the notebook, packages may include:

```bash
pip install torch torchvision transformers datasets accelerate scikit-learn matplotlib
```

Follow each notebook's own installation cells and restart the runtime if a package update requires it.

## 🧪 Advanced-track challenge

Fine-tune a pretrained **image or text model** on a suitable dataset. Compare your results with a meaningful baseline where practical, and justify your choices.

Your explanation should cover:
- Why the chosen pretrained model fits the task
- How the dataset was split and preprocessed
- Which metrics are appropriate and why
- What validation/test results show
- Overfitting, class imbalance, or other limitations
- What you would improve with more time or compute

## 📊 What participants should submit

- A reproducible notebook with clear comments
- Dataset and model references
- Training configuration and compute environment
- Evaluation metrics and relevant plots
- A short explanation of results, limitations, and next steps

## ⚠️ Important notes

- Do not evaluate repeatedly on the test set while tuning; use validation data for model selection.
- Do not report only accuracy when classes are imbalanced; consider macro-F1 and per-class metrics.
- GPU availability and training speed depend on the environment.
- Model and dataset licenses or terms may apply. Check the linked model and dataset pages before redistribution or deployment.
- The notebooks are educational examples; run all cells and verify outputs in your chosen environment before the event.

## 💡 Learning outcome

Participants move beyond classical ML into **transfer learning, pretrained-model fine-tuning, neural-network training, and evaluation-driven experimentation**.

---

Part of the **AuraGen 2026** machine-learning workshop.
