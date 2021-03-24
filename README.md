# Pre-work - _Memory Game_

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program.

Submitted by: Sharon Sanchez

Time spent: 14 hours hours spent in total

Link to project: 
1. For the code (https://glitch.com/edit/#!/memory-game2)
2. For the live game (https://memory-game2.glitch.me) 

## Required Functionality

The following **required** functionality is complete:

- [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
- [x] "Start" button toggles between "Start" and "Stop" when clicked.
- [x] Game buttons each light up and play a sound when clicked.
- [x] Computer plays back sequence of clues including sound and visual cue for each button
- [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess.
- [x] User wins the game after guessing a complete pattern
- [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

- [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
- [x] Buttons use a pitch (frequency) other than the ones in the tutorial
- [x] More than 4 functional game buttons
- [x] Playback speeds up on each turn
- [x] Computer picks a different pattern each time the game is played
- [x] Player only loses after 3 mistakes (instead of on the first mistake)
- [ ] Game button appearance change goes beyond color (e.g. add an image)
- [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
- [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [x] Change the color of the background and changed the sizing than the tutorial to make it more appealing
- [x] Added a bit more instructions so the user can understand better on how to play!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

![When the player makes mistakes and loses](http://g.recordit.co/LopKafxBXQ.gif)
![The player goes through the entire game, it is a 12 step pattern going faster](http://g.recordit.co/Adpjnpd3ip.gif)


## Reflection Questions

1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.
   
   I used mainly w3schools.com on the HTML, Javascript, and CSS sections to make my project look neater and change the appearances
   with the optional features. An example for w3schools.com is this page where it gives the list of colors the code supports. 
   https://www.w3schools.com/colors/colors_names.asp
   I also used stackoverlow to see how certain ideas are done to implement the optional features such as the random patterns:
   https://stackoverflow.com/questions/21816595/how-to-generate-a-random-number-of-fixed-length-using-javascript
   Finally, I used repl.it to test some code so I can visualize and practice so I don't mess up the project code, I used it to 
   practice on the random pattern feature and understand how certain commands worked (I only use the js section to use console):
   https://replit.com/join/yvsimues-sharons3

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)
   
   The challenge was the random code generator feature. I had the idea where if there was originally a pattern of 8 with 4 buttons, there would be a pattern of 12
   with 6 buttons. I had to look up how for loops worked and how to append items on a list with javascript using w3schools. I erased the original pattern from the pattern list so the program understands 
   that we have started with an empty pattern since the randomization has not occurred yet. I created the function patterngenerator() to house the for loop where it was from index 0 to 12 (I want 12 integers and the list starts at index 0), 
   generate a random number and append it to the list. Problem one was that I originally did not use Math.floor which told the program to only print out integers. As a result, decimal numbers were added to the list and the pattern did not play 
   because the buttons are assigned as integers. So I went back to w3schools to research on the MATH functions and decided to use a repl.it page to visualize and experiment how the commands worked. 
   Second thing was after the 1st problem was solved, the pattern played and stopped immediately giving me an error that the function patterngenerator() did not exist. I saw that I placed the function after the function
   has been called in the startgame() function so I moved it before it was called and it worked successfully. 
   
3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)

   I do want to know how to implement pictures appearing as the user clicks on the buttons. I successfully uploaded images on the asset folder and make them invisible on the .css page
   if it is not clicked but I could not get them to appear after attempting to add it to the onclick feature to the buttons on the .html page (pictures and code was left so feel free to check it out!).
    Being new to web development, I would like tips on how to make code look cleaner and less repetitive so it is not "spaghetti code" because I would love to make complicated projects without having to worry about crashes or slowdowns on a website. 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)
   
   I would definitely try to solve the optional features I didn't get to for the project just to make it more challenging and interactive for the user. I was
   close to implementing the images to appear when the user clicks on the button. I also would like to implement a menu before the game starts where the user can pick a 
   one or two player mode where the user plays by himself or with a friend to compete on how far they can go with memorizing the pattern. To do this, there would also need to 
   be a point system  recommended where each new button added to the pattern and guessed correctly adds to one point. I was reading a blog where they shared their code on a cool feature that gives
   a button or animation where pressing on a button/card flips over to show a picture. That would also be a nice feature to smooth out the game. You can see it here where it was developed by Nate Wiley! : https://codepen.io/natewiley/pen/HBrbL
    

## License

    Copyright [Sharon Sanchez]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
