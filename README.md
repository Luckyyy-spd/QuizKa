# Quiz-KA

## Overview
Quiz-KA is a simple web-based quiz application designed to test users' knowledge on various topics. The application consists of two main pages: the home page (`index.html`) and the login page (`login.html`). Users can enter their information on the login page and start the quiz.

## File Structure
- `index.html`: The home page of the quiz application.
- `login.html`: The page where users enter their information and start the quiz.
- `style.css`:  This file contain styles for the application.

## How to Edit Questions and Answers

### Editing Questions
To modify the questions in the quiz, locate the `questions` array in the `login.html` file. This array contains the questions that will be presented to the user.

```bash
javascript
let questions = [
"What is the purpose of the title tag in HTML?",
"Which HTML tag is used to create a hyperlink?",
// Add or modify questions here
];
```

### Editing Choices
Each question has a corresponding set of answer choices stored in the `choices` array. Each sub-array corresponds to a question in the `questions` array.

```bash
javascript
let choices = [
["To define the document's heading", "To define the document's title", "To define the document's paragraph", "To define the document's image"],
["<p>", "link", "img", "button"],
// Add or modify choices here
];
```


### Editing Correct Answers
The correct answers for each question are stored in the `correctAnswers` array. Each answer corresponds to the index of the correct choice in the `choices` array.

```bash
javascript
let correctAnswers = ["b", "b", "b", "b", "d", "a", "d", "b", "a", "c"];
```

### Example of Editing a Question
If you want to change the first question and its choices, you would do the following:

1. Update the question in the `questions` array.
2. Update the corresponding choices in the `choices` array.
3. Update the correct answer in the `correctAnswers` array.

For example, to change the first question to "What does HTML stand for?", you would modify the arrays like this:

```bash
javascript
let questions = [
"What does HTML stand for?",
// other questions...
];
let choices = [
["Hyper Text Markup Language", "High Text Markup Language", "Hyper Tabular Markup Language", "None of these"],
// other choices...
];
let correctAnswers = ["a", // updated answer for the first question
// other correct answers...
];
```

## Running the Application
1. Open `login.html` in a web browser.
2. Fill in the student information form and click "Start Quiz" to begin the quiz.
3. Follow the prompts to answer the questions.

## License
This project is open-source and available for anyone to use and modify.
