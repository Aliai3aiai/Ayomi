## Django Development with Docker Compose and Machine

Featuring:
- Python 3.8
- Django 3.1.1

### Overview

1. User Login Page

![Alt text](https://github.com/Aliai3aiai/Ayomi/blob/main/login.png?raw=true)

2. User Register

![Alt text](https://github.com/Aliai3aiai/Ayomi/blob/main/register.png?raw=true)

After successfully registering, user will be redirected to the Login Page

3. Home Page after login

![Alt text](https://github.com/Aliai3aiai/Ayomi/blob/main/home.png?raw=true)

User can see their username and email on the body, also on the navibar

4. Edit Profile Page

![Alt text](https://github.com/Aliai3aiai/Ayomi/blob/main/editprofile.png?raw=true)

After updating user email, user will be redirected to the home page with a message of successful update

5. Redirected Homepage

![Alt text](https://github.com/Aliai3aiai/Ayomi/blob/main/updated%20email.png?raw=true)


### OS Instructions
1. Start new machine - `docker-machine create -d virtualbox dev;`
1. Configure your shell to use the new machine environment - `eval $(docker-machine env dev)`
1. Build images - `docker-compose build`
1. Start services - `docker-compose up -d`
1. Create migrations - `docker-compose run web /usr/local/bin/python manage.py migrate`
1. Grab IP - `docker-machine ip dev` - and view in your browser
