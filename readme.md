# Minesweeper


## Getting Started
[Play the Game here](https://minesweeper-game-with-javascript.netlify.app/)!

### Basic Gameplay
1. Select your difficulty level.
* Easy = 9x9, 10 mines
* Medium = 16x16, 40 mines
* Hard = 30x30, 160 mines
2. Click anywhere on the board to begin and start the timer.
*The numbers depict how many mines are adjacent to any given cell.
3. Use **"Shift + Click"** to add flags to a cell if you think it's a mine.


### Winning/Losing
* If you hit a mine... game over, homie.
* Win by uncovering all the cells without mines!

## Technologies Used
* HTML
* CSS
* JavaScript

### HTML
As you can see from the source code, the HTML is very concise, as most of the action happens in the JavaScript. Not to mention, the gameboard itself is just a simple table.

### CSS
I had a lot of fun styling this to the old look of the Windows '95 desktop view. I still want to mess around with it a bit to get it perrrrfect (couldn't find the exact font used by MS).

My biggest challenge with the CSS was figuring out the table styles (borders, td sizes, etc.)

### JavaScript
As this was my first time ever writing a functioning web app using JavaScript, it's not a big surprise that this section was by far the greatest challenge of the project for me. 

Here are a couple highlights:

1. Dynamically sizing the table when clicking a difficulty level
* I created a function (with the help of Jim, of course) which parses the number from the ID on the table which converts it into a ${size} variable which basically appends rows/cols based on the number it grabs. This concept blew my mind.
2. In turn, dynamically creating an array of arrays to match the visual table.
3. Creating a "Cell" class which I used to create individual "cell objects" which I assigned a ton of properties to: row#, col#, bomb t/f, # of adjacent bombs (another challenge in and of itself, btw), revealed t/f, and flagged t/f.
* This approach made it a lot easier to write more concise code and not repeat myself over and over, as well as create methods on the class that would run for every cell object.
4. Creating a functional timer that displayed the seconds elapsed.
5. Randomizing bomb placement on the array.
6. Rendering everything in the DOM.
7. Assigning click handlers to different events.
8. Creating win/lose logic
9. Figuring out the control flow of how the functions are all chained together synchronously.
10. Learning about **recursion** and how to properly write a function that creates such an effect.

## My Design Choices

I decided to roll with the OG Windows '95 look, so figured for my first project I needed to walk before I could run and start with the imitation phase of the learning process.

## Thank you for reading! I hope you enjoy the game :)
