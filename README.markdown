# T-Rex Runner Game

A 2D endless runner game built with p5.js, inspired by Chrome's Dino game. Control a T-Rex to jump over obstacles, aim for a high score, and win at 1000 points!

## Features
- **Jump**: Press spacebar to dodge obstacles.
- **Dynamic Difficulty**: Speed increases with score.
- **Start Delay**: 5-second countdown before gameplay.
- **Victory**: Reach 1000 points to win.
- **High Score**: Saved in browser's localStorage.
- **Game Over**: Click restart button to play again.

## Setup
1. Clone the repository.
2. Ensure the `images/` folder contains all assets: `trex1.png`, `trex3.png`, `trex4.png`, `trex_collided.png`, `ground2.png`, `cloud.png`, `obstacle1.png` to `obstacle6.png`, `gameOver.png`, `restart.png`.
3. Run a local server:
   - VS Code: Use Live Server extension.
   - Node.js: Run `npx http-server`.
   - Python: Run `python -m http.server`.
4. Open `http://localhost:8000` in your browser.

## Controls
- **Spacebar**: Jump.
- **Mouse Click**: Restart after game over.

## Debugging
- Check console for `trex.y` (should be 180 when grounded) and jump triggers.
- Ensure frame rate (`getFrameRate()`) is ~60 FPS for smooth gameplay.
- Verify `images/` paths are correct in `sketch.js`.

## Known Issues
- Rapid spacebar presses may miss if T-Rex hasn't landed. Adjust `trex.y >= 140` in `keyPressed` if needed.

## Future Ideas
- Add sound effects.
- Implement double jump.
- Add pause feature.

## Credits
- Built with [p5.js](https://p5js.org/).
- Inspired by Chrome Dino Game.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

*Note*: For local text editor use with `#` as bold, replace `**` with `#` (e.g., `#Jump# instead of **Jump**), but this will render as headings on GitHub. Use this file as-is for GitHub compatibility.