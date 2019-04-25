# One Minute Pitch

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


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

You will need to:

-   Have python installed
-   Have PostgreSQL DB installed
-   Have a terminal to interact with the app.
-   Any text editor
-   Browser to view


Installation
========

    $ git clone https://github.com/jameskomo/one-minute-pitch.g


Build & Deployment
========

**NOTE:** You need to have fully cloned it to run it locally.


    $ ./start.sh 

    # it will launch the web page from local server. You can also visit the livelink [here](https://komo-pitch.herokuapp.com/).
 to use the system

##Built With

- Built with Python 3.6
- Flask
- Styled using Bootstrap

Behavior Driven Development (BDD)
==================================
### To update with BDD


Contribute
========

If you want to add any new features, or improve existing ones, feel free to send a pull request!

## License

MIT License

Copyright (c) 2019 James Komo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

