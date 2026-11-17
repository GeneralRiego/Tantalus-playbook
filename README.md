# Tantalus Playbook Board

A tactics board for Tantalus coaches. Draw plays phase by phase, keep them in **My plays**, and make a **Playbook PDF**.

It is a single file (`index.html`) with no server and no accounts.

## Put it online with GitHub Pages

1. Create a repository (for example `playbook`) and upload `index.html` to the root.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After a minute the board is live at `https://<your-user>.github.io/playbook/`. Share that link with the coaches.

To update the board later, replace `index.html` in the repository. Coaches keep their plays.

## Where plays are saved

- Plays are saved **in the coach's own browser**, on that device only. Nobody else can see them.
- Clearing the browser's data, using private mode, or switching browser or device means the plays are not there.
- **Export** (in My plays) downloads all plays as a `.json` file. Keep it as a backup.
- **Import** loads that file on another phone or computer, or from another coach. A play with the same name is replaced.

## Making the PDF

- **My plays → Playbook PDF**: every saved play, with a cover page.
- **PDF** next to a play, or **Review phases → PDF of this play**: one play.
- The browser's print window opens. Choose **Save as PDF** (on iPhone: Share → Print, then Share again → Save to Files).
- Each phase shows the explanation typed under the court. If a phase has none, the PDF lists the actions instead (for example "2 passes to 5").

## Phone and computer

The board picks its layout from the screen width; plays are the same in both.

- **Phone:** the drawing tools, Undo, Clear, Next phase and **More** stay at the bottom of the screen. More has Show defense, Rotate defender, Full court, Review phases, Save play and PDF. ☰ opens My plays.
- **Computer (1000 px wide or more):** My plays on the left, the court in the middle with phase thumbnails underneath (click one to edit that phase), tools and the phase explanation on the right. Keys: Enter next phase, Ctrl+Z undo, ← → previous / next phase while editing, 1–8 tools.

## How to draw

- **Set start**: drag players and the ball to their starting spots. The light green border is out of bounds, for sideline and baseline plays.
- **Pass, Cut, Dribble, Screen, Hand-off**: drag from a player. **Shot**: one tap; it comes from the player with the ball.
- **Next phase** (or Enter) saves the phase; the next one starts from the end positions.
- Tap a phase chip to edit it; ◀ ▶ move between phases and save as you go.
- **+ Option**: a second ending that shares the first phases.
- **+ Defender** and **↻ Defender**: a plain red defender and the way she faces. **Show defense**: X1–X5.
- **Full court**: both baskets; the team attacks the top one.
