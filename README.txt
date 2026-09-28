RED CARD 2018 — HTML/CSS ASSIGNMENT
=====================================

WHAT'S IN THIS PROJECT
-----------------------
screen1.html   - "Submission" award-nomination form page (matches screen1.png)
screen2.html   - "Red Card 2018" report / Best Clubs listing page (matches screen2.png)
style.css      - shared stylesheet used by both pages
assets/        - all image assets provided in the original zip

HOW TO RUN
----------
No build step, no server required.
1. Unzip this folder.
2. Double-click screen1.html or screen2.html to open it in any browser.
   (Or right-click -> Open with -> your browser of choice.)
Both pages load style.css and the images from the assets/ folder using
relative paths, so keep the folder structure exactly as it is.

TECH USED
---------
Plain HTML5 + CSS3 only. No frameworks (no Bootstrap/React/Vue/etc).
Font: Google Fonts "Poppins" (loaded via @import in style.css — requires
an internet connection the first time it's viewed; the page still works
fine offline, it just falls back to the default system sans-serif font).
Layout: Flexbox for both pages (badge grid on screen2 also uses flexbox
instead of CSS Grid, for the widest possible browser compatibility).

ASSETS
------
Used directly in the two pages:
  - logo.png          -> header logo (both screens)
  - icon_awards.png   -> small red triangle before each "BEST CLUBS" heading
  - 1.png             -> club badge repeated in the Best Clubs grid (screen2)

Kept in assets/ but not used on these two screens (not present in either
reference screenshot, so left untouched rather than force-fit into the
layout): 2.png, 3.png, 4.png, 5.png, premier.png, ronaldo.png, header.jpg,
footer.jpg, logo0.png. These may belong to other pages of the same site
that weren't part of this task's two reference screens.

NOTES ON THE DESIGN
--------------------
- The small white "+" square next to each award checkbox on screen1 has
  no matching image in the provided assets (icon_awards.png is a
  triangle, used correctly on screen2 instead), so it was recreated with
  plain CSS rather than substituted with an unrelated/online image.
- Colors were sampled directly from screen1.png / screen2.png (maroon
  background, dark footer bar, etc.) to match as closely as possible.
- The diagonal corner cuts (bottom-right notch on screen1's panel, and
  the header/footer notches on screen2) are done with CSS clip-path,
  matching the angles measured from the reference screenshots.
- Both pages are responsive: layout stacks to a single column and the
  badge grid re-wraps at tablet and mobile widths.
