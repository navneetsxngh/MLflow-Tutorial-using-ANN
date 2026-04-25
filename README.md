# 🧠 MLflow Tutorial using ANN

A hands-on tutorial demonstrating how to track, log, and manage machine learning experiments using **MLflow** with an **Artificial Neural Network (ANN)** built in TensorFlow/Keras. Hyperparameter tuning is handled via **Hyperopt**, with all runs tracked in a local MLflow SQLite backend.

---

## 📁 Project Structure

```
MLflow-Tutorial-using-ANN/
│
├── starter.ipynb       # Starter notebook — baseline ANN setup
├── mlflow.ipynb        # Main notebook — MLflow tracking integration
├── mlflow.db           # SQLite database storing MLflow experiment runs
├── requirements.txt    # Python dependencies
└── .gitignore
```

---

## 🚀 What You'll Learn

- How to set up **MLflow experiment tracking** with a local SQLite backend
- How to **log parameters, metrics, and models** using `mlflow.log_param()` and `mlflow.log_metric()`
- How to build and train an **ANN using TensorFlow/Keras**
- How to integrate **Hyperopt** for automated hyperparameter search
- How to use the **MLflow UI** to compare experiment runs visually

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| [MLflow](https://mlflow.org/) | Experiment tracking & model registry |
| [TensorFlow / Keras](https://www.tensorflow.org/) | Building & training the ANN |
| [Hyperopt](http://hyperopt.github.io/hyperopt/) | Hyperparameter optimization |
| SQLite (`mlflow.db`) | Local MLflow tracking backend |

---

## ⚙️ Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/navneetsxngh/MLflow-Tutorial-using-ANN.git
cd MLflow-Tutorial-using-ANN
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

**Dependencies:**
```
tensorflow
mlflow
keras
hyperopt
```

---

## ▶️ Running the Notebooks

Launch Jupyter and open the notebooks in order:

```bash
jupyter notebook
```

1. **`starter.ipynb`** — Start here. Sets up the base ANN without MLflow.
2. **`mlflow.ipynb`** — The main tutorial. Adds MLflow tracking and Hyperopt tuning.

---

## 📊 Viewing the MLflow UI

The project uses a local SQLite backend (`mlflow.db`) to store runs. To launch the MLflow dashboard:

```bash
mlflow ui --backend-store-uri sqlite:///mlflow.db
```

Then open your browser at **http://localhost:5000** to compare runs, metrics, and parameters across experiments.

---

## 📌 Key Concepts Covered

- **MLflow Tracking** — Log and query experiments, parameters, metrics, and artifacts
- **MLflow Projects** — Packaging code for reproducibility
- **ANN with Keras** — Dense layers, activation functions, loss and optimizer configuration
- **Hyperopt** — Tree-structured Parzen Estimator (TPE) for efficient hyperparameter search

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

> Built with ❤️ to make ML experiment tracking easy and reproducible.