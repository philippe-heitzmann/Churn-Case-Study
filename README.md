This repository supports the data analysis needed for a customer churn case study at a wealth management business.

## Getting Started

Build and run the Jupyter environment in one step:

```bash
docker build -f Dockerfile_notebook -t docvault-notebook . && docker run -p 8888:8888 docvault-notebook
```

When the container starts, Jupyter will print a URL with a token. Open that link in your browser, then open **DocVault Notebook 1** (`notebooks/Customer Churn Case Study vF.ipynb`).

The dataset lives at `data/Churn Modeling.csv`. The notebook loads it in the second code cell with:

```python
data = pd.read_csv('../data/Churn Modeling.csv', sep=',')
```

If you run the notebook from a different working directory, adjust the path accordingly.
