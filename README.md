# Adaptive Learning Platform

This is a Flask-based web application designed to provide an adaptive learning experience. Users take a quiz to determine their skill level, and the platform then recommends appropriate learning resources tailored to their performance. It includes user authentication, quiz assessment, course navigation, and a mini-game.

## Features

- Home page with welcome interface

- User login with basic authentication

- Quiz-based adaptive assessment

- Dynamic course recommendation based on quiz score

- Course navigation with next/previous functionality

- Congratulatory page on course completion

- Mini-game page for user engagement

## Project Structure

app.py: Main Flask application with routing logic

interfaces/: Folder containing all HTML templates

staticFolder/: Contains static assets like CSS or images

data.py: Stores course data objects

recommendation.py: Contains logic to recommend courses based on user score

congrats.py: Stores congratulatory message content

## Usage

Start the server by running the Flask application:

The app runs on localhost:5000 by default.

Navigate through the platform:

/ — Home page

/login — Login page (credentials: student / student1234)

/test — Quiz form page

/course — Course display and navigation

/game — Mini-game

/congrats — Congratulations screen after completing the course

The application stores the quiz score, evaluates the user's proficiency, and recommends content accordingly.

## Quiz & Recommendation Logic

The quiz consists of 5 questions.

Each correct answer scores one point.

The total score is passed to a recommendation function which determines the user’s level.

Based on the level, course content is selected from the dataset and displayed sequentially.

## Requirements

Python 3.x

Flask

Other files like data.py, recommendation.py, and template files are essential for the app to work.

## Authentication

Basic username-password based login is implemented.

No database is used; users are stored as a dictionary in the app.

## Note

This is a basic prototype meant for educational purposes.

Authentication and data storage can be expanded using proper databases and security measures.

