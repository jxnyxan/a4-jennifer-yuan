
# PokéCatch Adventure

This project is my fourth assignment for CS4241. It focuses on creative coding and client-side development using JavaScript, HTML Canvas, and Express.

Live Website: https://a4-jennifer-yuan.onrender.com

The goal of the application is to create an interactive Pokémon-inspired catching game where users can throw Pokéballs at moving creatures and earn points for successfully catching them.

Users can customize their gameplay experience by adjusting Pokéball speed, Pokémon movement speed, spawn rate, Pokéball size, maximum Pokémon count, and difficulty. These settings directly affect the behavior of the game.

The game includes five different creature types with different colors, point values, and catch probabilities. Players begin with 30 Pokéballs and try to catch as many creatures as possible before running out. Successfully catching a creature increases the score and creates a particle animation.

One of the main challenges I faced was implementing the game animation using the HTML Canvas API. I had to manage multiple moving objects, calculate collisions between Pokéballs and creatures, and update the game continuously without reloading the page.

Another challenge was connecting the user interface controls to the game logic so that changing the settings would immediately affect gameplay.

I used JavaScript's requestAnimationFrame() to create the animation loop and the Canvas API to draw the background, creatures, Pokéballs, and particle effects.

## Technical Achievements

- **Tech Achievement 1: HTML Canvas Game Development**
  I used the HTML Canvas API to create the entire game environment, including the grassy field, moving creatures, Pokéballs, and particle effects. All game elements are drawn dynamically using JavaScript instead of relying on static HTML elements.

- **Tech Achievement 2: Continuous Game Animation**
  I implemented an animation loop using `requestAnimationFrame()` to continuously update and redraw the game. The animation system manages creature movement, Pokéball movement, spawning, collision detection, and visual effects.

- **Tech Achievement 3: Collision Detection**
  I implemented collision detection using the distance between the center of a Pokéball and a creature. When the distance is smaller than their combined radii, the game registers a collision and attempts to catch the creature.

- **Tech Achievement 4: Randomized Catch Probability**
  Each creature type has its own catch probability and point value. The selected difficulty level changes the probability of a successful catch. This adds randomness and makes the gameplay more challenging.

- **Tech Achievement 5: Interactive Gameplay Parameters**
  I implemented six adjustable parameters using HTML sliders and a dropdown menu. Users can change Pokéball speed, creature speed, spawn rate, Pokéball size, maximum creature count, and difficulty. These settings directly affect the game while it is running.

- **Tech Achievement 6: Particle Animation Effects**
  Successfully catching a creature generates a particle animation using randomized movement and colors. The particles gradually disappear as their lifetime decreases.

- **Tech Achievement 7: Game State Management**
  I implemented game state management for starting, pausing, resuming, and restarting the game. The application also tracks the player's score, remaining Pokéballs, and total creatures caught.

## Design/Evaluation Achievements

- **Design Achievement 1: Custom Game Interface**
  I designed a Pokémon-inspired interface with a red header, dark control panel, grassy game field, and yellow highlights. The layout separates the game controls from the interactive Canvas to make the application easier to use.

- **Design Achievement 2: Responsive Layout**
  I used CSS Flexbox and media queries to create a responsive layout. On larger screens, the controls appear beside the game. On smaller screens, the controls move above the game area.

- **Design Achievement 3: Interactive Control Panel**
  I created a control panel containing five sliders and one difficulty dropdown. Each control has a descriptive label, and the sliders display their current values so users can understand the settings they are adjusting.

- **Design Achievement 4: Visual Gameplay Feedback**
  The application displays the player's score, remaining Pokéballs, and total catches. It also provides messages when a creature is caught, escapes, or when the game ends.

- **Design Achievement 5: User Instructions**
  I included a How to Play section that appears when the application first loads. The instructions explain how to start the game, throw Pokéballs, adjust settings, pause, and restart.

## W3C Accessibility Achievements

I followed accessibility recommendations from the W3C Web Accessibility Initiative (WAI) when designing and developing my game.

1. **Provide informative, unique page titles:** I used the descriptive page title "PokéCatch Adventure" to identify the application.

2. **Use headings to convey meaning and structure:** I organized the page using an H1 for the application title and H2 headings for the game settings and instructions.

3. **Provide clear instructions:** I included a How to Play section explaining how users can start the game, throw Pokéballs, catch creatures, adjust settings, and restart.

4. **Associate labels with form controls:** I associated labels with the sliders and difficulty dropdown using matching `for` and `id` attributes.

5. **Provide sufficient contrast:** I used light text on dark backgrounds and contrasting button colors to improve readability.

6. **Don't use color alone to convey information:** The game uses text messages and numerical counters to communicate scores, successful catches, and remaining Pokéballs.

7. **Make interactive elements easy to identify:** I used clearly labeled buttons for Start Game, Pause, Resume, and Restart.

8. **Identify page language:** I added `lang="en"` to the HTML element to identify the language of the page.

9. **Use markup to convey meaning and structure:** I used semantic HTML elements including `header`, `main`, `section`, and `footer`.

10. **Create designs for different viewport sizes:** I implemented a responsive layout using CSS media queries so the controls and game area adjust to smaller screens.

11. **Provide clear feedback for user input:** I included a message area that updates when the player starts, pauses, resumes, or restarts the game and when a creature is caught or escapes.

12. **Support keyboard interaction for interface controls:** I used standard HTML buttons, sliders, and a dropdown menu so the settings and game controls can be operated using a keyboard.

## Express Server

I used Express to create a simple Node.js server that serves the client-side application.

The server uses `express.static()` to serve the HTML, CSS, and JavaScript files from the public directory.

The application runs on port 3000 locally and uses `process.env.PORT` when deployed to Render.

The gameplay logic runs entirely on the client side using JavaScript and the HTML Canvas API.

## AI Use

I used ChatGPT to help plan the project, implement the HTML Canvas game, edit JavaScript animation and collision detection logic, troubleshoot errors, and improve the HTML, CSS, and Express implementation.