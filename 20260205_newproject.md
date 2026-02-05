# 2026-02-05 University of Washington Libraries Python Interest Group meeting
## Greeting / review Python IG community Agreement 🤝
> - **Our [community agreement](https://github.com/uwlib-python-ig/meetings/tree/main#community-agreement) is adapted from that of the UW Libraries Digital Scholarship Collective**  
> - *[More UWL Python Interest Group information](https://github.com/uwlib-python-ig/meetings#get-in-touch-with-the-pig)* 

## Announcements
> - Introductions if time and number of participants permits, else please say hello in chat!
> - Started a [list of potential speakers](https://hackmd.io/-s08LbKmRq2kbKzXJmSZLw?both) that can be edited by anyone. Please add to the list! 

## Discussion
- Summer project idea: comparing spreadsheets of potential gifts/donations with ISBNs to Alma to see if we already have the materials in our collections
- How do you get the information from Alma? Wouldn’t be surprised if there are a couple of endpoints: does this exist? Do we have it? (because of summit, etc.)
- There’s an API for Alma stuff. But the question is is there a public API or something that doesn’t require a lot of setup? Ahead of time or in between sessions, we could check with Wade on the API. 
- Some places actually goes to the catalog as if it were a human – but don’t think we should do this.
- Way I would build it is building program or script that checks ONE ISBN then if it works you know it works. Maybe pause every second. Cache it so that if it errors out you don’t have to restart from the beginning.
- People could be interested in summit but probably most interested in if we have the book.
- In the past when a tool has been hard to get data out of, have been trying to get report of ALL ISBNs and compare to that report rather than querying it.
- How can we print out information to the screen? How can we create a csv? If we want to create a straight excel file, how do we layer that on?
- Start with session where you can run Python, get things set up, everything works. Github repos, VSCode, etc. Copy and paste commands, etc. Read the spreadsheet. Thinking through the phases. Timing to do this should be trying to weigh having breathing space between sessions and not forgetting everything.
- When thinking about a programming challenge, thinking about edge cases? 10 digit vs 13 digit? What about hyphens? ISSNs? If you don’t have an ISBN at all, would you want it to look up what the ISBN would be?
- If we don’t need production data, could get access to the staging environment. From my perspective, if yall are up for identifying what you want to do, can schedule me and say if you want me in the meeting or just on chat.
- Claude Code discussion:
-   Force multiplier. If you’re going in a good direction, 20x faster in that direction. If bad direction, go in that bad direction 20x faster.
-   Claude can just do it. Is that the purpose of the activity?
-   Because of JB’s experience, can see its logic and stop it. Or stop bad design decisions.
-   High signal low noise. Haven’t thought about what this means for society. Software companies’ stock valuations going down (seen on Instagram). Thinking about digital asset management tools. One of the tools isn't working out, thinking could build it using Claude Code.
-   Though still need to consider deployment and maintenance. 
