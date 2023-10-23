# interest-rate

This is a simple interest calculator for a savings account that pays varying interest rates based on the balance of the account. The interest rates are defined as follows:

- < $1,000: 1%
- $1,000 - < $5,000: 1.5%
- $5,000 - < $10,000: 2%
- $10,000 - < $50,000: 2.5%
- $50,000 and above: 3%

## Getting Started

### Prerequisites

- Node.js and npm should be installed on your machine.
- Assuming using a JavaScript/TypeScript environment, we are using Jest for testing.

`npm install --save-dev jest @types/jest ts-jest typescript`

- Run Tests
`npm test`

### Installation

1. Clone this repository or download the ZIP file.
2. Navigate to the project directory in your terminal.
3. Run `npm install` to install the required dependencies.

## Usage

To calculate the interest for a given balance, use the `calculateInterest` function. The function takes a single argument, which is the account balance, and returns the calculated interest in dollars and cents.

```javascript
const { calculateInterest } = require('./interestCalculator');

const balance = 1001;
const interest = calculateInterest(balance);
console.log(`Interest for $${balance} is $${interest.toFixed(2)}`);
