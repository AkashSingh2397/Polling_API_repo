# PollingAPI
API for Polling Questions - Coding Ninjas Backend Skill Test Project

Task: Need to create an API where anyone can create questions with options and also add votes to it

---
## hosted link is redirecting to readme file; here i have explained everything that is needed to run the project over postman; now you have to follow the following steps over postman.

## Features
- Create a question
- Add options to a question
- Add a vote to an option of question
- Delete a question → (optional: A question can’t be deleted if one of it’s options has votes)
- Delete an option → (optional: An option can’t be deleted if it has even one vote given to it)
- View a question with it’s options and all the votes given to it

## Required Routes
- /question/create (To create a question)
- /question/:id/options/create (To add options to a specific question)
- /question/:id/delete (To delete a question)
- /options/:id/delete (To delete an option)
- /options/:id/add_vote (To increment the count of votes)
- /question/:id (To view a question and it’s options)

## Folder Structure
```
CSV_Upload/
|── |config/
│   |      ├── mongoose.js
|   |
├── routes/
│   |      ├── api/
│   ├── index.js
|   |
├── controllers/
│   ├── OptionsController.js
│   ├── QuestionsController.js
|   |
├── models/
│   ├── options.js
│   ├── questions.js
|   |
├── package-lock.json
├── package.json
├── README.md
