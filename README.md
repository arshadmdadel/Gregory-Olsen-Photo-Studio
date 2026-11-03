# Gregory Olsen Photo Studio: QA Testing Project

Manual QA project on the **Gregory Olsen Photo Studio** website, a photographer's portfolio and session-booking site, completed as part of the SQA training program at the A1QA training center (QATC).

## Overview

The site presents a photographer's work and lets visitors book a photo session. This repository documents the testing performed and the defects found in version **1.0**.

## Application Areas Under Test

- **Home**: preview photos linked to their galleries.
- **Work galleries**: Portrait, Lifestyle, Motion and others, with photo previews, pagination, an expand/lightbox view and navigation buttons.
- **Clients**: client gallery with links to each client's destination page.
- **Bio & Press** and **Philanthropy**: content pages.
- **Contact**: contact form with first name, last name, email, phone and message fields.
- **Book a Session**: choose a session type (Standard or Mini Studio), set additional subjects, then fill in the Book Information form and continue to payment.
- **Header, footer and search**: navigation, search box, logout option and external links such as InstaOlsen.

## Scope of Testing

| Type | Focus |
|------|-------|
| Functional | Booking flow, price calculation, form validation, search, pagination, links and navigation |
| GUI | Layout, image sizes, language of interface text, page titles, placeholder and hover behavior |
| Content | Missing content, typos, wrong or missing images |
| Negative / boundary | Whitespace-only input, special characters, wrong data types, field length limits |

## Test Environment

| Item | Details |
|------|---------|
| OS | Windows 11 (64-bit) |
| Browser | Google Chrome 150.0.7871.115 |
| Application version | 1.0 |
| Defect tracking | Jira (project: Training Center, component: GregOlsen.PhotoStudio) |

## Defect Summary

**40 defects** were reported, all currently **Open**.

| Priority | Count |
|---|---|
| Major | 21 |
| Minor | 18 |
| Trivial | 1 |

| Error type | Count |
|---|---|
| Functional | 29 |
| GUI | 11 |

### Defect categories

| Category | Examples |
|----------|----------|
| Booking and Book Information form | Required fields accept only spaces; fields accept special characters, numbers or wrong data types; optional Company field is treated as required; "Save this information" checkbox cannot be checked; newsletter checkbox is checked by default; wrong session photo shown; total price miscalculated with additional subjects; Additional Subjects dropdown has 7 values instead of 10 |
| Payment | Payment page not found |
| Contact form | First name validation missing; generic browser message instead of the specified custom message; last name limited to 8 characters; search box layout broken |
| Work galleries | Preview buttons appear in Russian instead of English; expand button missing on some previews; no photo-number tooltip; Motion page does not load |
| Portrait and Lifestyle galleries | Wrong photo shown on page 1; image order broken on page 3; "Next" on page 3 loops back to page 2; no navigation between photos in single view; preview size does not match the 225px by 130px requirement |
| Clients | Links cross-mapped or not working; two galleries missing from the list; page title is "Clients" instead of "Clients Gallery" |
| Content pages | Bio & Press has no content; Philanthropy article has typos and a missing client quote |
| Header, footer and search | Header search box not functional; placeholder text not shown after the cursor leaves; no logout option; session tab missing on the Contact page; footer missing on the Connect page; hover shows the URL in the status bar; InstaOlsen redirect URL differs from the requirement |

## Defect Report Format

Each defect was logged in Jira with:

- Title and summary
- Steps to reproduce
- Actual result and expected result
- Environment (OS, browser)
- Priority, severity, and error type (Functional / GUI)
- Screenshots as attachments

## Skills Demonstrated

- Functional, GUI and content testing
- Requirement-based verification (sizes, URLs, dropdown values, messages)
- Form validation and boundary testing
- Clear, reproducible bug reporting
- Defect tracking in Jira

## Author

**Arshad Md. Adel**: SQA trainee, CSE graduate of United International University (UIU).
