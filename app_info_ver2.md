
## App Overview
- **App Name:** Quizzes
- **App Description:** This is a simple quiz app designed to test users' knowledge. The app presents list of quizes, each quiz has multiple-choice questions, allows users to use hints, and keeps track of their score and progress throughout the quiz. After answering all the questions of a single quiz, the user's final score is displayed. The app provides instant feedback after each question, indicating whether the answer was correct or not.


## Core Functionality:

### Features:
- **Multiple-choice questions**: Each question presents four possible answers, and the user selects one.
- **Hints**: Users can request a hint for each question. The app keeps track of how many hints the user has used.
- **Instant feedback**: After answering a question, users are informed if their answer was correct, along with the correct answer if they were wrong.
- **Progress tracking**: The app tracks the user's score and displays progress for each question answered.
- **Next question navigation**: Users move through questions one by one and can proceed to the next question after answering.
- **Final score**: Upon completing the quiz, the user's final score is displayed.
- **User-friendly interface**: Simple layout with buttons for selecting answers, requesting hints, and moving to the next question.

### User Stories (? User Actions?)
- **As a user**, I want to answer a series of multiple-choice questions so that I can test my knowledge of a certain topic.
- **As a user**, I want to request a hint during a question to help me answer it if I’m unsure.
- **As a user**, I want immediate feedback after I answer a question so that I know if I was correct.
- **As a user**, I want to track my progress so that I can see how well I am doing in the quiz.
- **As a user**, I want to see my final score at the end of the quiz so that I know how many questions I got right.


## App Layout and UI Elements
- **Home Screen:**  
  - **Purpose:** Displays a list of quizes available.
  - **Content:** List of all quizes available.
  - **UI Elements**:
    - App name as title
    - List of items - Each item includes a badge displaying the number of questions per quiz, background color #1e1e1e, border 1px solid #333.
  - **Navigation:** Users can tap a quiz item to go to the "quiz detail screen".

- Quiz Detail Screen:
  - Purpose: 
  - Content:
  - UI Elements:
    - Back button with icon
    - Quiz title
    - Score info
    - Progress info
    - Hints used info
    - Devider
    - Question title
    - Options - List of asnwer options
      - Option - Single answer option button
    - Show hint button
      - has a less prominent style compared to answer buttons.
    - Next question button
    - Hint text - Text of shown hint
    - Result info
  - Navigation: Users can tap a back icon to go to the "home screen".
  

## Navigation Flow
Home --> Quiz detail --> Home
Home --> Profile --> Home


## Design / Style
It includes details like color schemes (color palette), font choices, icon styles, and spacing rules.
- **Responsive Design**: The app is designed to be mobile-friendly with a simple layout that works on small screens.
- **Color palette (scheme)**: modern dark theme with primary colors centered around shades of purple.
  - **Primary Color**: `#6c63ff` (This is used for primary actions like buttons and overlay buttons).
  - **Secondary Color**: `#5753c9` (Used on hover states for primary buttons).
  - **Background**:
    - **Primary Background**: `#121212` (This is the main background color of the application for the dark theme).
    - **Secondary Background**: `#2b2b2b` (Used for input fields and the overlay content background).
  - **Text Color**:
    - **Primary Text**: `#e0e0e0` (The main color for text on standard backgrounds).
    - **Secondary Text**: `#9e9e9e` (Used for less important text, such as placeholders).
    - **Inverse Text**: `#ffffff` (Used for text on colored buttons or elements with a darker background, such as in buttons or on hover states).


## Technical specifications
- **Minimal Dependencies**: The app is built with vanilla HTML, CSS, and JavaScript, with no external libraries or frameworks required.
- SPA using "Fragmentation using HTML sections" - each screen (view) is in a separate <section> tag. When displaying a specific screen, hide the others and make the desired one visible. Use universal function "navigateToScreen(screenId)" to navigate between screens.
- Define basic UI elements in CSS by classes. 
- Use "CSS Custom Properties" for defining and using CSS variabls - main usage is for defining app's color palette. Example of the css code defining variables:
  :root {
    --primary-color: #6c63ff;
    --secondary-color: #5753c9;  
    --primary-bg-color: #121212; /*#1e1e1e*/
    --secondary-bg-color: #2b2b2b;  
    --primary-text-color: #e0e0e0; /*#fff;*/
    --secondary-text-color: #e0e0e0; /*#9e9e9e*/
    --inverse-text-color: #fff;  
    --list-item-card-bg-color: #2b2b2b;
    --list-item-card-bg-color-hover: #333;
    --list-item-card-label-bg-color: #444;
  }
- Folder and file structure:
  


## Future Enhancements (Optional)
- **Question Pool Expansion**: Add more questions to make the quiz longer or enable random question selection.
- **Timer Feature**: Introduce a timer for each question to make the quiz more challenging.
- **Score Saving**: Allow users to save and review their scores over time.
- **Difficulty Levels**: Add varying difficulty levels to the questions (easy, medium, hard).
- new data structure:
