student-k8s-demo - ready-made project

1. Unzip, open the folder in VS Code.
2. python -m venv .venv
3. .\.venv\Scripts\python.exe -m pip install -r requirements.txt
4. .\.venv\Scripts\python.exe -m pytest -v
5. .\.venv\Scripts\python.exe app.py

.github/workflows/pipeline.yml      -> CI (tests only), use first
extras/pipeline-with-docker.yml     -> later, copy over pipeline.yml after adding Docker Hub secrets
k8s/deployment.yaml                 -> replace YOUR_DOCKERHUB_USERNAME and REPLACE_WITH_COMMIT_SHA before applying
