# Pose Exercise Web App
![image](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white) ![image](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)  ![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue) ![image](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Description
A collaboration between the proponents of the thesis titled "DEVELOPMENT OF WEB BASED APP FOR DETERMINING ANATOMICAL METRICS OF NON-LOCOMOTOR EXERCISES USING POSE ESTIMATION" for the completion of the degree of Bachelor of Science in Computer Science in Cavite State University - CCAT Campus.

## Features
- Real Time Repetition Counting Using Machine Learing
- Real Time Speed per Repetition Counting Using Machine Learing
- Calories Burned in Session
- Register and Login
- Session Records Viewing

## Requirements
- Python 
> https://www.python.org/downloads/
- NodeJS
> https://nodejs.org/en/download
- Git
> https://git-scm.com/downloads

## Creating .env.local
- under root create file and save to .env.local
```
MONGODB_URI='Your MongoDB Connection string'
JWT_SECRET='Json Webtoken String (Random Generated String)'
DB='MongoDB Database name'
COLLECTION='MongoDB Collection name'
NEXT_PUBLIC_MODEL_API='api link for modelengine default is: http://127.0.0.1:5000/predict'
```

## Installation
1. Clone the repository
> git clone https://github.com/sidex15/Thesis-Interface-nextJS.git

2. Proceed to child directory
> cd thesis-interface-nextJS

3. Install dependencies
> npm install

4. Create a python virtual environment:

 Go to src/backend
> cd src/backend

 Install python virtual environment
> pip install virtualenv

 Create virtual environment
> virtualenv -p python3 `name of virtual environment`

5. Run the virtual environment
> ./`name of virtual environment`/Scripts/activate

6. Install python dependencies
> pip install flask flask_cors joblib pandas numpy scikit-learn gevent

7. Run the backend

 Must be in src/backend
> py ModelEngine.py

8. Run the frontend

 Must be in thesis-interface-nextJS
> npm run build
>
> npm run start

9. Open the browser and test the app
> http://localhost:3000
