# MySQL Assignment

## Objective: 
Create a MySQL database for a Question & Answer forum system. This assignment focuses only on designing and implementing the database structure. This database will supports:

1. Users who can log in
2. Categories that organize questions
3. Questions posted by users
4. Answers posted by users for questions

## Required Tables:

Users: Stores user information.
* userID (Primary Key, AUTO_INCREMENT)
* username (Not null)
* password
* email

Categories: Stores question categories.
* categoryID (Primary Key, AUTO_INCREMENT)
* name
* description

Questions: Stores questions posted by users.
* questionID (Primary Key, AUTO_INCREMENT)
* title
* userID (Foreign Key → users.userID)
* categoryID (Foreign Key → categories.categoryID)
* Each question must belong to one user
* Each question must belong to one category

Answers: Stores answers for questions.
* answerID (Primary Key, AUTO_INCREMENT)
* content
* questionID (Foreign Key → questions.questionID)
* userID (Foreign Key → users.userID)

## Rules

* Each answer must belong to one question
* Each answer must belong to one user

## Relationships

* One user → many questions
* One user → many answers
* One category → many questions
* One question → many answers

## EER Diagram Requirement

After creating your database: 
1. Open MySQL Workbench
2. Use Reverse Engineering to generate an ER Diagram from your database
3. Ensure that:
* All tables are visible
* Primary keys are clearly marked
* Foreign key relationships are shown






