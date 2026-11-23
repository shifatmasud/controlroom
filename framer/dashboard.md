# Framer dashboard: v1

Project: Control Room (Framer). Page: Home (`/`).

Data comes from the Notion collection synced by Framer's official Notion plugin. Edit content in Notion, then click Sync in Framer.

## Layout

- Background `#F5F5F7`, centered column, max width 1080px, 96px top and bottom padding.
- **Header:** blue eyebrow "Control Room", 56px bold title "Your day, at a glance.", 21px grey subtitle.
- **Needs you:** collection list, filter `Pinned = true`, newest first, limit 6.
- **Latest updates:** collection list, filter `Status != Done`, newest first, limit 24.
- **Footer:** "Content from Notion · Hosted on Framer · Versioned on GitHub".

## Card

- White, 24px radius, 24px padding, soft two-layer shadow.
- Grid: auto-fill, min column 320px, 16px gap. Reflows from 3 columns to 1.
- Meta row: section chip (colour dot + name) on the left, date on the right.
- Title: Inter 20px / 600.
- Summary: Notion rich text, "Card body" preset (Inter 15px, `#6E6E73`).
- Action pill: label from the `Action` field, links to `Link` in a new tab. Hidden when Action = None.
  - Needs you: solid blue `#0071E3`, white text.
  - Latest updates: tinted blue (10%), blue text.

## Section colours

| Section | Colour |
| --- | --- |
| Mail | #0071E3 |
| Code | #AF52DE |
| Calendar | #34C759 |
| Work | #FF9500 |
| Note | #8E8E93 |

## How to act

- Mark something done: set Status = Done in Notion, then sync. It drops off the page.
- Pin something: tick Pinned in Notion. It moves to Needs you.
- Hide the button: set Action = None.
