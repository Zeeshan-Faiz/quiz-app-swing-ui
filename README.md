# Java Swing Quiz Application

## Overview

This Java-based Quiz Application, featuring a Swing-based user interface, offers an interactive quiz experience. Users can answer a series of questions with a 10-second timer for each question. The application provides immediate feedback on answers and displays the correct answer if the user's choice is incorrect. At the end of the quiz, the final score is printed.

## Functionality

### 1. Question Asking

- The application displays a series of questions with four options.
- Questions are presented one at a time to the user.
- Each question has a timer set to 10 seconds.

### 2. Answering Questions

- Users choose their answers by selecting one of the four provided options.
- A timer counts down from 10 seconds for each question.
- If the user does not answer within the time limit, the question is marked as unanswered.

### 3. Feedback on Answers

- After answering each question, the application provides immediate feedback.
- If the answer is correct, the user receives positive feedback and can proceed to the next question.
- If the answer is incorrect or unanswered, the correct answer is displayed to the user.

### 4. Scoring

- The application keeps track of the user's score based on correct answers.
- Incorrect answers and unanswered questions are considered as negative points.
- Users can view their overall score at the end of the quiz.

### 5. Timer

- Each question is associated with a 10-second timer.
- Users must answer within the given time limit.

### 6. User-Friendly Swing UI

- The quiz interface is implemented using Java Swing for a graphical and interactive user experience.
- Clear instructions and visual elements guide users through the quiz.

## How it Works

1. **Start Quiz:**
   - Users initiate the quiz, and the first question is displayed with a 10-second timer.

2. **Answering Questions:**
   - Users select an answer within the time limit.

3. **Immediate Feedback:**
   - The application provides instant feedback on each answer.

4. **Score Tracking:**
   - The application keeps track of the user's score throughout the quiz.

5. **Correcting Mistakes:**
   - If an answer is incorrect or unanswered, the correct answer is displayed.

6. **End of Quiz:**
   - Users receive their final score and can review their answers.

## Usage Example

```java
// Sample code demonstrating how to use the Quiz application with Swing UI

@Override
	public void actionPerformed(ActionEvent e) {
		
		buttonA.setEnabled(false);
		buttonB.setEnabled(false);
		buttonC.setEnabled(false);
		buttonD.setEnabled(false);
		
		if(e.getSource() == buttonA) {
			answer = 'A';
			if(answer == answers[index]) {
				correct_guesses++;
			}
		}
		if(e.getSource() == buttonB) {
			answer = 'B';
			if(answer == answers[index]) {
				correct_guesses++;
			}
		}
		if(e.getSource() == buttonC) {
			answer = 'C';
			if(answer == answers[index]) {
				correct_guesses++;
			}
		}
		if(e.getSource() == buttonD) {
			answer = 'D';
			if(answer == answers[index]) {
				correct_guesses++;
			}
		}
		
		displayAnswer();
}
