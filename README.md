# Heroku Practice
 
**Ok so WTF is this:**

Let's say you've made a discord bot on visual studio code but want it on 100% of the time. Heroku provides a free server (kind of like replit.com but you get to use any IDE)!
 
**Instructions:**

1. Create a requirements.txt for your repository and add `git+https://github.com/nextcord/nextcord` (whatever github library you're using) 
2. Create a Procfile.txt for your repo and add `Logs: python main.py` (make sure filename = main.py)
3. Log on to https://id.heroku.com/login and create a new app 
4. Go to Settings --> Add Buildpack --> Add Python (Or whatever language you are using)
5. Go to Deploy --> Connect with Github --> Choose the branch that you put your main.py code in
6. Deploy the branch --> Go to Resources --> Edit & turn on worker python main.py (refresh if needed)
7. Give Heroku around a minute and see your results

**Note: You have the option to use a config var (think of a .env file) to hide your API keys**

1. Go to Settings --> Config Vars --> Create a {key} to call and the api key {value}
2. In your main.py file add `import os` and `token = os.getenv('your_key')`. Call this variable wherever needed
3. Make sure to redeploy your branch so that heroku runs the updated code

<hr>

**Documentation & Other Method (Harder one in my opinion):**

- https://devcenter.heroku.com/articles/how-heroku-works
- https://www.youtube.com/watch?v=BPvg9bndP1U&t=406s
