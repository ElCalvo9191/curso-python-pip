# Create the file

```sh
$ mkdir py-proyect
$ touch README.md
```
# Create a SSH Connection
## Check if you have your email linked with git.

```sh
$ git config -l
```
If you email is linked omit the next step
## Lets link the email

```sh
$ git config --global user.email "Your @ email.com"
```
## Create SSH key

```sh
$ ssh-keygen -t rsa -b 4096 -C "Your @ email.com"
```
Select the default file to save the key and assign a passphrase

## Check and add the key

```sh
$ eval $(ssh-agent - s)
$ ssh-add ~/.ssh/id_rsa
```
# Link the file with git and github

Start linking with local git being in py-game file.
```sh
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin "Your SSH link"
$ git push -u origin main
```
# Game Project

Go to the file game
```sh
$ cd game
```
Execute  main.py 
```sh
$ python3 main.py
```
# Install Virtual Environment

To be able to have different version for your requiremnt in your projects at the same time, make the next step.

```sh
$ sudo apt install -y python3-venv
```
# App Project

```sh
$ git clone 
$ cd app 
$ python3 -m venv env 
$ source env/bin/activate
$ pip3 install -r requirements.txt
$ python3 main.py
```
To get out from env enveironment use.
```sh
$ deactivate
```