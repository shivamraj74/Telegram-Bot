
# What is a Telegram Bot?

Bots are third-party applications that run inside Telegram. Users can interact with bots by sending them messages, commands and inline requests. You control your bots using HTTPS requests to Telegram Bot API.

Telegram Bots are special accounts that do not require an additional phone number to set up. These accounts serve as an interface for code running somewhere on your server.

## Dialogue-flow
#### Login into dialogflow console.
#### Create a new agent or import a pre-built agent.
#### From settings page of agent, open the service account of your project in Google Cloud Console.
#### Create a new service account for your project. Download private key for the service account in a JSON file.
#### Install Python Client for Dialogflow.

## News Source
```bash
pip install gnewsclient
```
## Deploying Flask App on Heroku



Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.

### Create some new files for Heroku deployment


#### Procfile

A Procfile is a mechanism for declaring what commands are run by your application's dynos on the Heroku platform.
```bash
web gunicorn app:app
```
Also, install gunicorn in your virtual environment:
```bash
pip install gunicorn
```

#### runtime.txt
To specify a particular version of Python via your app's runtime.txt
```bash
python-3.7.3
```
#### requirements.txt
Contains all 3rd party libraries required by your app.
Simply do:
```bash
pip freeze > requirements.txt
````
to generate a requirements.txt file.

#### .gitignore
.gitignore file specifies patterns which are used to exclude certain files in your working directory from your Git history.

## Now, its time to create a Heroku app!

### Setup Git repository (Download)

#### Initialize a new git repository in your project folder.

```git init```

#### Add all untracked files to git repository by:

```-git add .```

#### Commit the changes to git repository by:

```-git commit -m "YOUR_COMMIT_MESSAGE_HERE"```

#### Create a new heroku account

#### Download Heroku CLI.

#### Create a new Heroku app.
  ```heroku create <your-app-name>```

#### Edit app.py and set webhook URL as your Heroku app's URL
  ```bot.set_webhook("https://telegrambot.herokuapp.com/" + TOKEN)```

#### Finally, you are ready to deploy your app by pushing your local git repository to the remote heroku app's git repository by:
  ```git push heroku master```

#### To check the logs of your heroku app:
  ```heroku logs```
## Screenshots of working project!
![Screenshot (57)](https://user-images.githubusercontent.com/48693624/115116468-37448100-9fb7-11eb-9f41-7dcbb4c02e7f.png)
![Screenshot (59)](https://user-images.githubusercontent.com/48693624/115116640-4415a480-9fb8-11eb-9bf3-d998fcfc8eff.png)
![Screenshot (58)](https://user-images.githubusercontent.com/48693624/115116508-74107800-9fb7-11eb-9265-32fe6cb43033.png)
## Authors

- [@Shivam Raj](https://www.github.com/shivamraj74)

  
