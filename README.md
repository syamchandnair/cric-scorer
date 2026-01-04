# Cricket Scorer Application

A simple, responsive web-based application for scoring cricket matches. This tool allows users to track runs, wickets, overs, and match statistics in real-time with a dark-themed, mobile-friendly interface.

## Features

### Scoring

- **Runs**: Buttons for 0, 1, 2, 3, 4, and 6 runs.
- **Extras**: Dedicated buttons for Wide (WD) and No Ball (NB).
- **Wickets**: Track wickets falling.
- **Overs**: Automatic over calculation (6 legal balls per over).

### Match Management

- **Settings**:
  - **Max Overs**: Set the total overs for the innings.
  - **Players**: Set the number of players (wickets limit).
  - **Target**: Set a target score for the second innings.
- **Statistics**:
  - **CRR**: Current Run Rate.
  - **RRR**: Required Run Rate (displayed when a target is set).
  - **Current Over**: Visual history of balls bowled in the current over.
- **Controls**:
  - **Undo**: Revert the last action in case of mistakes.
  - **Next Innings**: Reset score but keep the target based on the previous innings.
  - **New Match**: Reset all data for a fresh game.

### Data Persistence

- **Local Storage**: The application automatically saves the match state. You can refresh the page or close the browser without losing data.

### Scorecard

- View a detailed history of all completed overs, including runs conceded, wickets taken, and maiden overs.

## File Structure

The application consists of three main files located in the `score` folder:

1.  **`index.html`**

    - Contains the HTML structure of the application.
    - Includes the scoreboard display, control keypad, settings inputs, and the scorecard modal.

2.  **`style.css`**

    - Provides the styling for the application.
    - Features a dark theme (`#121212` background) suitable for outdoor visibility.
    - Includes responsive grid layouts for buttons and animations for the scorecard modal.

3.  **`script.js`**
    - Handles all the game logic (scoring, over counting, run rates).
    - Manages state persistence using `localStorage`.
    - Implements the undo functionality using a history stack.

## Usage

Simply open `index.html` in any modern web browser to start scoring.
