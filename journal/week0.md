# Week 0 — Billing and Architecture

For week 0, I started by destroying the root account credentials with the aim of improving the security of my account and align with best practices. I destroyed all access codes that I had created earlier and set MFA for the root account. Any time I wish to log via the root account, I will be required to generate a unique code using an authenticator (Google authenticator). I also create an I am use and assigned full administrative priviledges. Moving forward this is how I will be logging into my account. 

Next, I created an alert by hooking EventBridge to Health Dashboard to SNS so that when there is a service health issue with my resources, I will be notified via mail. 

I then reviewed the questions of each pillars in the well archtected tool and answered the questions. 

Napkin Design 


![image](https://user-images.githubusercontent.com/21007127/219944190-55013943-aedc-4bd1-b7a4-d3060a69f88e.png)

Logical Diagram 

Link: https://lucid.app/lucidchart/7c50fbbb-ccc5-446c-82f2-907ab88ccfe5/edit?viewport_loc=-824%2C-1682%2C3570%2C1569%2C0_0&invitationId=inv_a5fa08b7-ba72-4d0b-9d7b-ac7edd61c78d


![image](https://user-images.githubusercontent.com/21007127/219959055-0f2c35de-7e03-4c30-9d7a-9e5e0c3cbce5.png)




