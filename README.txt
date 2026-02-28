1. Prompt 1: Planning prompt

Prompt: "How should I structure CSS media queries to handle a hero section that needs to stack vertically on mobile and a grid that changes from 4 columns to 2 to 1?"

Accepted from plan: Using flex-direction: column for the hero stacking and grid-template-columns with repeat() for the grid breakpoints.

Rejected from plan: I rejected the suggestion to use a CSS framework like Bootstrap because the assignment requirements specify "HTML and CSS only".

2. Prompt 2: Debug prompt

Problem Statement: The navigation links in the header were not aligning to the right on desktop, and the grid was overflowing the screen on mobile.

CSS Snippet asked about: .header { display: flex; } .grid { display: grid; grid-template-columns: 1fr 1fr 1fr 1fr; }

AI Response Snippet: "Use justify-content: space-between on the header to push items apart and grid-template-columns: 1fr inside a max-width: 600px media query."

Changes made: Added justify-content to the header and implemented the @media breakpoints for the grid.

3. Verification list

Viewport sizes tested: 1200px (Desktop), 768px (Tablet), 375px (Mobile/iPhone).

Visual check: Confirmed the hero card moves below the text on mobile, the grid shifts to a single column, and the navigation links center vertically.





I used the Chrome DevTools "Device Mode" to simulate different screen widths.
1200px: Verified 4-column grid and side-by-side hero layout.

768px: Verified grid snapped to 2 columns.

375px: Verified 1-column grid and vertical stacking of the header and hero.
