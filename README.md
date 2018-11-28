# eShop
A simplified version of eBay where users are able to view, create, update, and delete item listings within a store.  This project is meant to demonstrate the use of REST APIs and how a web application is built from scratch.

The project implements the following additional features:
  * User authentication and logging
  * SQLite3 database
  * Heroku deployment

Note: Currently no web interface has been implemented yet.  Therefore to make HTTP requests to the application, [Postman](https://www.getpostman.com/) is used for interacting and testing.

---
## Quick Start
1. Clone the repo
  ```
  $ git clone https://github.com/jygh98/eShop.git
  $ cd eShop
  ```

2. Initialize and activate a virtualenv:
  ```
  $ virtualenv --no-site-packages env
  $ source env/bin/activate
  ```

3. Install the dependencies:
  ```
  $ pip install -r requirements.txt
  ```

5. Run the development server:
  ```
  $ python code/app.py
  ```

6. Navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000)

---
## Deploying to Heroku
1. Signup for [Heroku](https://api.heroku.com/signup)
2. Login to Heroku and download the [Heroku Toolbelt](https://toolbelt.heroku.com/)
3. Once installed, open your command-line and run the following command - `heroku login`. Then follow the prompts:

  ```
  Enter your Heroku credentials.
  Email: someone@gmail.com
  Password (typing will be hidden):
  Could not find an existing public key.
  Would you like to generate one? [Yn]
  Generating new SSH public key.
  Uploading ssh public key /Users/michaelherman/.ssh/id_rsa.pub
  ```

4. Activate your virtualenv

5. Create a local Git repository (if necessary):

  ```
  $ git init
  $ git add .
  $ git commit -m "initial files"
  ```

6. Create your app on Heroku:

  ```
  $ heroku create <name_it_if_you_want>
  ```

7. Deploy your code to Heroku:

  ```
  $ git push heroku master
  ```

8. View the app in your browser:

  ```
  $ heroku open
  ```

9. Having problems? Look at the Heroku error log:

  ```
  $ heroku logs
  ```
