# Capital City Quiz

## Description

The Capital City Quiz is a web application that challenges users to identify the capital cities of various countries. The quiz is implemented using Node.js, Express, and PostgreSQL, and it features a simple user interface where users can enter their answers and see their total score.

## Features

- **Quiz Functionality**: Users are presented with a country and must enter the corresponding capital city.
- **Score Tracking**: The application keeps track of the user's total score.
- **Game Over Handling**: The game displays a final score and provides an option to restart the quiz.

## Technologies Used

- **Frontend**: HTML, CSS (via `styles/main.css`)
- **Backend**: Node.js, Express
- **Database**: PostgreSQL
- **Templating Engine**: EJS
- **Middleware**: body-parser

## Getting Started

### Prerequisites

- Node.js
- PostgreSQL

### Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/RUBBOSS/Capital-City-Quiz.git
    cd Capital-City-Quiz
    ```

2. **Install dependencies**

    ```bash
    npm install
    ```

3. **Set up the PostgreSQL database**

    Create a database named `world` and ensure that the `capitals` table is populated with country-capital pairs.

    Example SQL query to create the `capitals` table:

    ```sql
    CREATE TABLE capitals (
        country VARCHAR(100),
        capital VARCHAR(100)
    );
    ```

    Populate the table with data:

    ```sql
    INSERT INTO capitals (country, capital) VALUES ('France', 'Paris');
    INSERT INTO capitals (country, capital) VALUES ('United Kingdom', 'London');
    INSERT INTO capitals (country, capital) VALUES ('United States of America', 'New York');
    ```

4. **Start the server**

    ```bash
    npm start
    ```

    The server will run at `http://localhost:3000`.

## Usage

- Open your web browser and go to `http://localhost:3000`.
- Enter the capital city of the displayed country.
- Click "SUBMIT" to check your answer and proceed to the next question.
- When the game ends, you can view your final score and restart the quiz.

## Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements or bug fixes.
