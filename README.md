# IRS Payroll

This vault holds notes on IRS Publication 15 (2026), (Circular E), Employer's Tax Guide. It is a flat, link-based Obsidian vault: one note per section of the publication, chapter notes for sections 2, 9, 11, 13 and 17 and How To Get Tax Help, topic notes, a register of forms, one reference note for the source, and an Index. Every section note names its section and pages in the publication. The design the notes were built to belongs to the private build and is not published with them; each note carries its own sources: the section and pages of the publication it restates.

## Release

**Release 1.0, 2026-11-23**, for Publication 15 (2026).
- **Acceptance sample:** the release gate RG-P15-1 drew 25 notes at random (seed `2026-v1.0-gate`, from 86 files; the Index was redrawn). It checked every statement of those notes against the page it cites, in a fresh read-only pass.
- **Result:** 696 statements, 0 critical and 2 minor findings, a minor rate of 0.29 %, within the 2 % limit.
- **The two minor findings** are both among the 8 listed under "Known limitations" below:
  - P15-Form-945, payment with the return, p. 31;
  - P15-Introduction, the dropped "must", p. 12.

## Licence and notice

- The text of this vault is licensed CC BY 4.0.
- The source is public domain (U.S. government work, 17 U.S.C. 105).
- Attribution: Internal Revenue Service, Publication 15 (2026), Catalog Number 10000W.
- Not tax advice. Not endorsed by or affiliated with the IRS.
- No IRS logo or seal is used anywhere in this vault.

## Known limitations

Each point below is measured, and says where it comes from.

**Audit result.** Every statement of every note was checked against the page it cites, in an audit job of its own after its batch was written. A finding is critical when a reader acting on the note would do something wrong or believe something false, and minor when only the strength or scope of the wording is off, with the facts and the action unchanged. The pass rule is 0 critical findings and minor findings at most 2 % of the statements checked. The last passing audit of each of the six note batches (NB-P15-PILOT-audit, NB-P15-PILOT-T1-audit, NB-P15-B1-audit, NB-P15-B2-audit, NB-P15-B3-audit2, NB-P15-B4-audit2) counted **2,508 statements, 0 critical and 8 minor findings (0.32 %)**. One note, P15-11_When-To-Deposit, is in two of these audits (29 and 28 statements); counted once, with its later audit, the total is 2,479 statements, and the rate is still 0.32 %. The 8 minor findings are still in the notes:
- a page range one page off: P15-04-Employees-Social-Security-Number-SSN gives pp. 17–18 for the paragraph on the SSA offices in the U.S. territories, which is on p. 17;
- a table heading without the page's "taxable": P15-12-Filing-Forms-941-943-944-945, Table 3, p. 39 (the rates and wage base limits are right);
- the three "must" of the page dropped from what the publication explains: P15-Introduction, p. 12;
- the page's open list ("which include") written as the whole definition of qualified tips: P15-Whats-New, p. 2;
- a section id one level off, S13 where the sentence is in S13.01, with the page right: P15-Form-941, P15-Form-943 and P15-Form-944, p. 40;
- one case of two given as the only one: P15-Form-945, payment with the return, p. 31.

Where the exact strength or scope of a rule matters, check the cited page.

**Text basis.** The notes were written from the publication's text in reading order (pdftotext without `-layout`). In that text a word broken by a printed line-end hyphen is joined into one word, and the hyphen is gone. Two web addresses had their printed hyphen at a line end, and both were checked against the page image and the PDF's link target: IRS.gov/Newsroom/E-News-Subscriptions (p. 10), which one note had without its hyphen and which batch B3's fix corrected (P15-E-News-for-Payroll-Professionals), and IRS.gov/irb/2020-44_IRB#TD-9924 (p. 26), which no note gives as an address (P15-09_Federal-Income-Tax-Withholding names Treasury Decision 9924). Six words are left split across a line end in that text, with an empty line between their two parts (pp. 14, 16, 19, 27, 29, 53). Three more line-end hyphens are left where the rest of the word comes at another place on the same page in reading order (p. 25 twice, p. 56), and in two places the first part of a word is joined to the page's footer text, with the rest on the next line (the page number on p. 18, "Publication 15 (2026)" on p. 57). None of these split words is in a note.

**Open tasks.** Six tasks are open in the notes, one for each form reference the inventory's rule could not settle:
- four form references the rule could not resolve (G2.1): "Schedule R" twice without its form (p. 5, P15-Reminders); "Schedule B" without its form and "Form" with no form number after it (p. 37, P15-11_Deposit-Penalties);
- two form names whose end the rule could not decide (G2.2): "Forms 1099-R" (p. 9, P15-Nonpayroll-Federal-Income-Tax-Withholding) and "Schedule D (Form 941)" (p. 30, P15-09_Social-Security-and-Medicare-Taxes), each followed by a comma and more capitalised words.

For a reader: these references stay plain text, never a link to a form note, and the note does not say which form a schedule belongs to or where a printed name ends; the cited page does. The design log has no row, so no other task is open.
