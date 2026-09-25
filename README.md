
# PokéCatch Adventure

This project is my fourth assignment for CS4241. It focuses on creative coding and client-side development using JavaScript, HTML Canvas, and Express.

Live Website: https://a4-jennifer-yuan.onrender.com

The goal of the application is to create an interactive Pokémon-inspired catching game where users can throw Pokéballs at moving creatures and earn points for successfully catching them.

Users can customize their gameplay experience by adjusting Pokéball speed, Pokémon movement speed, spawn rate, Pokéball size, maximum Pokémon count, and difficulty. These settings directly affect the behavior of the game.

The game includes five different creature types with different colors, point values, and catch probabilities. Players begin with 30 Pokéballs and try to catch as many creatures as possible before running out. Successfully catching a creature increases the score and creates a particle animation.

One of the main challenges I faced was implementing the game animation using the HTML Canvas API. I had to manage multiple moving objects, calculate collisions between Pokéballs and creatures, and update the game continuously without reloading the page.

Another challenge was connecting the user interface controls to the game logic so that changing the settings would immediately affect gameplay.

I used JavaScript's requestAnimationFrame() to create the animation loop and the Canvas API to draw the background, creatures, Pokéballs, and particle effects.

## AI Use

I used ChatGPT to help plan the project, implement the HTML Canvas game, edit JavaScript animation and collision detection logic, troubleshoot errors, and improve the HTML, CSS, and Express implementation.