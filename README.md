
# What is a Telegram Bot?

Bots are third-party applications that run inside Telegram. Users can interact with bots by sending them messages, commands and inline requests. 
You control your bots using HTTPS requests to Telegram Bot API.

Telegram Bots are special accounts that do not require an additional phone number to set up. 
These accounts serve as an interface for code running somewhere on your server.

# Dialogue-flow
1. Login into dialogflow console.
2. Create a new agent or import a pre-built agent.
3. From settings page of agent, open the service account of your project in Google Cloud Console.
4. Create a new service account for your project. Download private key for the service account in a JSON file.
5. Install Python Client for Dialogflow.

# News Source

pip install gnewsclient

# Deploying Flask App on Heroku

Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.

Create some new files for Heroku deployment


Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.

Create some new files for Heroku deployment
1. Procfile

A Procfile is a mechanism for declaring what commands are run by your application's dynos on the Heroku platform.
web gunicorn app:app
Also, install gunicorn in your virtual environment:
pip install gunicorn

2. runtime.txt
To specify a particular version of Python via your app's runtime.txt
python-3.7.3

3. requirements.txt
Contains all 3rd party libraries required by your app.
Simply do:
pip freeze > requirements.txt
to generate a requirements.txt file.

4. .gitignore
.gitignore file specifies patterns which are used to exclude certain files in your working directory from your Git history.

#Now, its time to create a Heroku app!

1. Setup Git repository (Download)

Initialize a new git repository in your project folder.

-git init

Add all untracked files to git repository by:

-git add .

Commit the changes to git repository by:

-git commit -m "YOUR_COMMIT_MESSAGE_HERE"

2. Create a new heroku account

3. Download Heroku CLI.

4. Create a new Heroku app.
heroku create <your-app-name>

5. Edit app.py and set webhook URL as your Heroku app's URL
bot.set_webhook("https://telegrambot.herokuapp.com/" + TOKEN)

6. Finally, you are ready to deploy your app by pushing your local git repository to the remote heroku app's git repository by:

git push heroku master

7. To check the logs of your heroku app:
heroku logs

