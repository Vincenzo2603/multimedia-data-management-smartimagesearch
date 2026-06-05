# multimedia-data-management-smartimagesearch
Content-Based Image Retrieval system developed for the Multimedia Data Management course. The project combines classical visual descriptors and modern deep learning embeddings for image retrieval.

# 🔍 SmartImageSearch

> A Content-Based Image Retrieval (CBIR) system developed for the **Multimedia Data Management** course at the **University of Bologna**.

---

## 📖 Overview

SmartImageSearch is a multimedia data management application designed to retrieve visually similar images from a collection.

Unlike traditional image search engines that rely primarily on textual metadata, SmartImageSearch analyzes the visual content of images and retrieves results based on similarity measures computed directly from image features.

The project explores both **traditional multimedia retrieval techniques** and **modern deep learning approaches**, providing a practical comparison between handcrafted visual descriptors and learned visual representations.

---

## 🎯 Objectives

The project aims to:

- Model multimedia data using structured, semi-structured, and unstructured representations
- Implement a Content-Based Image Retrieval (CBIR) system
- Compare classical and modern retrieval pipelines
- Evaluate retrieval quality using similarity metrics
- Demonstrate the transition from traditional multimedia retrieval to embedding-based retrieval

---

## 🏗️ System Architecture

The retrieval process follows the architecture below:

```text
Query Image
     │
     ▼
Feature Extraction
     │
     ▼
Feature Vector
     │
     ▼
Similarity Engine
     │
     ▼
Ranking Module
     │
     ▼
Retrieved Images
```

The system extracts visual features from a query image, compares them against a feature database, computes similarity scores, and returns the most relevant results.

---

## 🗂️ Multimedia Data Modeling

SmartImageSearch integrates multiple types of multimedia data:

| Data Type | Example |
|------------|------------|
| Structured Data | Image IDs, Categories |
| Semi-Structured Data | XML Metadata, Tags |
| Unstructured Data | Images |

The project also explores metadata management and retrieval mechanisms commonly adopted in Multimedia Database Management Systems.

---

## 🔎 Retrieval Pipelines

### 1️⃣ Classical Retrieval Pipeline

The classical approach represents images through handcrafted visual descriptors.

#### Features

- RGB Color Histograms
- Feature Vector Representation
- Euclidean Distance Similarity

#### Workflow

```text
Image
  ↓
Color Histogram Extraction
  ↓
Feature Vector
  ↓
Euclidean Distance
  ↓
Top-K Similar Images
```

---

### 2️⃣ Modern Retrieval Pipeline

The modern approach uses deep visual embeddings extracted from a pretrained neural network.

#### Features

- ResNet18 Pretrained Model
- Deep Feature Embeddings
- Cosine Similarity

#### Workflow

```text
Image
  ↓
ResNet18
  ↓
Deep Embedding
  ↓
Cosine Similarity
  ↓
Top-K Similar Images
```

---

## 📝 Text-Based Retrieval Extension

In addition to Content-Based Image Retrieval, the project includes a simple text-based retrieval module.

Users can search by category labels such as:

```text
airplane
automobile
cat
dog
```

The system retrieves matching images using metadata associated with the dataset.

This extension demonstrates how visual retrieval and metadata-based retrieval can coexist within a multimedia management framework.

---

## 📊 Dataset

The implementation uses a subset of the **CIFAR-10** dataset.

### Selected Categories

- ✈️ Airplane
- 🚗 Automobile
- 🐱 Cat
- 🐶 Dog

The same dataset is used across all experiments to ensure a fair comparison between retrieval approaches.

---

## 📈 Evaluation

Retrieval quality is evaluated using:

### Precision@1

Measures whether the first retrieved image belongs to the same category as the query.

### Precision@5

Measures the proportion of relevant images among the first five retrieved results.

These metrics allow a direct comparison between the classical and modern retrieval pipelines.

---

## 📁 Repository Structure

```text
SmartImageSearch-CBIR/
│
├── README.md
│
├── notebook/
│   └── SmartImageSearch.ipynb
│
├── presentation/
│   ├── SmartImageSearch_ABCDEF.pptx
│   └── SmartImageSearch_ABCDEF.pdf
│
├── report/
│   └── StudentsFreeExercise.pdf
│
├── results/
│   ├── classical_retrieval.png
│   ├── modern_retrieval.png
│   ├── text_retrieval.png
│   └── performance_comparison.png
│
├── docs/
│   ├── architecture.png
│   ├── workflow.png
│   └── diagrams/
│
├── requirements.txt
│
├── .gitignore
│
└── LICENSE
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/USERNAME/SmartImageSearch-CBIR.git
cd SmartImageSearch-CBIR
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebook/SmartImageSearch.ipynb
```

and execute all cells sequentially.

---

## 🧪 Demonstrations

The notebook includes:

✅ Classical image retrieval

✅ Deep-learning image retrieval

✅ Side-by-side comparison

✅ Precision evaluation

✅ Text-based image retrieval

---

## 🎓 Academic Context

This project was developed as part of the **Multimedia Data Management** course.

Main topics covered:

- Multimedia Data Modeling
- Multimedia Databases
- Similarity Measures
- Information Retrieval
- Content-Based Image Retrieval
- Multimedia Indexing
- Multimedia Search Systems
- Deep Visual Representations

---

## 🔮 Future Extensions

Possible future developments include:

- Hybrid text-image retrieval
- Natural language image search
- Semantic image retrieval
- Multimodal retrieval systems
- Larger-scale image collections
- User relevance feedback mechanisms

---

## 👨‍💻 Author

**Vincenzo Lombardi**

Master's Degree in Computer Science  
Curriculum C  
University of Bologna

---

## 📜 License

This project is released under the MIT License.

---

⭐ If you found this project interesting, consider giving it a star.