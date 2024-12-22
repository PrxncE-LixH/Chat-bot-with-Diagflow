
# Tasty Eastery After-Hours Chat Bot

Tasty Eastery Chat Bot is an intelligent assistant powered by Google's Dialogflow - ES, designed to enhance user interaction on the Tasty Eastery website. This chatbot seamlessly guides users in making online orders during closing hours, ensuring a smooth and efficient customer experience even when the restaurant is not actively open.
## Structure

- [Frontend](https://github.com/PrxncE-LixH/Chat-bot-with-Diagflow/tree/master/frontend)
- [Chatbot](https://github.com/PrxncE-LixH/Chat-bot-with-Diagflow/blob/master/Tasty-Eatery.zip)
- [Backend](https://github.com/PrxncE-LixH/Chat-bot-with-Diagflow/blob/master/backend/main.py)
- [Database](https://github.com/PrxncE-LixH/Chat-bot-with-Diagflow/tree/master/backend/database)

## License


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

## Authors

- [PrxncE-LixH](https://github.com/PrxncE-LixH)


## Installation
- Frontend

```
index.html
```

- chatbot
```
Chatbot logic is located at 
https://github.com/PrxncE-LixH/Chat-bot-with-Diagflow/blob/master/Tasty-Eatery.zip 
```
Download and import as a new diaglog flow project.  


- Backend

  Install dependancies
  ```
  pip install -r requirements.txt
  ```


- Start server
  ```
  uvicorn main:app --reload
  python -m uvicorn main:app --reload    if you're on windows 
  ```
    
Google only allows HTTPS connections. To reach the chatbot api, you will need to generate a self-signed certificate with openssl. Refer to https://www.youtube.com/watch?v=P5mdDTMmfL0&list=PLmiXwP1ZU2Fd3KxbA6LvulUs5j8BUDXX0 for assistance. 

To run locally with HTTPS without a signed certificate, you can use Ngrok. Refer to 
https://www.youtube.com/watch?v=aFwrNSfthxU to install and set it up.
```
ngrok http 8000
```
- Goto Fulfillment on your Diagflow project, enable webhooks and replace the url with the new Ngrok url.



## Database

An SQL Database was used locally for the process. Database file is located at https://github.com/PrxncE-LixH/Tasty_Eatery_Dialogflow/tree/main/database. 

It is assumed you already have XAMPP, mysql, and MySQL Workbench 8.0 set up. Refer to https://www.youtube.com/watch?v=2ydHLNnGIVI for assistance. 

- Create a connection in MySQL Workbench, click on the server tab and data import. Import the attached database file and set it as the default schema. The database file has the names and prices of food items. It also generates and stores Order IDs needed for tracking.  
  

## How to run

- Start XAMPP (APACHE, MYSQL) and MySQL Workbench 8.0 
- Run backend server
- Start Ngrok and generate an HTTPS url- Ngrok should be in the same directory as the backend server file. 
- Enable webhooks on Diagflow and replace the url with the new Ngrok url.
- Start frontend
## Screenshots
```
video

https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Recording.mp4?alt=media&token=92bc97c1-fc19-4aaa-9dd6-0ca66b9f9780

```

![image](https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Screenshot%202024-12-22%20014423.png?alt=media&token=d04713e8-6071-4f8f-9f72-2156d33a4cee)


![image](https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Screenshot_1_TE.jpg?alt=media&token=6d957cb3-656f-44b8-a902-b44de86f4838)

![image](https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Screenshot_2_TE.jpg?alt=media&token=905c60ce-7fb3-46cb-a9fe-6ddb29895ff6)

![image](https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Screenshot_3_TE.jpg?alt=media&token=4fa06635-25c1-4958-bde6-b833ebe7df0c)

![image](https://firebasestorage.googleapis.com/v0/b/tomatoguard-2110e.appspot.com/o/Screenshot_4_TE.jpg?alt=media&token=c92b3138-a72a-41c1-beaf-250370f9d300)




