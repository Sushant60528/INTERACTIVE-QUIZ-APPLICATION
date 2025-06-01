# INTERACTIVE-QUIZ-APPLICATION

*COMPANY*:CODETECH IT SOLUTIONS

*NAME*:SUSANTA DASH

*INTERN ID*:CT04DM1286

*DOMAIN*:FRONTED WEB DEVELOPMENT

*DURATION*:4WEEKS

*MENTOR*:NEELA SONTOSH

##The HTML part defines the user interface. It includes:

A title inside the <head>.

A div with class "app" that wraps the quiz.

An <h1> element for the quiz title.

A div with class "quiz" containing:

A placeholder <h2> for the question (id="question").

A div (id="answer-buttons") to dynamically insert answer choices as buttons.


A "Next" button (id="next-btn") that progresses through the quiz.



---

CSS Styling

The CSS file (style.css) styles the app to be clean and centered:

Uses the Poppins font and resets margins/padding.

.app has a white background, rounded corners, and is centered.

.btn styles each answer button with hover and disabled effects.

Buttons turn green (.correct) or red (.incorrect) based on whether the answer is right or wrong.



---

JavaScript Functionality

The scripts.js file (placed incorrectly in the same HTML document) contains the logic for the quiz.

1. Data Structure

An array named question holds the quiz questions. Each item has a question string and an answer array. Each answer has text and a correct boolean flag.

2. DOM Elements

JavaScript references key HTML elements:

questionElement – where the current question is displayed.

answerButtons – container for the answer options.

nextButton – progresses the quiz or restarts it.


3. Game Flow Functions

startQuiz(): Resets the index and score, sets "Next" as button text, and calls showQuestion().

showQuestion(): Displays the current question and creates buttons for answers. Correct answers are marked using dataset.correct.

resetState(): Clears old answers and hides the next button.

selectAnswer(e): Triggered when an answer is selected. It:

Marks the selected button as correct/incorrect.

Disables all buttons.

Reveals the correct answer.

Shows the next button.


showScore(): Displays the user's final score and allows replay.

handNextButton(): Moves to the next question or ends the quiz.


4. Event Handling

An event listener on nextButton determines whether to show the next question or restart the quiz.


---

Issues and Improvements

The script should be in a separate file (scripts.js) rather than embedded.

There’s a typo in "handNextButton"; a better name would be "handleNextButton".

Some typos in the questions like "Auntarctica" and "Ausia" should be corrected.



---

Conclusion

This quiz app provides a functional and visually clean way to quiz users with multiple-choice questions. It demonstrates dynamic DOM manipulation, event handling, and basic game logic using vanilla JavaScript. With slight improvements, it could be expanded to include more features like a timer, category selection, or persistent score tracking.
