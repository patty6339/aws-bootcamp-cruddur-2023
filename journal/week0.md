# Week 0 — Billing and Architecture

For week 0, I started by destroying the root account credentials with the aim of improving the security of my account and align with best practices. I destroyed all access codes that I had created earlier and set MFA for the root account. Any time I wish to log via the root account, I will be required to generate a unique code using an authenticator (Google authenticator). I also create an I am use and assigned full administrative priviledges. Moving forward this is how I will be logging into my account. 

Next, I created an alert by hooking EventBridge to Health Dashboard to SNS so that when there is a service health issue with my resources, I will be notified via mail. 

I then reviewed the questions of each pillars in the well archtected tool and answered the questions. 

Here is the napkin design 
https://github.com/patty6339/aws-bootcamp-cruddur-2023/blob/main/_docs/assets/NApkin%20Design.jpeg


