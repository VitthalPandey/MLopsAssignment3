# MLOps Assignment 3

- DockerHub Image: *https://hub.docker.com/repositories/150191*
  
This project shows how to build a full machine learning pipeline that runs automatically.

## 📁 Files in This Project

- `train.py` → trains the model and saves it
- `predict.py` → loads the model and runs prediction
- `quantize.py` → compresses the model and tests it in PyTorch
- `Dockerfile` → builds a Docker container
- `.github/workflows/ci.yml` → GitHub Actions automation
- `requirements.txt` → list of required Python packages


## 📊 Final Model Comparison Table

| Metric       | Original Sklearn Model (`model.joblib`) | Quantized Model (`quant_params.joblib`) |
|--------------|-----------------------------------------|------------------------------------------|
| R² Score     | 0.6012                                  | 0.1657                                   |
| Model Size   | 414 Bytes                               | 469 Bytes                                |
