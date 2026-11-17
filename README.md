# Tantalus Playbook Board

A tactics board for Tantalus coaches. Draw plays phase by phase, keep them in **My plays**, and turn them into a **Playbook PDF**.

**Open the board:** https://generalriego.github.io/Tantalus-playbook/

It works on a phone and on a computer, with no account and no installation. The **?** button at the top of the board opens these instructions inside the app.

---

## For coaches

### Quick start

1. Type the play's name at the top.
2. With **Start** selected, drag the players and the ball to where the play begins.
3. Pick a tool (Pass, Cut, Dribble…) and drag from a player to draw the action.
4. Write one or two sentences in the explanation box. They go into the PDF.
5. Tap **Next phase**. The next phase starts where the players ended.
6. When the play is done, tap **Save play**.

### Drawing

| Tool | Drawn as | How |
|---|---|---|
| Start | — | Move players and defenders. Drag the orange ball onto a player to give her the ball. |
| Pass | Dashed arrow | Drag from the passer to the receiver. The ball moves with it. |
| Cut | Solid arrow | Drag along the path of a player without the ball. |
| Dribble | Zigzag | Drag along the path of the player with the ball. |
| Screen | Line ending in T | Drag from the screener to the spot. A short flick = she holds the screen where she stands. |
| Hand-off | Line ending in ‖ | Drag from the ball handler to the receiver. Drawn from the receiver to the ball handler, the ball handler waits and the receiver comes to her. |
| Shot | Double-line arrow | One tap. It comes from the player who has the ball. One shot per phase. |

- **Undo** removes the last thing you did. **Clear lines** removes all actions of the phase.
- The light green border around the court is out of bounds, for sideline and baseline inbounds plays.
- **Full court** shows both baskets. Your team attacks the top basket.

### Phases and options

- Tap a saved phase (the chips under the court on a phone, the small courts on a computer) to edit it. ◀ ▶ move to the phase before or after and save your changes on the way.
- While editing: **Save**, **Delete** the phase, or **Cancel**. Later phases follow the new end positions.
- **+ Option** makes a second ending that shares the first phases, for example a read when the defense switches. Pick the last phase both options share. The tabs Option A, B… switch between them. Shared phases can only be edited in the option they come from.
- **Review phases** shows every phase of the play with its actions, and makes a PDF of that play.

### Defenders

- **Show defense** adds X1–X5 next to their players.
- **Defender** adds one plain red defender with a tap, only in that phase, to show how to read the defense. Drag her to the edge of the board to remove her.
- **Rotate defender**: touch her and drag towards where she looks. A tap turns her 45°.

### Saving your plays — read this

- Plays are saved **only in this browser on this device**. Nothing is sent anywhere and nobody else can see them.
- **Export** (in My plays) downloads all your plays as one `.json` file. Do it now and then: it is your only backup.
- **Import** loads that file on another phone or computer, or a file from another coach. A play with the same name is replaced.
- Clearing the browser's data, private mode, or another browser or device: your plays are not there. Import your backup.
- **iPhone / iPad:** Safari can delete the saved plays of a site you haven't opened for about a week. Add the board to the Home Screen (Share → Add to Home Screen) and open it from there.
- Opened another play or started a **New play** by mistake? **Undo** brings back the play that was on the board.
- Fill in your **Team** name in My plays. It is printed on the PDF.

### PDF

- **Playbook PDF** (in My plays, or the top bar on a computer): all saved plays with a cover page.
- **PDF** next to a play, or in Review phases: one play.
- The print window opens: choose **Save as PDF**. On iPhone: Share → Print, then Share again → Save to Files.
- Each phase shows your explanation. Without one, the PDF lists the actions (for example "2 passes to 5").

### Phone and computer

The layout follows the screen width (computer layout from 1000 px). Same plays in both, as long as you use the same device and browser.

- **Phone:** tools and Next phase stay at the bottom. **More** has Show defense, Rotate defender, Full court, Review phases, Save play, PDF and How to use. ☰ opens My plays.
- **Computer:** My plays on the left, tools on the right. Keys: **Enter** next phase, **Ctrl+Z** undo, **← →** previous / next phase while editing, **1–8** tools, **Esc** closes menus.

---

## For whoever maintains the board

- The whole app is one file: `index.html` on the **`gh-pages`** branch of this repository. There is no server and no build step.
- GitHub Pages setting: **Settings → Pages → Deploy from a branch → `gh-pages` / (root)**.
- **To update:** replace `index.html` on `gh-pages`. The site refreshes within a minute or two. Coaches keep their saved plays, as long as the address stays the same.
- **Don't** rename the repository or the file, or move the site to another address: plays are stored per web address, so coaches would no longer see them (they could still import their backup).
- Saved data uses these keys in the browser's local storage: `tpb-plays` (plays), `tpb-board` (the play on the board), `tpb-team` (team name), `tpb-backup` (last export), `tpb-help-seen`.
- The export file format is `{"app":"tantalus-playbook","version":1,"team":…,"plays":[{"name":…,"data":…}]}`. Keep it readable by Import when changing the app.
