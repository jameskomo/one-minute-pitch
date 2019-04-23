![One Minute Pitch](https://cdn-images-1.medium.com/max/1200/1*ov4QOEqOhWf3OYtBbis-4w.jpeg)

 In life, you only have 60 seconds to impress someone. 1 minute can make or break you. How do you make sure that you use your 1 minute to actually say something meaningful? This Python Flask application allows users to use that one minute wisely. The users will submit their one minute pitches and other users will vote on them and leave comments to give their feedback on them. The pitches are organized by category- pickup lines, interview pitch, product pitch, promotion pitch among others. 

You can see the live Application here [One Minute Pitch](https://komo-pitch.herokuapp.com/).

Author Information
========
James Komo 

Features
========

- Built with Python 3.6, Flask microframework
- Shows Posted Pitches, Upvotes & Downvotes, Uer comments and categories.
- Styled using Bootstrap
- Uses Flask WTForms and various validators to arrest CRSF attacks.
- Uses Flask Login extension for authentication management
- Post pitches based on categories (`Choose from various pitch categories`)
- Uses PostgreSQL DB, SQLAlchemy ORM and Flask Migrate

User Stories
============
- As a user, you will be able to see the pitches other people have posted.
- As a user, you will be able to vote on the pitch you liked and give it a downvote or upvote.
- As a user, you will be required to be signed in for you to leave a comment
- As a user, you will receive a welcoming email once you sign up.
- As a user, you will be able to view the pitches you have created in your profile page.
- As a user, you will be able to comment on the different pitches and leave feedback.
- As a user, you will be able to submit a pitch in any category.
- As a user, you will be able to view the different categories.


Installation
========

    $ git clone https://github.com/jameskomo/one-minute-pitch.git


Usage
========

**NOTE:** You need to have fully cloned it to run it locally.


    $ ./start.sh 

    # it will launch the web page from local server and allow you to interact with the app
    # You can sign up on the live link and create pitches, vote and view profile



**Arguments:**

To insert BDD table



## Model Class: `User`

The `User` table has the following class attributes

- **id** - This is the primary key of the user model
- **username** - This is the user's unique username
- **email** - This is the user's unique email address
- **pass-secure** -This is the user's secure password
- **pitch** - This is the user's posted pitch. It is a foreign key in user table
- **comment** -This is the user's comments on posted pitch. It is a foreign key in user table
- **upvote** - This is the upvote tally. It is also a foreign key
- **downvotes** -This is the downvote tally. It is also a foreign key


## Model Class: `Pitch`

The `Pitch` table has the following class attributes

- **id** - This is the primary key of the pitch model class/pitch table
- **owner-id** - This is a unique id of the pitch owner which is a foreign key to user's id
- **description** - This is the pitch detailed description
- **category** -This is the  category of the pitch based on various categories defined in the system
- **pitch** - This is the user's posted pitch. It is a foreign key in user table
- **comments** -This is the users comments on posted pitches.
- **upvote** - This is the upvote tally. It is also a foreign key
- **downvotes** -This is the downvote tally. It is also a foreign key



Tests
========

To run the tests locally just do:

    $ cd app
    $ python3.6 test_user.py/test_comment.py


The tests are run on a local test server.

Contribute
========

If you want to add any new features, or improve existing ones, feel free to send a pull request!
