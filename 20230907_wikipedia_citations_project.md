# 2023-04-06 University of Washington Libraries Python Interest Group meeting
## Very brief PIG stuff
- Find [information about the UWL PIG online](https://github.com/uwl-python-ig/meetings#about-the-university-of-washington-libraries-python-interest-group) 
- We meet on the first Thursday of each month from 11 AM-12 PM
- No meeting in October, we'll meet again in November

## Presentation - Project to Improve and Normalize Wikipedia Citations

### Cat Ball intro
- Cat has a bachelor's of science in computer science and is currently pursuing a master's degree in computational linguistics here at UW
- They currently work as a site reliability engineer, and are planning to start applying for PhD programs next year

### Presentation notes
***See [slides](https://github.com/uwl-python-ig/meetings/blob/main/presentation_materials/20230907_Wiki_Citation_Improvement.pdf)***

#### Background
- A lot of Natural Language Processing (NLP) ends up ingesting Wikipedia, but citation information is often either stripped out or under-represented when this ingestion takes place
- Project goals:
    - Make it easier to understand where the information in articles being used to create/train language models is coming from
    - Make it easier for users to go from Wikipedia citation to source
    - Do no harm (to citations)--leave them in *at least* better shape than we found them! This is why the project wil use a human review process--generate edits and then have humans review these. See for example workflows for transcription where auto-transcriptions are reviewed and cleaned up by humans
- Make sure several people agree with the new citation (wow! So, looking for volunteers?)

#### More on the service
- Backend is "a little bit like middleware" - "updating the database as it goes"
- Once we have a "quorum" we can send the revision to Wikpedia (see notes on human review above)
- On parsing data: Processing data on a local drive is faster than calling API for each article!

#### Citations in Wikpedia
- Citations we like: Wikipedia citations that use a template for citing formats such as books, journal articles, websites, etc.
    - See Wikipedia:Citation templates > [examples](https://en.wikipedia.org/wiki/Wikipedia:Citation_templates#Examples) such as [Template:Cite journal](https://en.wikipedia.org/wiki/Template:Cite_journal)

```
<ref name="bn23hle0">
{{cite book 
| ... 
| ... }}
```

- Note that *{{templates}} can also be nested?!* &#x192f;, so a robust parser would be good to have
- Many Wikipedia citations don't use templates at all, they just enclose the citation material in the body of text with `<ref>` tags
- There are also deprecated citation styles!!
- **How will the citaton actually affect NLP? Or is it 'NLP-adjacent'??

#### Options for parsing templated citations
- The MediaWiki parser is *colossal*, 100,000s of lines of [PHP](https://www.php.net/); bespoke for Wikimedia Foundation needs... see:
    - [Parser.php File Reference](https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php.html)
    - [Parser Class Reference](https://doc.wikimedia.org/mediawiki-core/master/php/classParser.html)
    - [Preprocessor Class Reference](https://doc.wikimedia.org/mediawiki-core/master/php/classPreprocessor.html)
- 3rd-party citation parsers are also available, see for example [this blog post](https://www.crossref.org/blog/whats-your-citations-style/) about the Crossref [Citation Style Classifier](https://gitlab.com/crossref/citation_style_classifier)
- Parsing strategies:
    - A [recursive descent parser](https://en.wikipedia.org/wiki/Recursive_descent_parser)
    - For near term, Python's [html.parser.HTMLParser module](https://docs.python.org/3/library/html.parser.html)

#### Parsing *untemplated* citations
- Maybe we can just get the components that are easily-recognizable?? (DOIs, ISBNs, etc.)
- Something Cat may do: Train their own model! Hand-annotate untemplated citations

#### A libraries tie-in!
- The project uses WorldCat is used to find the article and **generate an 'authoritative' citation from 'authoritative' bibliographic data**

#### Q&A
- Do you get *citations* as such from WorldCat, or do you get full bibliographic records and create citations from this??
    - We get a record, and then generate a citation from that
- **How will the citation actually affect NLP? Or is it 'NLP-adjacent'??
    - Kind of an indirect relation
    - For training a large language model to make fluent-sounding language, it doesn't matter
    - For training an info-retrieval system, it could be important!
    - Indirect: Improving citations can help put human eyes on places where there are misapplied citations
- Ready for having beta testers?
    - A little bit away from this, I could share code, but for having actual UI testers, a little while
