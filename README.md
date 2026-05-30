# Cash Register

A complete cash register application that calculates change due, determines the exact coins and bills to return, and manages cash drawer inventory.

[Live Demo](https://reyrove.github.io/cash-register/)

## Features

- Calculates exact change needed
- Determines which bills and coins to return
- Displays current cash drawer status
- Shows different statuses (OPEN, CLOSED, INSUFFICIENT_FUNDS)
- Handles exact payment scenarios
- Keyboard support (Enter key)

This project was built as part of my learning journey with freeCodeCamp

## How It Works

1. The item price is displayed ($1.87 in the example)
2. Customer enters the amount of cash they provide
3. Click "Purchase" or press Enter
4. The application calculates:
   - If customer has enough money
   - Exact change due
   - Which denominations to return from the drawer
   - Current drawer status after transaction

## Cash Drawer Initial State

| Denomination | Amount |
|--------------|--------|
| PENNY | $1.01 |
| NICKEL | $2.05 |
| DIME | $3.10 |
| QUARTER | $4.25 |
| ONE | $90.00 |
| FIVE | $55.00 |
| TEN | $20.00 |
| TWENTY | $60.00 |
| ONE HUNDRED | $100.00 |

## Possible Status Results

| Status | Description |
|--------|-------------|
| OPEN | Change given, drawer still has funds |
| CLOSED | Change given, drawer is empty |
| INSUFFICIENT_FUNDS | Not enough change available |

## Valid Scenarios

- **Exact cash**: "No change due - customer paid with exact cash"
- **More than price with sufficient funds**: Shows OPEN status and change breakdown
- **More than price with exact drawer amount**: Shows CLOSED status
- **More than price with insufficient drawer**: Shows INSUFFICIENT_FUNDS
- **Less than price**: Alert message

## Technologies Used

- HTML5
- CSS3
- JavaScript

## Installation

1. Create a new folder on your computer
2. Save the following files in that folder:
   - `index.html` (the HTML structure)
   - `styles.css` (the styling)
   - `script.js` (the JavaScript logic)
3. Open `index.html` in any modern web browser

## File Structure

```
cash-register/
├── index.html
├── styles.css
├── script.js
├── README.md
├── LICENSE
└── .gitignore
```

## Usage Examples

| Cash Provided | Result |
|---------------|--------|
| $1.87 | No change due - exact cash |
| $2.00 | Status: OPEN QUARTER: $0.10 DIME: $0.02 PENNY: $0.01 |
| $5.00 | Status: OPEN ONE: $3.00 QUARTER: $0.12 DIME: $0.01 |

## Project Features

- Real-time price display
- Dynamic drawer inventory display
- Responsive grid layout for drawer items
- Input validation
- Keyboard Enter support
- Precise decimal calculations

## Browser Support

Works on all modern browsers including:
- Google Chrome
- Mozilla Firefox
- Safari
- Microsoft Edge

## Customization

You can modify:
- `price` variable to change item cost
- `cid` array to change drawer inventory
- CSS styles for different visual themes

## License

MIT License - see the LICENSE file for details

---

*Created for freeCodeCamp JavaScript Algorithms and Data Structures certification*