# 2024-03-07 University of Washington Libraries Python Interest Group meeting

## Greeting / review Python IG community Agreement
> **Our [community agreement](https://github.com/uwlib-python-ig/meetings/tree/main#community-agreement) is adapted from that of the UW Libraries Digital Scholarship Collective**  
> *More UWL Python Interest Group information is available at https://github.com/uwlib-python-ig/meetings#get-in-touch-with-the-pig.* 

## Guest speaker Anna Preus
SEE  
- [Recording](https://washington.zoom.us/rec/share/Tyi39CWW6yY8WaJrwRrpJbdQTRaEqHYe5lYj5zNNyTStONe80jdnEqxYeyRhokeY.m2V5Ugy3Ti0TxFsT): Presentation and discussion with transcript (*available until July 7, 2024*)
- [Presentation slides](https://github.com/uwl-python-ig/meetings/blob/main/presentation_materials/20240307_publishing-empire_uwl-python.pdf)
- As of date of presentation, project code is available at https://github.com/apreus/english-catalogue-of-books 

### Discussion notes
- So many overlaps with library land! Poster "don't attempt to recreate information and library science"
- The examples were so helpful! As someone struggling to get code to do what you want
- I wanted to mention two resources helpful for me:
	- [Regex Crossword](https://regexcrossword.com/) is helpful for learning regexes
	- Dealing with unicode characters/diacritics - see blog post [Compare strings the right way](https://www.b-list.org/weblog/2023/dec/23/compare-python-strings/)
	- Thank you! Looking into unicode errors became a whole summer of work!! For example, mix-up between a unicode character that looks like the letter 'y'
- More about gathering and processing data:
	- I didn't have API access during initial data gathering -- there was a lot of clicking to download MARC
	- For processing texts on HathiTrust, HT performed OCR
	- Used [NLTK](https://www.nltk.org/) for processing, also used some of [spaCy](https://spacy.io/)
	- Once the data was more structured, everything went into [Pandas](https://pandas.pydata.org/) 
	- See also [chapter on Pandas](https://melaniewalsh.github.io/Intro-Cultural-Analytics/03-Data-Analysis/00-Data-Analysis.html) in Melanie Walsh's book Introduction to Cultural Analytics & Python
- "We've all been tortured by the concept of comprehensiveness", there's got to be more than is in the guild catalog or even in a vast database--is it achievable to be complete?
	- It's tough -- using data can provide the illusion of being comprehensive...
	- For example - WorldCat records for Tagore pale in comparison to what's available in the [Bichitra: Online Tagore Variorum :: School of Cultural Texts and Records](http://bichitra.jdvu.ac.in/index.php)
	- Interesting example - Virginia Woolf is not in the guild catalog, because she hadn't gone through the required apprenticeship
	- "Free the dataset and let people critique it" instead of holding it until it is "ready for release"?
- Is it true that the cleanup of OCRed text was written largely from scratch?
	- Yes, it pretty much had to be custom
	- I'm hearing that "you need to re-OCR this; this is a computer-vision problem, not a text-processing problem" - OK, yes, it's so true... but the scope of this project can't really expand to improving OCR...
- What about [RLIN](https://cdlib.org/cdlinfo/1998/11/18/rlin-database-available-for-testing-through-the-web-interface/) and/or other, older databases, which might be of use?
- See also [Summarizing America: The Impact of Metadata on Historical Discovery](https://www.neh.gov/blog/summarizing-america-impact-metadata-historical-discovery), written by a UW CHID alumni