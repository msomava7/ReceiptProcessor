# Receipt Processor

This project is a webservice that processes receipts and calculates points based on specific rules.

## Prerequisites

- Node.js (v16 or later)
- npm (comes with Node.js)

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd receipt-processor
   ```

2. Install dependencies:
   ```
   npm install
   ```

## Running the Application

To start the server, run:

```
npm start
```

The server will start on port 5000 by default.

## API Endpoints

### Process Receipts

- **URL**: `/receipts/process`
- **Method**: POST
- **Body**: JSON Receipt object
- **Response**: JSON object containing an ID for the receipt

### Get Points

- **URL**: `/receipts/{id}/points`
- **Method**: GET
- **Response**: JSON object containing the number of points awarded

## Project Structure

- `index.js`: Main entry point of the application
- `routers/receiptRouter.js`: Contains the route handlers for receipt processing
- `models/config.js`: Database configuration (if applicable)

## Data Persistence

This application stores data in memory and does not persist data between restarts.

## Testing

To run tests (if implemented):

```
npm test
```

## Contributing

Please read CONTRIBUTING.md for details on our code of conduct, and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.