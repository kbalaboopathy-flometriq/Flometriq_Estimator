BUILD 2026-10-22T04:45:00Z
On top of: 2026-10-22T02:00:00Z ("Ramya")
SQL needed: none

WHAT CHANGED - Document Control board
1. New view "By contract" (next to By stage / By person / All (list))
   - One list per LIVE contract: Pending in the Contract Register, or a Sale Order
     not closed / cancelled / on hold. Live contracts with no documents yet show
     "No documents yet".
   - Lists in contract-number order. Button "Contract no. ↑ / ↓" reverses it;
     the choice is remembered on that computer.
   - Cards inside each contract list are in due-date order and show their stage,
     hold, owner and due date.
   - List header: contract + customer, "x of y approved", Full Hold open or not.
   - Cards do not drag in this view; change stage from the card detail
     (+ Add revision). Dragging in By stage / By person is unchanged.
   - Filters, tiles, My cards only and search work here too; with a filter on,
     only contracts with matching documents are listed.
2. Card detail on double-click (desktop) or long press (phone)
   - Works on every view, on All (list) rows, in the table and in the report.
   - The detail window now also has the latest-file link next to the name.
   - The 🕘 icon still opens it.
3. Table (⊞): new "Revisions" column with ▸ / ▾ to open each document's
   revision history under its row; "Expand all revisions" and "Collapse all".
4. PDFs: "Revision history" choice - Not shown / Summary / Detailed
   - Table PDF and Report by contract (screen and PDF).
   - Summary: one column with the whole trail, e.g.
     R0 Out 28/05/2026 > R0 In 12/06/2026 Code 3 > R1 Out 20/06/2026
   - Detailed: every revision on its own line under its document
     (Rev, Out/In, date, client code, reason, by).
   - Client version: reasons and names left out unless
     "Include reasons and names" is ticked.

UNCHANGED
- By stage / By person / All (list) behave as before (drag, sort select).
- Report and table Excel files.

Manual: new article "Document Control: By contract view, card detail,
revision history" (English and Tamil).
Files to deploy: Index.html, version.txt. This ReadMe is not deployed.
