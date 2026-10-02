# Jack Slobodian's website

A small static website with four pages, prepared for the GitHub repository `jackrslobodian/is201_proj`. GitHub Pages hosting is a separate setup step.

## Files

- `index.html`: professional home page using Bootstrap and `professional.css`.
- `resume.html`: HTML résumé using the same styling. No personal contact information is included.
- `scratch.html`: college football page with its own `scratch.css`, the supplied stadium photo, nested lists, anchors, a YouTube player, and an interactive Tableau embed.
- `app.html`: a five-kick field-goal game. Its CSS and JavaScript are inside the file.
- `assets/les-stadium.jpg`: the stadium photo supplied for this project.
- `requirements.md`: project scope and rubric checklist.

## Preview locally

Open `index.html` in a browser. For a more reliable preview of external embeds, serve the folder over HTTP. If Python is installed, run this command from this folder:

```text
python -m http.server 8000 --bind 127.0.0.1
```

Then open `http://127.0.0.1:8000`. Stop the server with Ctrl+C.

Bootstrap, YouTube, and Tableau require an internet connection. YouTube may reject a file-based preview or restrict embedding of a particular video. The field-goal game works without an internet connection.

## Future GitHub Pages publishing

The repository uses the `main` branch. When ready to host the site, open repository Settings > Pages and choose `main` and its root folder as the publishing source. Confirm the resulting HTTPS site works, including video playback and Tableau interaction, before submitting it.

The scratch URL will end in `/scratch.html`, and the game URL will end in `/app.html`. Publishing remains necessary to satisfy the online-hosting portion of the rubric.

## Editing the project

The regular pages use a single column with ordinary headings, paragraphs, and lists. The scratch stylesheet uses basic colors, fonts, margins, and padding, at a similar complexity to the friend's example. Its HTML comment identifies the nested-list requirement. No build step is needed.

For the game, the wind arrow indicates the direction of the push. Aim the other way. The game uses a simple flat field and a short timer to move the ball. Longer distances require more power, and stronger wind causes more drift. More power reduces drift. The ball must finish between the posts with sufficient power. These are simplified game rules.

Keep private résumé contact details and the original résumé PDF out of the website folder before uploading.

## Verification (October 2, 2026)

Local navigation, image paths, anchors, and contact privacy were checked. Desktop and mobile layouts were reviewed. Game checks covered made/missed kicks, all 728 possible wind/distance combinations being playable, scoring, five-kick completion, repeated-click protection, and restarting during flight.

The supplied YouTube video played in the HTTP preview. Its title identifies BYU vs. Utah Tech, so the page uses that label rather than BYU vs. Utah. The Tableau embed loaded interactively, and its team filter was used to select BYU. Recheck these external services after future publishing because their availability is controlled by their hosts.
