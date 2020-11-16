
setting up your work environment(linux):
#install text editor for easy coding,
linux alread have a text editor pre install in it but there are other obtions out there
->vim(for programing using terminal)
->atom(i use this)
->sublim text etc
#install python
      $ python3 --version
      $ sudo apt-get install software-properties-common
      $ sudo add-apt-repository ppa:deadsnakes/ppa
      $ sudo apt-get update
      $ sudo apt-get install python3.6
# Step 1: Update your repositories
sudo apt-get update
# Step 2: Install pip for Python 3
sudo apt-get install build-essential libssl-dev libffi-dev python-dev
sudo apt install python3-pip
# Step 3: Use pip to install virtualenv
sudo pip3 install virtualenv
# Step 4: Launch your Python 3 virtual environment, here the name of my virtual environment will be env3
virtualenv -p python3 django_venv
# Step 5: Activate your new Python 3 environment. There are two ways to do this
. django_venv/bin/activate # or source django_venv/bin/activate which does exactly the same thing
# you can make sure you are now working with Python 3
python -- version
# this command will show you what is going on: the python executable you are using is now located inside your virtualenv repository
which python
# Step 6: code your stuff
# Step 7: done? leave the virtual environment
deactivate
#install django
->pip3 install django.(do this when your virtual environment is active)
#start django project
-> django-admin startproject mysite(mysite will be the name of the django project)
#run django server
-> cd mysite/
->python3 manage.py runserver
copy the url and check on your browser.
->N/B you need to install vitual environment activate it and install what is in requirements.txt to run the Django program locally but if you want to deploy professionally use docker deploye.

django-tutorial-02 talks on deploying connecting with mysql data base and deploying with docker
