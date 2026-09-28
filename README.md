# Simple Counter A simple **Counter Application** built using **HTML, CSS, and JavaScript**. This project allows users to increase and decrease a counter value while also keeping track of how many times the **Increment** and **Decrement** buttons have been clicked.

## Features

- Increment the counter
- Decrement the counter
- Counter does not go below `0`
- Counter resets to `0` after reaching `10` and clicking Increment
- Track Increment button clicks
- Track Decrement button clicks
- Increment click count resets after `10`
- Decrement click count resets after `10`
- Simple and clean user interface

## Technologies Used

- **HTML5** - Used to create the structure of the application
- **CSS3** - Used to style and design the counter
- **JavaScript** - Used to implement the counter and button functionality

## How It Works

### 1. Counter Value

The application uses a variable called `c` to store the current counter value.

```javascript
let c = 0;

When the Increment button is clicked:

c = (c >= 10) ? 0 : c + 1;

The counter increases by 1.

When the counter reaches 10, the next Increment click resets it to 0.

The Decrement button decreases the counter:

c = (c > 0) ? c - 1 : 0;

This prevents the counter from going below 0.

2. Increment Click Count

The variable ci stores the number of times the Increment button has been clicked.

let ci = 0;

Each time Increment is clicked, the value increases by 1.

After reaching 10, the next click resets the value to 0.

3. Decrement Click Count

The variable cd stores the number of times the Decrement button has been clicked.

let cd = 0;

Each time Decrement is clicked, the value increases by 1.

After reaching 10, the next click resets the value to 0.

4. Updating the Page

The update() function displays the latest values on the webpage.

function update() {
    incCount.textContent = ci;
    decCount.textContent = cd;
    count.textContent = c;
}

The JavaScript values are updated inside the HTML using textContent.
