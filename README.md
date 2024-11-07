# ES6-Destructuring

# React Car Stats App

This React app renders a table displaying stats for different car models, including their top speed and most popular color. The data is stored in a JavaScript object, and destructuring is used to access specific properties.

## Features

- **Car Statistics Display**: Renders car model data such as brand, top speed, and top color in a table.
- **Data Destructuring**: Uses ES6 destructuring to access data properties directly from objects, simplifying the code.

## Components and Files

### `data.js`

Contains the basic data structure for animals, each with `name` and `sound` properties. While not used in the main app functionality, it can serve as additional data.

### `index.js`

Main file where:
- Car data is imported from `practice.js`.
- Data destructuring is used to pull out relevant stats from each car object.
- The car stats are rendered in a table using React’s `ReactDOM.render()` method.

### Data Destructuring Breakdown

- `const [honda, tesla] = cars;` extracts the Honda and Tesla car objects from the imported `cars` array.
- Nested destructuring is used to pull `topSpeed` and the top color (`coloursByPopularity`) of each car, allowing direct access to these properties for rendering.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/jbolan12/ES6-Destructuring.git
    ```
2. Navigate to the project directory:
    ```bash
    cd react-car-stats-app
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm start
    ```
2. Open your browser and navigate to `http://localhost:3000` to view the app.

## Code Example

Example code showing how data is destructured and rendered:
```javascript
const [honda, tesla] = cars;
const { topSpeed: hondaTopSpeed } = honda.speedStats;
const { topSpeed: teslaTopSpeed } = tesla.speedStats;

## Dependencies
- React: 18.3.1
- React-DOM: 18.3.1
- React-Scripts 5.0.1

##License
This project is licensed under the MIT License. See the LICENSE file for details.
