# Who Has the Wealth?

An interactive guess-first activity about the U.S. wealth distribution. Students imagine the country as 100 households sharing $100, divide the money the way they think it’s really divided, and then see the Federal Reserve’s figures. By Gwen Sharp, as a companion to Chapter 4 (Social Class, Inequality, and Poverty) of *A Sociology Experiment*.

**Live site:** https://gsharpokie.github.io/wealthdistribution/

## What it does

- **Your guess:** students split $100 among four groups of households: the 50 least wealthy, the next 40, the next 9, and the single wealthiest.
- **A live pie chart** next to the sliders updates as students hand out the $100 (money not yet handed out shows in gray).
- **The real split:** three pie charts (the 100 households by group, the student’s guess, and the actual split), then the guess and the actual split as two bars on the same scale, a table of dollars per household, and a note on their biggest miss.
- **The fuller picture:** what Americans guessed and preferred in Norton and Ariely’s 2005 survey; the top 1%’s record share; the bottom half’s recovery from its 2010–2012 low; and why wealth isn’t the same as income (age, Social Security).
- **Discussion questions.**

## For instructors

To show the answer without guessing (for example, on a projector), add `#answer` to the link: https://gsharpokie.github.io/wealthdistribution/#answer

## Data

- Federal Reserve Board, Distributional Financial Accounts, share of household net worth, 2026:Q2 (released September 18, 2026): bottom 50%, 2.3%; 50th–90th percentiles, 28.8%; 90th–99th, 36.4%; top 1%, 32.5%. https://www.federalreserve.gov/releases/z1/dataviz/dfa/
- History (top 1% at 22.8% in 1989; bottom 50% at 3.5% in 1989 and 0.4% in 2010–2012): FRED series WFRBST01134 and WFRBSB50215.
- Norton, Michael I. and Dan Ariely. 2011. “Building a Better America—One Wealth Quintile at a Time.” *Perspectives on Psychological Science* 6(1): 9–12.

## Updating it

The Fed releases new numbers every quarter and revises old ones. To update, open `index.html` on GitHub, select the pencil icon, and near the top of the `<script>` section change:

- the four `actual:` numbers in `const G = [` (they should add up to 100),
- `const AS_OF = "mid-2026";`,
- the figures in “The fuller picture” and “About the data,” which are plain text.

The “5 cents each” in the summary sentence is also plain text; check it if the bottom 50% share changes much (it’s the share divided by 50).

## Turning on the site (one time)

Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and select **Save**. Keep Issues turned on so the “Suggest a correction” link works.

## Author

Created by Gwen Sharp ([@gsharpokie](https://x.com/gsharpokie)).

## License

© 2026 Gwen Sharp. Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): you may share and adapt it for noncommercial purposes with credit. See [LICENSE](LICENSE). The figures belong to their sources; this license covers the page’s design, text, and code.
