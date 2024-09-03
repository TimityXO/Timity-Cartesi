# Loan Calculator DApp

This decentralized application (DApp) implements a simple loan calculator using Cartesi Rollups technology. Users can calculate monthly payments, total payments, and total interest for a loan based on the principal amount, annual interest rate, and loan term.

## Installation

1. Clone this repository:

2. Install dependencies:
   ```
   npm install
   ```

## Interacting with the DApp

### Sending Inputs (Advance Requests)

Use the Cartesi Rollups CLI or SDK to send inputs to the DApp:

Calculate loan details:

```json
{
  "principal": 200000,
  "annualRate": 3.5,
  "loanTermYears": 30
}
```

### Response

The DApp will return a JSON object with the following information:

```json
{
  "monthlyPayment": "898.09",
  "totalPayment": "323312.18",
  "totalInterest": "123312.18"
}
```

## Implementation Details

The DApp is implemented in JavaScript and uses the following main components:

- `viem` library for hex-string conversions
- A `calculateLoan` function that performs the loan calculations
- Error handling for invalid inputs
