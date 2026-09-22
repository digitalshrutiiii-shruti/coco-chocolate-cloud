# COCO Chocolate — Flask + Cloud Computing

This version keeps the existing COCO Chocolate website and adds a Python Flask layer so it can be run from Jupyter and deployed as a cloud web service.

## Files
- `app.py` — Flask server
- `templates/index.html` — website
- `requirements.txt` — Python dependencies
- `Procfile` — production start command
- `render.yaml` — Render deployment configuration
- `COCO_Cloud_Computing.ipynb` — Jupyter notebook
- `CLOUD_COMPUTING_GUIDE.md` — project/viva explanation

## Run from Jupyter
Open `COCO_Cloud_Computing.ipynb` and run the cells in order.

## Run from terminal
```bash
pip install -r requirements.txt
python app.py
```
Then open `http://127.0.0.1:5000`.

## Live cloud deployment
Push the folder to GitHub and deploy it on Render as a Python Web Service. Use:
- Build: `pip install -r requirements.txt`
- Start: `gunicorn app:app`
