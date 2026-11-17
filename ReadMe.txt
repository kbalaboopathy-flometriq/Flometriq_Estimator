Build 2026-11-17T03:00:00Z  (on top of 2026-11-17T02:30:00Z)
No SQL in this build.

QUOTE / ORDER ACCEPTANCE HEADER
-------------------------------
1. Quote screen — Find box lists quotes only
   - Order Acceptance (contract) numbers such as 260116 no longer appear in the quote Find list.
   - The Order Acceptance screen already listed Order Acceptances only; unchanged.
   - "New quote" still refuses a number that already exists, OA numbers included.

2. Quote header ("Shared across all Sl Nos in this quote")
   - "Enquiry number" is now "Quote number". It shows the quote's own number (e.g. FW250108) and cannot be
     edited there.
   - Enquiry date is no longer shown, and is no longer in the header Edit / Amend forms.
     The stored enquiry date is kept (the Enquiry Register still sorts by it).

3. Order Acceptance header
   - Enquiry number and Enquiry date are gone (display and Edit / Amend forms).
   - "From quote: <quote no>" shows the quote the OA came from, as a link. Clicking it opens that quote.

4. The line above each Sl No (Quote date / Model ...)
   - Quote screen: "Quote#: <quote no>" instead of "Enquiry#"; no Enquiry date.
   - OA screen: "From quote: <quote no>"; no Enquiry date.

Nothing stored is changed or deleted — only what the screens show and let you edit.

AFTER DEPLOYING
- Open a quote: the Find list has no 26xxxx numbers; the header reads "Quote number".
- Open an OA (e.g. 260018): the header reads "From quote: FEX250316-R15"; click it to open the quote.

Tests: new header/Find test passed (quote Find lists quotes only, "Quote number: FW250108", no Enquiry
labels on quote or OA, "From quote" link opens the quote). The GRN-values test from 2026-11-16T12:00:00Z
still passes. Both script blocks pass the syntax check; the whole app renders (sign-in screen).
