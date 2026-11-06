# Gen X Showdown — 900 Questions · GitHub Pages-only hosting

## Quick publishing
1. Create (or open) a **public** GitHub repository named `gen-x-showdown`.
2. Upload **index.html** to the repository root, replacing the previous index.html. You do not have to upload the other files.
3. In **Settings → Pages**, choose **Deploy from a branch**, **main**, **/(root)** and save.
4. Open `https://YOUR-USERNAME.github.io/gen-x-showdown/` on both phones.

## Two phones, no additional website account
This edition uses **native WebRTC with manual pairing** rather than a room signaling server.
1. Host taps **Create private invitation** and **Let's Play**. After a few seconds copy the invitation code.
2. Send this code to Player 2 privately, e.g. through your usual text messaging application.
3. Player 2 opens the same GitHub Pages game, taps **Accept invitation**, **Let's Play**, pastes invitation, then taps **Generate response**.
4. Player 2 copies the response code and sends it privately to the host.
5. Host pastes the response code and selects **Complete connection**. Once connected both phones switch to the shared game.
6. Keep both browser tabs open. Use **New game** for an immediate rematch.

**Honest technical limit:** GitHub Pages hosts only static HTML/CSS/JS. It has no websocket or multiplayer server. Manual WebRTC pairing bypasses server-based signaling but may **fail on restrictive NATs/mobile networks** without a TURN relay. This version uses public Google STUN for address discovery, not another hosting account. STUN availability is not guaranteed. The invitation and response codes can include IP addresses; share privately. This is casual private play, not strongly authenticated or cheatproof.

## Included improvements
* 900 questions, 150 in each of six categories; no repeat within a game.
* 24-space circular board, animated die, two player tokens, 6 wedges, bonus wedge spaces.
* Quick and Classic wedge rules; configurable 15/25/45-second or untimed questions.
* 70s disco, 80s neon, 90s pop visual themes; independent sound toggle.
* Web Audio tones (no externally copyrighted recordings), preset player reactions.
* Local automatic saving and explicit resume option; restart/rematch control.
* No external JS/CDN, user account or game backend. One self-contained index.html.
* Responsive design, keyboard focus, reduced-motion support.

## Known limitations
* No six-letter automatic multiplayer rooms can be provided by GitHub Pages alone without a signaling backend; the invite/response text exchange replaces those rooms.
* No cross-device saved-game recovery if a peer disconnects; host must stay online.
* Questions are the original 900-question set and have not received a complete independent fact-check. No fabricated question explanations were added.
* Answer data is shipped in the public HTML and can be inspected by players, so it is not cheatproof.
* Tested for JavaScript syntax and question structure. Live two-phone WebRTC connectivity has not been verified.

## Files
`index.html` = complete game, upload this file; `questions.json` = editable question bank; `questions-answers.csv` = answer key.
