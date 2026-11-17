# XGBoost training and delivery

The project estimates house prices. Training imputes and scales features, tunes XGBoost and persists preprocessing objects with the classifier. Flask uses these artifacts for inference. GitHub Actions runs tests, builds the image and includes registry and SSH deployment steps. Configure the registry and server secrets referenced by the workflow before enabling deployment.

## Run locally

```sh
python -m pip install -r requirements.txt
python -m pytest tests/
python -m scripts.automatiza_treino
```
