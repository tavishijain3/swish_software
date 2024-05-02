# Swish

Swish is the smartest way to log in using facial recognition.

## Overview

Swish is an extension that recognizes a user whenever they try to log in to any of their accounts. Only users who have registered their face will be given the option to access the accounts. Facial recognition occurs every time the user attempts to access any of the accounts. An option to open the accounts via PIN is also provided, eliminating the need to log out every time to keep the data safe. With just a single click, users can access their accounts and keep their account password protected.

## Built With

- Django
- OpenCV
- Mediapipe
- Bootstrap

## Features

- Save Password
- Auto-Fill with Facial Recognition
- PIN Login

## Dependencies

- Chrome Browser
- Python 3.8
- Dlib

## Getting Started

### Running this app using Docker

You'll need to have Docker installed. It's available on Windows, macOS, and most Linux distributions. If you're new to Docker and want to learn more, check out the additional resources links near the bottom of this README.

If you're using Windows, it's expected that you're following along inside of WSL or WSL 2.

1. Clone this repo anywhere you want and move into the directory:
git clone https://github.com/STCVIT/Swish.git
cd SWISH-SUBMISSION
cd swish-webapp

# Optionally checkout a specific tag, such as: git checkout 0.4.0

2. Build everything:
docker build --tag swish:latest .


3. Now that everything is built, run the app with:
docker run --name swish -d -p 8000:8000 swish:latest


4. Visit http://localhost:8000 in your favorite browser to check it out.

### Running locally

1. Clone the repository:
git clone https://github.com/vinmik/Swish-Submission

2. Navigate to the project directory:
cd Swish-Submission/swish-webapp

3. Install the dependencies:
pip install -r requirements.txt

4. Start the server:
python manage.py runserver

5. Setup the initial database:
python manage.py migrate

6. Visit http://localhost:8000 in your favorite browser to access the application.

## Novelty

- Swish not only authenticates but also autofills and logs the user in for a seamless experience.
- Swish is compatible with both Chrome and Edge.
- Use of DLIB library for facial recognition ensures optimal accuracy and preprocessed images account for least errors.
- Swish webapp is disability responsive, making it accessible to people with low or limited vision.

## Future Scope and Development

- IR Sensor input for depth Perception
- Support For Android and IOS based browsers also.
- Incorporating autofill with Google Autofill or Microsoft Authenticator rather than from extension itself.
- Option to store multiple profiles of a face for multi-angle authentication.
- Incorporating decentralized authentication with the help of Block-chain and IPFS.
- Instead of just autofilling passwords, documents can also be retrieved.













