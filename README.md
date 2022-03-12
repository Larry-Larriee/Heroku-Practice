# Heroku Practice
 
**Ok so WTF is this:**

Let's say you've made a discord bot on visual studio code but want it on 100% of the time. Heroku provides a free server (kind of like replit.com but you get to use any IDE)!
 
**Instructions:**

1. Create a requrements.txt for your repository and add `git+https://github.com/nextcord/nextcord` 
2. Create a Procfile.txt for your repo and add `Logs: python main.py` (make sure filename = main.py)
3. Log on to https://id.heroku.com/login and create a new app 
4. Go to Settings --> Add Buildpack --> Add Python (Or whatever language you are using)
5. Go to Deploy --> Connect with Github --> Choose the branch that you put your main.py code in
6. Deploy the branch --> Go to Resources --> Edit & turn on worker python main.py (refresh if needed)
7. Give Heroku around a minute and see your results

**Other Method (Harder one in my opinion):** 

https://www.youtube.com/watch?v=BPvg9bndP1U&t=406s

**Documentation:**

https://devcenter.heroku.com/articles/how-heroku-works
