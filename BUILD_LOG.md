# Midway Mayhem — AI / Build Log

## Project goal
Build a small browser carnival game with a clear play loop: start a timed round, click targets for tickets, see a final score/prize result, and restart.

## Major prompts and changes

1. “Build a small finished class-assignment web game inspired by a carnival game. It needs visible state, action, feedback, an ending, and restart.” Created *Midway Mayhem*, a self-contained HTML/CSS/JavaScript target-click game.
2. “Make the game understandable without instructions from the developer.” Added the start panel, concise play directions, score/time/best-score HUD, target styling, and a visible 150-ticket goal.
3. “Make the ending and replay clear.” Added an end card with final score, prize-tier feedback, and a Play Again button that resets the round.
4. “Use a classic carnival bottle game and give ticket earnings a purpose.” Replaced bullseyes with clickable bottles; each hit earns 10 persistent tickets. Added a prize locker with replay tokens and three collectible prizes.
5. “Add sound effects without making the project hard to deploy.” Added short hit, purchase, and round-end sounds generated in the browser with the Web Audio API; no audio files or external dependencies are required.
6. “Make the booth a real toss game and broaden prize choices.” Replaced direct bottle-clicking with a click-to-throw ball animation at a standing three-bottle rack. Added Glow Wand, Plush Octopus, and Golden Trophy prizes.
7. “Let players return prizes at a discount.” Added a return button beside each owned locker item; returns pay 50% of its original ticket cost, allowing players to trade prizes back for more toss tokens.
8. “Make the bottles move so timing matters.” Added a continuously side-to-side moving bottle rack, with staggered bottle motion. Throws now use each bottle’s live on-screen position for hit detection.
9. “Compete against the AI.” Added Rival Bot, a visible green-ball opponent that throws at the same moving rack, keeps its own score, and produces a clear win/loss/tie result at round end.
10. **Human decisions:** I selected the carnival target-click concept, chose a 30-second round and ticket costs, reviewed the text and visual style, and will conduct the unfamiliar-user check below before submission.

## Human verification checklist

- [ ] Open `index.html` in a browser or deployed URL while signed out.
- [ ] Start a round; click near a standing bottle; confirm a ball animates toward the aim point and a hit raises the round score and ticket wallet by 10.
- [ ] Let the clock reach 0; confirm the round-complete card appears.
- [ ] Buy an **Another Toss** token with tickets; confirm a new round can start.
- [ ] Buy a prize; confirm it appears in **Your Locker** and ticket balance decreases.
- [ ] Return a locker prize with its ↩ button; confirm it disappears and the ticket balance increases by half its purchase cost.
- [ ] Confirm hit, purchase, and round-end sounds play when the browser is not muted.
- [ ] Check desktop and phone-width browser sizes.

## Deployment note

This is a static site. Publish this folder with GitHub Pages, Netlify Drop, or Cloudflare Pages, then paste the public URL in your assignment after confirming it works in a private/incognito window.
