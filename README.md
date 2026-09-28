````markdown
# Simple Counter

A simple **Counter Application** built using **HTML, CSS, and JavaScript**.

This project allows users to increase and decrease a counter value while also keeping track of how many times the **Increment** and **Decrement** buttons have been clicked.

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
````

When the **Increment** button is clicked:

```javascript
c = (c >= 10) ? 0 : c + 1;
```

The counter increases by `1`.

When the counter reaches `10`, the next Increment click resets it to `0`.

The **Decrement** button decreases the counter:

```javascript
c = (c > 0) ? c - 1 : 0;
```

This prevents the counter from going below `0`.

### 2. Increment Click Count

The variable `ci` stores the number of times the Increment button has been clicked.

```javascript
let ci = 0;
```

Each time Increment is clicked, the value increases by `1`.

After reaching `10`, the next click resets the value to `0`.

### 3. Decrement Click Count

The variable `cd` stores the number of times the Decrement button has been clicked.

```javascript
let cd = 0;
```

Each time Decrement is clicked, the value increases by `1`.

After reaching `10`, the next click resets the value to `0`.

### 4. Updating the Page

The `update()` function displays the latest values on the webpage.

```javascript
function update() {
    incCount.textContent = ci;
    decCount.textContent = cd;
    count.textContent = c;
}
```

The JavaScript values are updated inside the HTML using `textContent`.

## Example

If the user clicks:

```text
Increment
Increment
Increment
Decrement
```

The result will be:

```text
Count: 2

Clicks of Increment: 3
Clicks of Decrement: 1
```

## Project Structure

```text
Simple-Counter/
│
├── index.html
└── README.md
```

The `index.html` file contains:

* HTML structure
* CSS styling
* JavaScript functionality

## How to Run

1. Download or clone the project.

2. Open the project folder.

3. Open `index.html` in a web browser.

4. Click the **Increment** button to increase the counter.

5. Click the **Decrement** button to decrease the counter.

## JavaScript Concepts Used

This project demonstrates basic JavaScript concepts such as:

* Variables
* Functions
* Conditional expressions
* Ternary operator
* DOM manipulation
* `getElementById()`
* `textContent`
* `onclick`
* Function calls
* Increment and decrement logic

## Future Improvements

Some features that can be added in the future:

* Add a Reset button
* Allow the user to set a custom maximum value
* Add a custom minimum value
* Add a history of counter changes
* Add different colors for positive and negative values
* Add keyboard controls
* Save the counter value using Local Storage

## Author

**Tarak Sai**

This project was created as a beginner-friendly JavaScript practice project to understand **functions, conditional logic, DOM manipulation, and event handling**.

```
```
