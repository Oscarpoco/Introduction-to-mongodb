# Codetribe Database Project

This project demonstrates the usage of MongoDB shell (Mongosh) to create and manage a database for Codetribe. It includes creating collections for `Facilitators`, `Trainees`, and `Projects`, and inserting sample documents into these collections.

## Getting Started

### Prerequisites
1. MongoDB must be installed on your machine. You can download and install MongoDB from [here](https://www.mongodb.com/try/download/community).
2. Ensure that the MongoDB server (`mongod`) is running in the background.

### Starting the MongoDB Shell (Mongosh)
To start the MongoDB shell (Mongosh), open your terminal or command prompt and run the following command:
mongosh

## Creating the Database and Collections
### 1. Create a Database named Codetribe:

Inside the MongoDB shell, run:
- use Codetribe
This will create the Codetribe database if it doesn't already exist and switch to it.

### 2. Create the Facilitators Collection and Insert a Document:

To create the Facilitators collection and insert a document:
- db.Facilitators.insertOne({
  Name: "John Doe",
  Location: "Johannesburg",
  Course: "Web Development"
})

### 3. Create the Trainees Collection and Insert a Document:

To create the Trainees collection and insert a document:
- db.Trainees.insertOne({
  Name: "Jane Smith",
  Location: "Cape Town",
  Facilitator: "John Doe"
})

### 4. Create the Projects Collection and Insert a Document:

To create the Projects collection and insert a document:
db.Projects.insertOne({
  Name: "Portfolio Website",
  Course: "Web Development",
  Lesson: "React Basics"
})

## Verifying the Inserted Documents
To check that your documents were successfully inserted, you can use the following commands:

### 1. View documents in the Facilitators collection:
db.Facilitators.find().pretty()

### 2. View documents in the Trainees collection:
db.Trainees.find().pretty()

### 3. View documents in the Projects collection:
db.Projects.find().pretty()

## Conclusion
This README.md provides instructions for setting up a MongoDB database named Codetribe, creating collections, and inserting documents using the MongoDB shell. Follow these steps to effectively manage your data in MongoDB.
