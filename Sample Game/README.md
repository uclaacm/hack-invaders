# Hack Invaders - Getting Started Workshop

**Date**: Tuesday, May 12, 2026<br>
**Teacher**: Kartik Bhatia

Hi there! Welcome to the Getting Started workshop for Hack Invaders, an intro AI hackathon where students use modern AI technologies to create retro-style games. In this workshop, we'll cover how games actually work under the hood, how to make one, and how to use AI (vibecoding!) to build your project. If you've ever wanted to make a game but didn't know where to start, you're in the right place!

## Resources
- [Slides](https://tinyurl.com/hack-invaders-intro)
- [README](https://tinyurl.com/hack-invaders-intro-readme)

## Topics Covered
- [How Games Work](#how-games-work)
- [How to Make a Game](#how-to-make-a-game)
- [Using AI (Vibecoding)](#using-ai-vibecoding)
- [Demo](#demo)
- [Next Steps](#next-steps)

## How Games Work

At their core, all games follow a simple loop:

1. **Take input** — keyboard presses, mouse clicks, typed words (e.g. WASD to move)
2. **Update game state** — process what happened (score, lives, position)
3. **Render graphics** — draw the screen based on the current game state

Take Snake as an example: the input is arrow keys, the game state tracks your score and whether you're alive, and the graphics show the snake moving around or a game-over screen when you lose.

## How to Make a Game

Building a game from scratch comes down to three steps:

1. **Pick your language or engine** — JavaScript, Python, Unreal Engine, and many others all work. For quick browser games, plain JavaScript or a small library like Three.js is a great choice.
2. **Plan it out** — think through your game mechanics, what states the game can be in, and any assets you need before diving into code.
3. **Code!** — implement your game loop: handle input, update state, and render.

## Using AI (Vibecoding)

It's 2026, and coding a game from scratch can feel daunting. The good news: AI tools can do a lot of the heavy lifting. You can use AI from:

- **The browser** — ChatGPT, Claude, Gemini, Perplexity, etc.
- **Dedicated apps** — Cursor, Claude Code, Codex, and similar tools
- **Inside your editor** — GitHub Copilot in VS Code is a great option
- **The command line** — tools like Claude Code (advanced)

One important caveat: try to actually understand what the AI has written! Blindly copy-pasting without reading the code is a fast track to mysterious bugs. Use AI as a collaborator, not a magic black box.

## Demo

For the demo, we built a **3D Snake game** in VS Code using GitHub Copilot. Here's the exact prompt used to generate the project from an empty folder:

> *"Build me a 3D snake game. I want the design to be similar to the old school snake with dark bg and a green snake. Let it move on a cube and when it hits an edge it carries on to the next side until it is looping in a square on the cube. Make sure you handle movements and corner taking gracefully. Let the cube be at the center and a small score on the top right. The folder is currently empty so set it up from scratch."*

### Steps to reproduce

1. Create a new empty folder on your computer
2. Open it in VS Code
3. Open Copilot (or your AI of choice) and paste the prompt above
4. Let the AI generate and set up the files
5. Open `index.html` in your browser and play!

The game runs entirely in the browser using HTML, CSS, and JavaScript with Three.js for 3D rendering — no install required.

## Next Steps

Now that you've seen how quickly AI can scaffold a project, here are some ways to take it further:

- **Think about your tech stack** — consider which libraries, platforms, and languages suit the game you want to build (speed, complexity, browser vs. native, etc.)
- **Learn prompt engineering** — the quality of your AI output is directly tied to the quality of your prompts. Being specific, iterative, and clear makes a huge difference. Check out our prompt engineering workshop for tips!
- **Debug and add features** — read through the generated code, understand it, and start tweaking. Add sound, a high score, new mechanics — make it yours.
- **Keep building!** — the best way to get better is to keep shipping things.

Good luck, have fun, and go build something awesome!
