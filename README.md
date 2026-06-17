\# Is College Worth It Here?



\## What I built

A simple web tool for first-generation UTEP students trying to figure 

out if their major is actually worth it, based on real El Paso salaries, 

not national numbers that don't apply here.



You pick a major, put in how much financial aid you're getting, choose 

how long you think you'll be in school, and it tells you how many years 

after graduation until your degree pays for itself. There's also a chart 

so you can see exactly when you break even, and you can compare two 

majors side by side.



\## Who this is for

A first-gen UTEP student from the border trying to make a real decision 

about what to study. Someone who wants honest numbers, not a sales pitch 

from an admissions office.



\## What it does

\- Pick from 14 common UTEP majors

\- Enter your financial aid so the cost is actually realistic

\- Choose 4, 5, or 6 years to graduate (most students take more than 4)

\- See how long until your degree pays off in El Paso

\- Compare two majors to see which one makes more sense financially



\## What I left out on purpose

\- Loan interest math, too complicated for this version and would need 

&#x20; real numbers from each student's loan offer

\- Live data from BLS or College Scorecard APIs, used realistic sample 

&#x20; data instead to keep it simple and focused

\- National salary comparisons — El Paso wages are what matter for 

&#x20; someone staying in this region



\## Data sources

\- BLS El Paso OEWS 2023

\- U.S. College Scorecard

\- U.S. Census ACS



Numbers are based on sample data modeled from these sources. Check your 

actual financial aid letter and current BLS data before making any real 

decisions.



\## Files

\- `index.html`: the app, just open it in a browser

\- `prompts.md`: the prompts I used in Claude Code and notes on 

&#x20; things I caught and changed along the way

