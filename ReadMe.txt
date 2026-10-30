Build 2026-10-30T10:00:00Z   (on top of 2026-10-30T08:00:00Z)

SQL - run in this order (Code folder):
 1. structure_document_rights_2026-10-30.sql   - BOTH companies (structural).
    Run after structure_module_rights_2026-10-30.sql. Lets the Rights Grid
    hold the new "Documents" column, and makes the delete-request table
    and the table that keeps a copy of every deleted document / entry.
 2. document_rights_flometriq_2026-10-30.sql    - FLOMETRIQ only.
    Documents admin: Suresh Subramaniam, Veenai Vimal, Karthik Raj.
    Documents user : Ramesh. A NO LOGIN FOUND row = set it in the grid.
 (If the 08:00 SQL files are not run yet, run them first.)

DOCUMENTS - won Sale Order to payment received
 Where: the Documents box on Sale Orders, and the Document Control board,
 Report by Contract, Chase Letters and Document Register.
 (Quote documents and PO / vendor documents are not part of it.)
 - Admin (no codes): add; edit any entry; unlock older entries; override
   the Out/In sequence; change Out/In; delete an entry or a whole
   document.
 - User: add; edit the latest entry; delete his OWN latest entry on the
   day he logged it. Any other delete -> "Ask to delete" with a reason.
   The Documents admins get it in the bell; they Approve or Reject at the
   top of that contract's Documents box. The answer goes to his bell.
 - Every delete keeps a copy with who / when / why. A Super Admin can
   restore it ("Deleted on this contract" in the Documents box).
 - Contract Closed (payment received): documents lock for everyone except
   the Documents admins and Super Admins.
 - The Rights Grid now has a "Documents" column; the Document Control
   screens follow it (no longer the Sale Order column).

CLEAR "YOU CAN'T DO THIS" MESSAGES
 Every block now says:
  - what you tried, and WHY it is blocked;
  - WHO can do it - with names (from roles, posts and the Rights Grid);
  - WHAT TO DO - ask them, or ask a Super Admin for the right.
 Also: code boxes name who can do it without a code; view-only screens
 say why nothing was saved and whom to ask; Add-only master screens say
 who edits / deletes; a screen with no access names whom to ask.
