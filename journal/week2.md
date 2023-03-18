# Week 2 — Distributed Tracing
First challenge was with installing npm packages on the frontend. I tried ruuning the npm audit fix command but kept running into the problem captured in teh screenshot below

![image](https://user-images.githubusercontent.com/21007127/223156356-11a4ee0b-db26-47e8-95e0-9068eae4ab3c.png)

it finally worked

Honeycomb

![image](https://user-images.githubusercontent.com/21007127/223192577-2cdf4d4e-e635-49e8-b5c5-532712074f49.png)


I was able to receive data to my Honeycomb account

Added span to the service tab then reran the query


![image](https://user-images.githubusercontent.com/21007127/223202943-fe5ea871-07e3-4dd4-8ce6-0e1a1b197dea.png)

Aded a heatmap and P90 data and visualized on Honeycomb

![image](https://user-images.githubusercontent.com/21007127/223205774-8db029a6-0e3c-4954-9cab-9214cdc45800.png)


CONFIGURING X-Ray

![image](https://user-images.githubusercontent.com/21007127/225574794-a920e071-1f0f-4270-ad9b-03b0b3273c92.png)

X-Ray Group Added to AWS 

![image](https://user-images.githubusercontent.com/21007127/225583232-418a9b60-b501-4c6e-ab11-68886a757274.png)

Added Sampling Rule to X-Ray

![image](https://user-images.githubusercontent.com/21007127/225585606-fe57795f-521d-4fc1-ae2a-fcbbfe37799c.png)

Backend is running fine

![image](https://user-images.githubusercontent.com/21007127/225592938-2241a12d-abb1-4107-9dd5-a2d3aec76e08.png)

Send Request Failed on X-ray Deamon

![image](https://user-images.githubusercontent.com/21007127/225593730-2d06b9c7-dc52-4a78-930c-609498039631.png)

Decided to install X-Ray Deamon on Ec2  using this code:

#!/bin/bash
curl https://s3.us-east-2.amazonaws.com/aws-xray-assets.us-east-2/xray-daemon/aws-xray-daemon-3.x.rpm -o /home/ec2-user/xray.rpm
yum install -y /home/ec2-user/xray.rpm


![image](https://user-images.githubusercontent.com/21007127/225602757-b2e929de-5818-427c-8186-e5b4d481df56.png)

Cloudwatch Running Successfully

![image](https://user-images.githubusercontent.com/21007127/225756086-cb5923ca-9c1d-4add-8957-0bba915ccd23.png)

Log Events 

![image](https://user-images.githubusercontent.com/21007127/225756561-1d1c4a07-f597-4b18-ab6c-b9cc8b60f0db.png)

Rollbar running well in the browser

![image](https://user-images.githubusercontent.com/21007127/226113852-3e971711-feac-40b2-89db-747684372b17.png)





