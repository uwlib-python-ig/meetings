# 2024-04-04 University of Washington Libraries Python Interest Group meeting

## Greeting / review Python IG community Agreement 🤝
> - **Our [community agreement](https://github.com/uwlib-python-ig/meetings/tree/main#community-agreement) is adapted from that of the UW Libraries Digital Scholarship Collective**  
> - *More UWL Python Interest Group information is available at https://github.com/uwlib-python-ig/meetings#get-in-touch-with-the-pig.* 

## Announcement 📢 - call for Python IG facilitator
> - ***See [mailing list announcement](https://mailman11.u.washington.edu/pipermail/uwlib_pig/2024/000024.html) for details***
> - Introductions if time and number of participants permits, else please say hello in chat!

## Text Manipulation in Python
***Welcome John Borwick!***  
***See [presentation slides](https://github.com/uwlib-python-ig/meetings/blob/main/presentation_materials/20240404_text_manipulation.pdf)***  

### Presentation/discussion
- Many (all?) slide examples use the Python IDLE - [more information here](https://realpython.com/python-idle/)
- We are talking about Python 3--and it's a big difference!
- "Python 3 strings are Unicode-aware (...) it's not a set of bytes, it has an encoding"
- Strings are arrays, so we looked at some indexing! "You can use \[the string\] like an array"
- [`dir()` method](https://www.programiz.com/python-programming/methods/built-in/dir)!! "Enumerate all of the properties for a given object"
	- So if `s1` is a string, `dir(s1)`
	- See also [`help(object.method)`](https://www.programiz.com/python-programming/methods/built-in/help)
	- "Get help at the point of need"!
- Regular expressions!
	- Slides include a link to a tool which converts a regex to an image!?!?
- Python [re library](https://docs.python.org/3/library/re.html)
	- NOTE that `search` and `match` function differently!
	- As above, see slides for lots of regex resources
	- Plug for `re.VERBOSE` - ignores excess whitespace, allows you to comment your regexes! (See S35)
