# 2026-04-02 University of Washington Libraries Python Interest Group meeting
## Greeting / review Python IG community Agreement 🤝
> - **Our [community agreement](https://github.com/uwlib-python-ig/meetings/tree/main#community-agreement) is adapted from that of the UW Libraries Digital Scholarship Collective**  
> - *[More UWL Python Interest Group information](https://github.com/uwlib-python-ig/meetings#get-in-touch-with-the-pig)* 

## Announcements
> - Introductions if time and number of participants permits, else please say hello in chat!
> - Started a [list of potential speakers](https://hackmd.io/-s08LbKmRq2kbKzXJmSZLw?both) that can be edited by anyone. Please add to the list! 

## Discussion
- Good idea to have structure, what we're going to do. Make a commitment. 

- Really enjoy this group, have been learning, totally outside of what I usually do or think about. In the past, discussed with John you need to know what this stuff does. Need to have a reason to use it. Have been trying to investigate. One reason as a subject librarian: time I'm looking at most spreadsheets is weeding time, collections development. That feels like one realm where Python can be important. English librarian -- Anna Preus, DH, scans of old publication records from India and England. Used Python to clean it up so that she could do something with the data. DH -- digitized something, scanned something. Need to use Python to make it useful. Another realm: classes where students are doing something with DH. Textual analysis. Sometimes feel like it's a magic trick that you do, end is that you've done the trick. Would really love to know where this textual analysis is useful. 

- HL does stuff already, maybe not more to be done? Python does stuff, but you need to have a reason. 

- Part of what I'm trying to reflect on is...think having a plan is great. What I could be useful with, what my role should be. Times I could be more of the lawyer expert, times I could be more of the counselor expert. More of the lawyer expert part in terms of the outcomes, have found it really helpful to use Bloom's taxonomy verbs and come up with learning outcomes. List Python keywords vs contract Python 2 from Python 3. 

- If this is a summer thing, trying to do it in a really compressed way. An hour meeting every day. Sometimes, people have more of a solution orientation, sometimes more of a problem orientation. You all may want to focus more on the problems like spreadsheets which is more level where I can help because things you're not aware of in the Python system. Would love to help however I can. Might be able to point out edge cases. Ex. GitHub. 

- [Bloom's Taxonomy](https://www.utica.edu/academic/Assessment/new/Blooms%20Taxonomy%20-%20Best.pdf)

- Collection development: 
- Space crisis. Totally out of space. Could be years before offsite storage facility set up. If we bring in 40K books, not space for that. If we get that many, then that many need to go. With some weeding projects, stage 1 was getting rid of duplicates. 
- Another thing was if we have ebook version, then get rid of print book. Debates about books. 
- Last couple of years, was really confusing. Things if there were multiple editions. Gets tricky bc if there are 13 editions, do you keep 1 and 13? What about those in between? 
- Spreadsheets -- in the Orbis Cascade Alliance, if there are more than 3, if there's a 4th one get rid of it. 
- Some worries that people have, all of us are getting rid of books at the same time. Need to be careful. 
- Circ stats -- if only circulated once in the past 100 years, do you get rid of it? 
- When talking to English student, sometimes they're excited to get the book no one has looked at in the past 100 years. 
- Cells and cells and cells of data. There's a lot of cleanup that needs to be done. A lot that doesn't seem relevant. I'm looking at my own thing, might help to take peek at what other people are doing. 
- We'll get a certain spreadsheet, might get different statistics in Alma. Inconsistent stats. 
- Journal cuts -- cost per use, sometimes thinking about what discipline does this fall into.
- All have rubrics, but they're all different. E.g., I don't care if something hasn't circulated in 100 years. Different in academic institution, want to have coverage so there aren't gaps in the record. 


- This makes me think that sometimes when you're trying to automate, can be useful in thinking about what as a human I'm doing. Ex. how do you find different editions? One approach to programming is to do that in an automated way. Probably not going to work 100% of the time. Ex. the ISBN doesn't show up. 
- Sometimes there will be a totally different approach. Less for example we're talking about, but IT lesson -- if it's under 100 things, do it manually. That's not true for this case because even if only 10 things can do a lot. Can help with learning because very well understood problem. 

- What is the data you're wanting to get and analyze together? What are you trying to grab? What are you looking for that's making it hard to navigate all of those spreadsheets? What's the data you're trying to get out of it? Would Python make it easier to get out and consolidate? 
 
- If we're getting all this stuff from Hana, raw stuff she gets, anything she needs cleaned up? 
- Edition thing -- was esp worried about Orbis Cascade stuff. Really look at Orbis Cascade. Really want to keep first edition and last edition, not sure what to do with editions in between. Looking at titles, as English studies librarian spent so many hours with these people. Not going to hold the book, read the book. Trying to see from the title, does this seem to be an important part of themes in the English dept. Looking for active teams that they care about. Might not be an active theme but gaps, good to get coverage. Some people really focused on circ.  

- Would it be helpful for report to generate some of that context so you have more than the title? Ex need to see notes fields, etc. Just need to see description, circ. 
- Yes, or even just subject terms. Often do look to those. 
- API call with Python to call MARC records. 

- Similar conceptually to this Toyota/Lean concept “autonomation” that’s essentially humans working in concept with [autonomation](https://en.wikipedia.org/wiki/Autonomation), e.g., script helps with context and maybe some checking, and humans are deciding

- Information management perspective: 
- What data are you receiving? Sometimes this requires a little more information. Is the author's name always last, first? Confirming how trustworthy that data is. Esp in this case, what data sources do I trust. 500 and 600 fields -- don't know how much to trust those. To what extent rely on this field. 
- Really like a program pulling together more context for a human to decide. Don't know if there's any other tools that you would trust besides Alma for this stuff. Totally different database where you could pull up number and get data from it. 
- One thing programs are good at is getting stuff from multiple sources. 

- Includes OCLC number. Maybe not included in export? If it's all from Alma. 
- Interesting to use that to look at what other people have. 
- Negeen will come up with a project plan, timing, weeklong intensives sessions. Sprint 0, getting installed, getting IDE set up VSCode, Elliott show and tell, check in with Hana. 

