# ConceptViz: A Visual Analytics Approach for Exploring Concepts in Large Language Models

ConceptViz is a visual analytics system designed for exploring and interpreting Sparse Autoencoder (SAE) features in Large Language Models (LLMs). Our system implements a novel **Identification ⇒ Interpretation ⇒ Validation** pipeline, enabling researchers to query SAEs using concepts of interest, interactively explore concept-to-feature alignments, and validate correspondences through model behavior verification.

## 🌟 Key Features

- **🔍 Concept-based SAE Discovery**: Efficiently identify relevant SAE models across different network layers based on concept-relevance metrics
- **🗺️ Interactive Feature Exploration**: Navigate thousands of features in a 2D semantic space with hierarchical clustering and topic modeling
- **🔬 Detailed Feature Analysis**: Examine semantic information through vocabulary projections and activation pattern analysis
- **⚡ Real-time Validation**: Verify feature responses to custom inputs and discover functionally related feature sets
- **🎛️ Causal Steering**: Observe causal relationships by manipulating feature activations and analyzing output changes

## 🏗️ System Architecture
```
    ConceptViz/
    ├── frontend/ # Next.js frontend application
    ├── backend/ # Python backend services
    └── README.md
```

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm/yarn/pnpm
- Python 3.8+ and pip
- Git
    ***
### Installation

1. **Clone the repository with submodules**
   git clone --recursive https://github.com/Happy-Hippo209/ConceptViz.git
   cd ConceptViz
If you already cloned the repository, initialize submodules:

    ```bash
    git submodule init

    git submodule update
    ```

2. **Setup Frontend**

    ```bash
    cd frontend
    npm install
    # or
    yarn install
    ```


3. **Setup Backend**

    ```bash
    cd backend
    pip install -r requirements.txt
    ```
    ***
### Running the Application
1. **Start the Backend**
    ```bash
    cd backend
    python app.py
    # Backend will run on http://localhost:5000
    ```
2. **Start the Frontend**
    ```bash
    cd frontend
    npm run dev
    # or
    yarn dev
    # Frontend will run on http://localhost:3000
    ```


3. **Access the Application**
    ```bash
    Open http://localhost:3000 in your browser to start exploring!
    ```

## 🐕‍🦺 Usage Guide
### 🌊 The Three-Phase Workflow
1. **Identification** 🎯

    **Concept Query View**: Build and refine concept queries with natural language descriptions

    **SAE Discovery View**: Identify the most relevant SAE models across different network layers

1. **Interpretation** 🔍

    **Feature Explorer View**: Navigate features in a 2D semantic space with clustering

    **Feature Details View**: Examine detailed semantic information and activation patterns

2. **Validation** ✅

    **Input Activation View**: Verify feature responses to custom inputs

    **Output Steering View**: Observe causal relationships through activation steering


#### 📈 Step-by-step process:

➡️ **Start** by entering a concept of interest  
➡️ **Review** SAE model recommendations and select the most relevant layer  
➡️ **Explore** the feature space to identify relevant features  
➡️ **Examine** detailed feature semantics and activation patterns  
➡️ **Validate** findings with custom inputs and steering experiments

### 🔬 Technical Approach

**Concept-based SAE Model Retrieval:** Multi-threshold ranking approach using semantic similarity

**Hierarchical Feature Organization:** UMAP dimensionality reduction with agglomerative clustering

**Activation-Similarity Matrix:** Novel visualization to identify discrepancies between feature explanations and actual behavior

**Interactive Validation:** Custom input analysis and causal verification through activation steering

## 🤖 Supported Models
**Currently supports SAEs trained on:**

Gemma-2-2b and GPT2 small models

Residual stream activations across all transformer layers

16,384-dimensional sparse feature representations for Gemma-2-2b and 32,768 for GPT2 small

## 🔗 Links

🌐 Project Website: https://happy-hippo209.github.io/ConceptViz/

📧 Contact: lihaoxuan@zju.edu.cn

## 🙏 Acknowledgments
We thank the anonymous reviewers for their insightful feedback.

**Special thanks to:**

**Neuronpedia** for providing SAE feature data

**GemmaScope** and **OpenAI** for the SAE models

The broader mechanistic interpretability research community

***

<div align="center">

<strong>🔍 Explore the inner workings of Large Language Models with ConceptViz! 🔍</strong>

</div>