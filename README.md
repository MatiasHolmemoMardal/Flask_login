# flask_login
## Google authentication

Before making this branch i watched a youtube-video from "Code Specialist" on the subject. Youtube:(https://youtu.be/FKgJEfrhU1E) GitHub:(https://github.com/code-specialist/flask_google_login). If you wish to introduce google authentication to your flask application i recomend checking out that video.

To run this program you will have to create your own google consent screen and OAuth Client ID. To do this, go to https://console.cloud.google.com/ login, and follow the steps bellow.
1. Create a new project.
2. Go to APIs & Services > Credentials > Configure consent screen
3. Chose Internal or External depending on your need
4. Fill in the needed information for the consent screen. For this project i only filled in the required fields and left everything else as it is.
5. Go to APIs & Services > Credentials > Create credentials > OAuth Client ID
6. Fill in the needed information for the OAuth Client ID as well as the authorized redirect URIs and press create. For this project the only autorized redirect URI is http://127.0.0.1:5000/callback.
7. Under APIs & Services > Credentials you will have the option to download the OAuth Client ID you just made in the form of a JSON file.
8. Save this file inside your project. I saved this file under the name "client_secret.json"