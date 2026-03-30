# Graduation-Project
Title: etvds-edge — Edge unit for license-plate detection & seatbelt violation reporting

Short description:
Edge processing pipeline that watches a folder for images, runs a YOLO detector + OCR to read license plates, logs plates to a local SQLite DB, sends plate data to a TCP endpoint, and posts detected violations (e.g., no seatbelt) to a backend API.

Quick run:

    Edit config.py for your environment.
    pip install -r requirements.txt
    python main.py

Notes:

    Model file (yolo12sconf.pt) is not included — place it in the project folder or update MODEL_PATH.
    Adjust OCR/model code if API signatures differ.
