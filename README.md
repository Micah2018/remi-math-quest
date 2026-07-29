# Remi's Rocket Maths

A single-page, no-build maths practice site for Remi, matching the Singapore Maths worksheets he's currently working through.

## What it covers
- **Times Table Blaster** - all times tables, 1 to 12
- **Addition Launch** - addition within 20
- **Subtraction Landing** - subtraction within 20
- **Place Value Probe** - expanded form to standard form (e.g. 500 + 20 + 3), and the value of a digit in a 3-digit number
- **Division Dock** - division facts built from all times tables, 2 to 12
- **Big Number Multiply** - 2-digit x 1-digit multiplication

## How it works
Every correct answer fuels the rocket and moves it along a starfield toward the Moon, Saturn, an asteroid and finally an alien planet. Streaks build up stars and a best-streak record, so Remi always has something just out of reach to chase. The background has drifting nebula colour washes, floating planets and the occasional shooting star, and finishing a mission triggers a confetti burst.

## Parent area
A small "⚙️ Parent area" link sits in the top-right corner of the page. It's PIN-gated so Remi can't wander in by accident.

- **Default PIN: 1234.** Before you publish this, open `index.html`, search for `PARENT_PIN`, and change it to whatever you'd like.
- Inside, you can see his total stars and best streak, and a table of every question he's answered wrong, grouped by mission, with his answer, the correct answer, and how many times he's missed that exact question. The list is sorted so his most-missed questions show up first, which is the quickest way to see what to go over with him.
- A "Reset stars & streak" button clears his progress numbers without touching the missed-questions list.
- A "Clear this list" button under the missed-questions table clears that log separately.

## Where progress is stored
Stars, streak history and the missed-questions log are saved in the browser's local storage once this is hosted on GitHub Pages, so they persist between visits on the same device and browser. If local storage isn't available (for example, in some in-app previews), progress just lives for the current session instead and resets on refresh.

## Publishing to GitHub Pages
1. Create a new repo, e.g. remi2019.github.io or remi-math-quest.
2. Upload index.html to the root of the repo.
3. In the repo Settings, then Pages, set the source branch to main and folder to / (root).
4. The site will be live at https://<username>.github.io/<repo-name>/

## Extending it later
- Add a Spanish-language toggle for the times tables mission, since he's also drilling tablas in Spanish.
- Add a simple sound effect on correct answers.
- Wire star totals into the AED reward tracker already built for Micah and Remi, so maths practice earns real reward balance.
