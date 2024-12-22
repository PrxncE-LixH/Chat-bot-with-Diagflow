Downloads
- My SQLBench
- Ngrok

# Backend needs to be hosted to get Chatbot to track orders.
# To run locally, run the following commands
   - pip intall pip install -r requirements.txt  - installs needed packages

# download and install my sql bench and import Tasty_eatery database file included.
 - set the imported database as your default schema.
   
COMMANDS
- run uvicorn main:app --reload - to run the backend
# an address will be generated. example: http://129.0.0.1:8000 
# Google's diagflow does not support https webhooks.

# you can download ngrok save it in the backend directory. 
 run the commnad ngrok.exe http://129.0.0.1:8000
