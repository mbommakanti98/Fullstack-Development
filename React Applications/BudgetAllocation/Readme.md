# Budget Allocation Application

This is a budget allocation application developed using React.js. The application allows users to segregate or allot budgets to various sectors of a firm, including Marketing, Finance, Sales, Human Resource, and IT. The application consists of several components that work together to provide a comprehensive budget management solution.

## Components

### Budget
The Budget component displays the total budget amount. It imports the AppContext and uses the useContext hook to access the budget value from the global state.

### ExpenseItem
The ExpenseItem component represents an individual expense item. It displays the name and cost of the expense. It also imports the dispatch function from the AppContext, allowing the user to delete an expense.

### ExpenseList
The ExpenseList component is responsible for rendering a list of ExpenseItem components. It uses the map function to iterate over the expenses in the state and generate ExpenseItem components accordingly.

### ExpenseTotal
The ExpenseTotal component displays the total amount spent so far. It imports the AppContext and uses the useContext hook to access the expenses from the state.

### Remaining
The Remaining component calculates and displays the remaining budget amount. It imports the budget and expenses from the AppContext and calculates the remaining value using subtraction.

### AllocationForm
The AllocationForm component allows users to add new expenses to the budget. It includes a form where users can enter the expense name and cost. When the form is submitted, an expense object is created and dispatched as the payload to update the state.

## State Management with Redux and AppContext.js

The application utilizes Redux for state management. The AppContext.js file contains the necessary logic to manage the state using the useReducer hook and the useContext hook to connect components to the context and access values from the global state.

In AppContext.js, a reducer is created to update the state based on different actions. The initial state includes the budgets for each department (Marketing, Finance, Sales, Human Resource, and IT). The Provider component is also created to wrap the components that need access to the state.

The switch statement in the reducer handles different actions, including "ADD_EXPENSE" to add a new expense, "RED_EXPENSE" to update an existing expense, and "DELETE_EXPENSE" to delete an expense from the state.

## Getting Started

To run the application, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies by running the command `npm install`.
4. Start the development server with the command `npm start`.
5. Open your browser and visit `http://localhost:3000` to access the application.

Please note that this application requires a compatible version of React.js and Redux to function correctly. Make sure to have the necessary dependencies installed before running the application.

Feel free to explore the code and customize it to suit your specific needs. Happy budget allocation!
