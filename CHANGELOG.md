# Changelog

## v0.12.1

A player update. The rules and puzzles are unchanged from v0.12.

**Route tools**
- **Quieter route overlay.** The route is drawn underneath the grid, so digits and pencil marks are never covered.
  - Each room on the route shows a faint visit number instead of a badge over its top-left cell.
- **Depth bonus on the board.** Each room on the route shows its monster's bonus (for example "+2 HP").
  - Adding a room says so in the status line, for example "Room 2 is visit 4: its monster gets +1 HP".
- **Show/hide the route** with the new button or **V**. Hiding keeps your route.
  - Route mode always shows it, and clicking "Hide route" from Route mode leaves route mode and hides it.

**Door notes (new, D)**
- **Turning them on:** press **D** or click **Doors** to put a chip on every room entrance.
  - Between rooms there's one chip per direction on each internal wall.
  - Each corner room gets one more chip for entering from outside.
- **Noting candidates:** click a chip and type the monster digits that could stand in that doorway.
- **Ruling out:** **X** rules a direction out, and **Shift+X** rules out both directions through a wall. **Backspace** clears the chip.
- **Saving:** door notes are saved with your progress and work with undo.
- **Route check:** adding a route step through a doorway you ruled out shows a warning.

**Removed**
- The single-cell **Door** flag. Door notes replace it, and **D** now toggles them. Old saves drop any leftover Door flags.

## v0.12

**Rules**
- **Hold the line:** the Fighter, Rogue or Cleric must stand adjacent to the monster, keeping it busy so it can't reach the Wizard.
- **All standing:** every adventurer must still be standing after each fight. A battle plan that knocks anyone out doesn't clear the room.
- Carried over from v0.11:
  - The Fighter's Bodyguard rule follows the ally with the lowest digit (healing doesn't change it).
  - The Wizard must be in line with the monster, never adjacent.

**Player**
- A **Party** banner shows both party-wide rules.
- Fighter, Rogue and Wizard cards have **Must** panels for their position rules.
- Rules text uses exact terms: *adjacent*, *within reach* and *in line*.
- Fixed: dialogs no longer appear on launch, and the end-of-puzzle dialog's rating buttons and Close work.

**Puzzles:** five puzzles, one per difficulty grade: novem-81 (Easy), 82 (Medium), 83 (Hard), 84 (Expert) and 85 (Fiendish).

**Known issue:** difficulty grades understate the opening. The grade doesn't yet count how many room-entrance facts it takes to find the route. novem-82 is rated Medium but plays much harder.
