# JavaScript IF Statements Practice
## Instructions

- Review the if statement examples shown below
- Then write your own if statements per the instructions

## Your GitHub Repo

1. Create a new GitHub repo: ***if-statements-js***

>Please make your repo **PUBLIC**.

2. Add your project files to your repo.
3. Publish your code and code updates to your online repo.
4. Submit the URL that points to your online repo on Google Classroom.

## Examples

### An IF statement

```javascript
const youEatMeat = true;
// If the user eats meat, tell them to order a hamburger!
if (youEatMeat) {
    console.log("Order a big, greasy hamburger!");
}
```

### A simple IF/ELSE statement
```javascript
const firstName = prompt("Please enter your first name:\n");
alert(`Greetings, ${firstName}!`);

if (firstName.length > 6) { 
	alert (`Wow, ${firstName}! Your first name contains ${firstName.length} characters!`);
} else {
	alert(`You have a short first name, ${firstName}!`);
}
```

### An IF/ELSE IF statement
```javascript
function checkNationality(nationality) {
  if (nationality === "US") {
    alert("You are American.");
  } else if (nationality === "UK") {
    alert("You are British.");
  } else if (nationality === "CA") {
    alert("You are Canadian.");
  } else {
    alert("Your nationality is not listed.");
  }
}

// Prompt the user for their nationality
const userNationality = prompt("Enter the code that represents your nationality: (US, UK, CA)\n");

// Call the function to check and display nationality
checkNationality(userNationality.toUpperCase()); // Convert input to uppercase using the JS toUpperCase ( ) method
```

## Write These IF Statements

You can write each code block in the same script (main.js).

### An IF statement
Write an IF statement that checks whether the user knows the Python programming language.  

Define a JS variable named *knowsPython* and set its value to either **true** or **false** depending on whether the user knows how to code in Python or not.

If the user does not know Python, display a message in the browser console that tells them they should start learning Python.

### A simple IF/ELSE statement

Write an IF/ELSE statement that checks whether the user has more than $100.00 dollars in their bank account.

Prompt the user to enter how much money they currently have in their bank account.

**HINT**: *How do you tell JavaScript to treat what the user types in as a number?*

If they have more than $100.00 in their account, display an alert box that says: Woohoo! You're rich!

Otherwise, recommend that they start adding $10.00 per week to their savings account.

### An IF/ELSE IF statement

Write a function named **checkSeason** that takes ONE **parameter** named **month**.

In the function body, create five (5) arrays: seasons, winter_months, spring_months, summer_months, fall_months

To your **seasons** array, add the values: 'winter', 'spring', 'summer', 'fall'.

To your **winter_months** array, add these values: 12, 1, 2 (representing December, January, and February).

To your **spring_months** array, add these values: 3, 4, 5 (representing March, April and May).

To your **summer_months** array, add these values: 6, 7, 8 (representing June, July and August).

To your **fall_months** array, add these values: 9, 10, 11 (representing September, October and November).

In your if clause, use the membership operator **in** to check which month corresponds to which season.  Do the same for your two elif clauses.  You should also add an else clause as the last part of your if statement in your function.
```javascript
if month in winter_months:
     return seasons[0];
elif month in spring_months:
     return seasons[1];
// and so forth...
```

Outside your function, prompt the user to enter a month number (1 - 12).
Then call the checkSeason ( ) function.   

Remember to pass the month number the user entered up to your function as an argument.

In your browser console display a message that says something such as:

> *The season for December is winter.*

> *The season for April is spring.*

**TIP**: Use a template string to build your output string.

