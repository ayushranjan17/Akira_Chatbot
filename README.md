# Akira_Chatbot
This is the repository for the files that are used in chatbot creation.

Backend Codes in:
db_helper.py, generic_helper.py, main.py

SQL file used for database management: pandeyji_eatery.sql

===================

backend: Contains Python FastAPI backend code
 pandeyji_eatery.sql: contains the dump of the database, you need to import this into your MySQL db by using MySQL workbench tool
dialogflow_assets: this has training phrases etc. for our intents

Install these modules
======================

pip install mysql-connector
pip install "fastapi[all]"

OR just run pip install -r backend/requirements.txt to install both in one shot

To start fastapi backend server
================================
1. Go to backend directory in your command prompt
2. Run this command: uvicorn main:app --reload

ngrok for https tunneling
================================
1. To install ngrok, go to https://ngrok.com/download and install ngrok version that is suitable for your OS
2. Extract the zip file and place ngrok.exe in a folder.
3. Open windows command prompt, go to that folder and run this command: ngrok http 80000

NOTE: ngrok can timeout. you need to restart the session if you see session expired message.

Drive link contains screen recording of the chatbot in action, the backend interface, and 
the database schema where order is stored and price is calculated along with progress of the order.
https://drive.google.com/drive/folders/11dTKjK-xi_RSKrjFmqQWHVsdho-yRM15?usp=sharing
