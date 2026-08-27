# Midway Mayhem — AI / Build Log

## Project goal
Build a small browser carnival game with a clear play loop: start a timed round, click targets for tickets, see a final score/prize result, and restart.

## Major prompts and changes

1. “Build a small finished class-assignment web game inspired by a carnival game. It needs visible state, action, feedback, an ending, and restart.” Created *Midway Mayhem*, a self-contained HTML/CSS/JavaScript target-click game.
2. “Make the game understandable without instructions from the developer.” Added the start panel, concise play directions, score/time/best-score HUD, target styling, and a visible 150-ticket goal.
3. “Make the ending and replay clear.” Added an end card with final score, prize-tier feedback, and a Play Again button that resets the round.
4. **Human decisions:** I selected the carnival target-click concept, chose a 30-second round and 150-ticket win goal, reviewed the text and visual style, and will conduct the unfamiliar-user check below before submission.

## Human verification checklist

- [ ] Open `index.html` in a browser or deployed URL while signed out.
- [ ] Start a round; click targets; confirm score rises by 10.
- [ ] Let the clock reach 0; confirm final-score card appears.
- [ ] Choose **Play Again**; confirm time and score reset and targets return.
- [ ] Check desktop and phone-width browser sizes.

## Deployment note

This is a static site. Publish this folder with GitHub Pages, Netlify Drop, or Cloudflare Pages, then paste the public URL in your assignment after confirming it works in a private/incognito window.
