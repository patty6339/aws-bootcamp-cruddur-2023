# Week 3 — Decentralized Authentication

The App is running well

![image](https://user-images.githubusercontent.com/21007127/226589045-9d20131b-44af-4047-87dd-d6e17408fc0c.png)

Added this code to solve the sign up error 

aws cognito-idp admin-set-user-password \
  --user-pool-id <your-user-pool-id> \
  --username <username> \
  --password <password> \
  --permanent

![image](https://user-images.githubusercontent.com/21007127/227298282-2506d1a4-033c-4f96-b94b-7def54c6816f.png)
  
  
 Edited the preferred name and name fields on Cognito and it reflected on the app as seen here 

  
  ![image](https://user-images.githubusercontent.com/21007127/227302863-bc79e697-c1cd-434e-8d60-2ed1c76c791f.png)
  
  Received a verification code when signing up to Cruddur to the email I provided
  
  ![image](https://user-images.githubusercontent.com/21007127/227316322-35b6a445-f273-4d93-91aa-3f75fc89060a.png)

  Was required to enter it here:
  
  ![image](https://user-images.githubusercontent.com/21007127/227316476-cd57fd2f-f2a4-4391-8dad-bb204ded8b7c.png)

  
 Successfully logged in after entering the verification code and signing in 
  
 ![image](https://user-images.githubusercontent.com/21007127/227317068-f2755e66-c082-4ca2-bce0-c50789107684.png)

  
  Updated CORS by adding this code to the app.py file
  
  cors = CORS(
  app, 
  resources={r"/api/*": {"origins": origins}},
  headers=['Content-Type', 'Authorization'], 
  expose_headers='Authorization',
  methods="OPTIONS,GET,HEAD,POST"
)
  
  


