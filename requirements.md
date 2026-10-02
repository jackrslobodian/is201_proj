# Personal Website Requirements

**Status:** Agreed scope; implementation authorized October 2, 2026
**Project level:** Entry-level HTML/CSS/JavaScript project, using the friend's project as a simplicity reference
**Graduate career page:** Not required

## 1. Project goal

Create a small, professional personal website for Jack Slobodian that satisfies the course rubric while keeping the implementation understandable and appropriately basic.

The site will contain professional Bootstrap-themed pages, one hand-built college-football page, and one small interactive football app.

## 2. Agreed site structure

### `index.html` - Home page and HTML résumé

- Use Bootstrap through a pinned CDN version, plus a small custom professional stylesheet.
- Make this the public résumé and main home page. The résumé is written in HTML, not shown as a PDF.
- Keep the résumé concise and use one column with sections for Education, Experience, Leadership & Service, Awards, Skills, and Interests.
- Do not publish any contact information: omit the street address, phone number, and email address.
- Include links at the top labeled “College Football - Scratch” and “Field Goal Game.”
- Keep the listed information relevant, accurate, and easy to scan.

### `resume.html` - Legacy address

- Redirect to `index.html`, where the HTML résumé now lives.
- Include the following résumé information from the provided source document:

  - Brigham Young University Marriott School of Business, B.S. Finance, expected April 2028.
  - 3.96/4.00 GPA, full-tuition academic scholarship, Marriott School Dean's List.
  - Teaching Assistant for FIN 400 and tutor for FIN 201.
  - Experience with Snap Finance, BYU Auxiliary & Programs Technology, Vermilion Rock Advisors, Blue Ladder Capital, doTERRA, and Swish Sports.
  - Leadership/service as a volunteer representative for The Church of Jesus Christ of Latter-day Saints.
  - Skills: SQL, Tableau, Python, Excel, reporting automation, KPI dashboards, statistical analysis, and financial modeling.
  - Additional interests/credentials: dual U.S./Canadian citizenship, varsity lacrosse, Utah All-State Academic Team, and commissioner of a long-running fantasy-football league.

### `scratch.html` - College football page

- Start from a blank HTML file.
- Do not use Bootstrap markup, components, or Bootstrap CSS on this page.
- Link to a separate hand-written stylesheet, `scratch.css`.
- Use a single-column layout and short stylesheet comparable to the supplied friend's project (basic selectors, colors, fonts, margins, and padding).
- Include at least three styled/positioned `div` blocks.
- Include an ordered list containing an unordered list, or an unordered list containing an ordered list.
- Include at least one football-related image that is not supplied by a Bootstrap theme.
- Include an embedded YouTube video:
  - User-provided video, verified as “FULL GAME HIGHLIGHTS | BYU vs UTAH TECH | BYU FOOTBALL.” Label it BYU vs. Utah Tech rather than Utah.
  - `https://www.youtube.com/watch?v=lIwbv8fpDXg`
- Include an on-page anchor, such as a “Jump to the Tableau graph” link.
- Include a custom background color or background image.
- Include a live embedded Tableau visualization, not a static image:
  - `https://public.tableau.com/views/VisualizingFBSCollegeFootball/VisualizingFBSCollegeFootball?:embed=y&:display_count=yes&:showVizHome=no`
- Link back to the professional home page.
- Link to `app.html`.

### `app.html` - Simple field-goal game

- Keep the app in one page with its HTML, CSS, and JavaScript together.
- AI assistance is permitted for the game. Keep it small, with a flat canvas field, two sliders, simple functions, and no game libraries.
- Present a field-goal attempt with a visible target and a wind direction/strength.
- Let the player choose kick direction and kick power.
- Make the wind meaningfully affect the ball's final path, requiring the player to compensate.
- Animate the ball moving toward the goalposts and show feedback: made kick, miss left/right, or too short. Use simple game rules for required power and wind drift.
- Offer a five-kick challenge, 3 points per made kick, visible distance and wind, and a restart control.
- Keep the same wind and distance during an attempt; generate the next conditions only when the player advances.
- Include a reset/new-kick control.
- Use simple football styling without external game libraries.
- Link back to `scratch.html` and the professional home page.

## 3. Visual design direction

Confirmed direction: navy backgrounds, white body text, and gold headings throughout.

- Professional pages and scratch page: navy, white text, gold headings.
- App: the same palette with a green field inside the game area.
- Use strong contrast, generous spacing, readable font sizes, and consistent buttons.
- Avoid animated backgrounds, excessive gradients, tiny text, clutter, and low-contrast color combinations.
- Use responsive layouts that remain usable on a phone-sized screen.

## 4. Content and media rules

- Test every local image path, navigation link, external link, video embed, social/contact link, and Tableau embed before delivery.
- Use descriptive `alt` text for images.
- Use a meaningful fallback message when an external embed is unavailable.
- Use the user's supplied `LES.jpg` stadium photo, copied to `assets/les-stadium.jpg` without editing it.
- Keep private contact information out of all public files, source, metadata, and links. Do not copy the original résumé PDF into the website.
- Do not include the graduate-only page.

## 5. Hosting plan

- Prepare the site as a static GitHub Pages-compatible website.
- Use relative links between local pages.
- Avoid server-side code or build steps that are unnecessary for this assignment.
- Initial preference was to prepare files locally. The user subsequently authorized pushing the files to the existing repository `https://github.com/jackrslobodian/is201_proj`.
- Push the project to that repository's `main` branch. Do not configure GitHub Pages hosting as part of this push.
- Online hosting remains a future step necessary to satisfy the course's hosted-site requirement.

## 6. Rubric checklist

- [x] Professional appearance and readable contrast.
- [x] Static-site files are ready for online hosting.
- [x] Local links/assets verified; supplied video plays and Tableau loads and filters. No social/contact links included.
- [x] Résumé is present as HTML.
- [x] Scratch page is created without Bootstrap content.
- [x] Scratch page has separate custom CSS.
- [x] Scratch CSS has at least four style definitions.
- [x] Scratch CSS specifies font color and font family.
- [x] Scratch page has at least three styled `div` elements.
- [x] Nested ordered/unordered list is present.
- [x] Non-Bootstrap image is present.
- [x] YouTube video is embedded.
- [x] On-page anchor is present.
- [x] Custom background color or image is present.
- [x] Live Tableau graph is embedded.
- [x] Scratch page links back to professional pages.
- [x] Scratch page links to the interactive app.
- [x] App is in one page and has no server or network dependency.
- [x] App includes wind-affected field-goal gameplay.
- [ ] Website is hosted through GitHub Pages (a separate step after the repository push).

## 7. Simplicity and handoff

- Use plain HTML, CSS, and JavaScript. No build system, backend, game library, or framework beyond Bootstrap on the professional pages.
- Use straightforward tags and CSS on the scratch page; keep it easy for the student to read and edit. Use the friend's ZIP only as a reference for complexity, preserving Jack's own content.
- Avoid custom CSS variables, flex/grid layouts, card systems, and decorative components on the regular pages. The game uses simple canvas drawing and a short animation timer.
- The rubric permits AI help with the scratch page, but it must originate from a blank file and use no Bootstrap content.
- Include a short README with local preview and future GitHub Pages instructions.
- Verify navigation, local assets, privacy, basic mobile layout, and game outcomes. Record external embed verification limitations honestly.

