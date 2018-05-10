# FIS100Pay


![Our Application Logo](https://fisblob1.blob.core.windows.net/1hackathon/FISecure2.PNG)
# Team 
We are Team 5 for 50 united from 5 FIS locations, Jacksonville, Orlando, Bangalore, Pune, and Tunis to offer FIS for its 50th Birthday an innovative solution on mobile payments
# Problem 
The increasing adoption of mobile payments globally requires thinking about strong fraud controls, humanize payments with a personalized customer service using cognitive technologies, capitalize on the captured data to provide analytics, and automate processes to save money.
# Solution 
Our application is a security enhancement solution that can be easily plugged into any existing mobile payment application.  Our application allows the detection and tracking of specific metrics.  First it improves security by the usage of three factor authentication : password, voice, and face. Second: it provides a personalized customer experience based on emotion recognition of a customer who is using a mobile payment service. Third: it automates the capture of login details and location: further initiating customer service calls and reports on account hacks and incorrect logins.
# Technologies and architecture used
•	Artificial Intelligence Cognitive Services are the technologies mainly used.  We use Face verification algorithms, Voice verification algorithms and Emotion detection algorithms.  All of these use Convolutional Neural Networks (CNN) architecture
o	Microsoft Face Detection API was used for Emotion detection
o	VoiceIT Face and Voice verification services were used for user authentication
•	API services are used to talk to the above service providers that provide us the cognitive algorithms services
•	Mobile App development done using IONIC/Angular and Android Studio
•	Google Maps API used for reverse geocoding and location display
•	Azure blob service was used to upload images and feed them to Microsoft Face Detection API services
# What your code was written in
a.	Python was used to a limited extent
b.	Java programming was used significantly
c.  TypeScript for the UI
# Open source or proprietary software used
Open source software was used.  All of the API services that we used were free of cost.  Some were used as trial services
# What your code is designed for
Our code is designed to achieve the following:
a.	Capture a video of a user who is going to login to the mobile payments app
b.	Send the video to the VoiceIT API service for face and voice authentication
c.	If an unsuccessful login happens – then we capture the photo, location and device details of the user and store it
d.	Do some essential transactions on the mobile payments app
e.	Capture the photo, location and device details of the user when he is logging out
f.	Send the logout photo capture – to Emotion recognition services to take further action
g.	Email the user of any hack/unsuccessful login attempt – with the picture of the person who tried to login, along with the location and device details
h.	Email the user if his emotions are negative and check with him if he needs a service call
# Why it's cool
a.	Emotion recognition based service automation is futuristic.  Our app automates the process of initiating service calls based on whether a user is unhappy or dissatisfied with his last login – purely based on his facial expressions
b.	We provide a three factor login – where we use a combination of userid + password, face authentication and voice authentication
c.	We use Artificial Intelligence based cognitive services which are the happening technologies of today
d.	We integrate AI services into mobile applications seamlessly and derive value to an online mobile bank payment application
# Underlying Flow
The underlying flow of the entire application is depicted here:
![enter image description here](https://fisblob1.blob.core.windows.net/1hackathon/FISecure_flow.JPG)


==========================================================
The core face and voice authentication flow through video is depicted here below:
![enter image description here](https://fisblob1.blob.core.windows.net/1hackathon/Voiceit_flow.JPG)

# How our solution helps automation
1.  Our solution automates capturing of login coordinates capturing like device details, location, face etc. This is apart from user id and password authentication. Our solution automates the capturing of these additional pieces of information.

2.  Our solution automates the initiation of a customer service call based on the emotion of the customer when he/she logs out (after completing the transaction)

3.  Our solution automates the capturing and reporting of account hack information and incorrect login.

# How our solution helps security

1.  We would be using HTTPS protocol for all our communications with API host servers

2.  In the final solution we will be storing all API keys on the SQL server on Azure and retrieving it based on successful user login. We would then be using those API keys for using the services. This architecture would prevent reverse engineering of the tool.

3.  A key feature of our tool is a three factor security authentication i.e. Userid/Password authentication, Face authentication and Voice authentication.

4.  Another key feature of our tool is that when someone tries to hack into a primary customers account – our tool reports the hack by sending an email to the primary customer. This email has details of the device, location, time and picture of the person who tried to login to their account.

5.  Our iOS based face/voice login also provides additional level of “liveness” recognition. What this means is that you cannot use a person photo and voice recording to try to login using this tool. The person in front of the camera has to be ‘alive’ and not a static photo/voice

# How our solution can be provided as an API service
Our solution can be integrated into the spread of API services that FIS already offers. 
The flow below gives a good depiction of how our API service will work to offer our application as a service
![enter image description here](https://fisblob1.blob.core.windows.net/1hackathon/FISSecure_API.JPG)