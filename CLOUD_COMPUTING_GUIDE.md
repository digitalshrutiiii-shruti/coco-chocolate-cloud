# COCO Chocolate — Cloud Computing Project

## Architecture
Browser → Render Cloud Web Service → Gunicorn → Flask → HTML/CSS/JavaScript

## Local/Jupyter run
The Jupyter notebook starts the Flask application locally and checks the `/health` endpoint.

## Cloud deployment
1. Create a GitHub repository and upload this project.
2. In Render, choose **New → Web Service** and connect the repository.
3. Build command: `pip install -r requirements.txt`
4. Start command: `gunicorn app:app`
5. Choose the Free plan and deploy.
6. Render provides a public `onrender.com` URL.

## Cloud-computing points for presentation
- **Cloud service:** hosted web application
- **Compute:** Render web service runs the Flask application
- **Application server:** Gunicorn
- **Framework:** Flask
- **Deployment:** Git-based continuous deployment
- **Public access:** HTTPS URL supplied by the cloud platform
- **Health check:** `/health`
- **Scalability concept:** the application can be moved to a larger compute plan or multiple instances as traffic grows
