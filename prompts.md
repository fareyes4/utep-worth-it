Prompts Used: "Is UTEP Worth It?"

Franz | AAII Build Exercise



\---



Prompt 1: Getting Started

I'm building a small web app called "Is Utep Worth It?" for a 

first-generation UTEP student trying to decide if their chosen major is 

worth the cost at UTEP given El Paso local wages.



Here's what it should do:

\- Let the user pick a major from a dropdown

\- Show UTEP's estimated annual cost (tuition + fees)

\- Show the median salary for that major in the El Paso area 2 years 

&#x20; after graduation

\- Calculate how many years until the degree pays off

\- Show a simple verdict like "At El Paso wages, this major pays off 

&#x20; in X years"



Build this as a single HTML file with embedded CSS and JavaScript. 

Use realistic sample data for now, a dozen or so common majors with 

realistic UTEP costs and El Paso salaries from BLS/College Scorecard. 

Keep it simple and readable for a non-technical user. Start with just 

the HTML file, one working thing before adding anything else.



\---



Prompt 2: Comparison Mode, Better UI, and Data Sources

Make these three improvements to index.html:



1\. COMPARISON MODE: Add a second dropdown so the user can compare two 

majors side by side, with a clear winner at the bottom.



2\. CLEANER UI: Use UTEP's official colors (orange #F47B20 and navy 

\#041E42). Add a clean header with the app title and a one-liner 

describing who it is for. Make it look like something you'd show a 

university stakeholder.



3\. DATA SOURCES \& DISCLAIMER: Add a footer with data sources (BLS El 

Paso, College Scorecard, U.S. Census ACS) and a note that 

salary figures are sample data modeled from real sources and should be 

verified before making enrollment decisions.



Keep it as a single HTML file.



\---



Prompt 3: Break-Even Chart

Add a break-even chart using Chart.js from CDN. One line is cumulative 

degree cost, the other is cumulative wage premium earned over 10 years 

after graduation. Mark where they cross.



\---



Prompt 4: Financial Aid and Graduation Time

Two more improvements:



1\. FINANCIAL AID: Add an input field for expected annual aid or 

scholarships (default $0). Subtract it from annual cost before 

calculating break-even. Add a note: "UTEP's average net price after 

aid is around $9,000/year, check your financial aid offer letter."



2\. GRADUATION TIME: Add a dropdown for 4, 5, or 6 years to graduate 

and use that in the cost calculation. Add a note: "Only 23% of UTEP 

students graduate in 4 years, 5 or 6 years gives a more realistic 

estimate."



Don't change the chart or comparison mode. Keep it one HTML file.





Things I caught and fixed along the way



\- The AI used $30,000 as the baseline high school wage in El Paso. 

&#x20; I checked BLS and Census data and updated it to $33,000, it was 

&#x20; affecting every single breakeven calculation.



\- Made sure breakeven is measured from graduation, not from when 

&#x20; you start school, that's what actually matters to the student 

&#x20; using this tool.



\- Decided not to add a student loan interest calculator. Too many factors

&#x20; for a prototype and would have taken too long. I'd add it in a 

&#x20; real version.



\- Used sample data modeled from real sources instead of live API 

&#x20; calls, practical for a 2-3 hour build, and clearly labeled in 

&#x20; the app so users know.



\- Headings and subheadings: the original layout had unclear hierarchy 

&#x20; so I adjusted the headings to make the flow more logical and easier 

&#x20; to read for a non-technical user.



\- Median earnings: several salaries were off compared to what I found 

&#x20; in BLS El Paso OEWS data. For example some fields were too high or 

&#x20; too low for the El Paso market specifically, so I corrected them to 

&#x20; better reflect local wages rather than national averages.



\- UI colors and spacing: the initial styling felt unbalanced so I 

&#x20; adjusted the spacing between sections and made sure the UTEP orange 

&#x20; and navy were applied consistently throughout.



\- Added Chart.js for the break-even visualization: the original version 

&#x20; was text only. I decided a visual chart would make the break-even 

&#x20; concept much clearer for a student user, so I added a line chart 

&#x20; showing cumulative cost vs cumulative earnings crossing over time.



\-Noticed the graduation time dropdown limited to 4, 5, or 6 years 

even for masters degrees, which was wrong. A masters is usually 1.5 

to 2 years. Fixed it so the options change based on degree type.



