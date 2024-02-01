# 2024-02-02 University of Washington Libraries Python Interest Group meeting

## Introductions

## Review community agreement 🤝
***Add comments to the [working document](https://docs.google.com/document/d/1Hgx4cfDhR_BDKSzUB-vDKso422DV0zg2lvtnN66PW6E/edit?usp=sharing)***

## Discuss reading: Python & APIs: A Winning Combo for Reading Public Data
> **https://realpython.com/python-api/**

### Add comments, questions, rants here!
- (BMR) The [HTTP Headers section](https://realpython.com/python-api/#http-headers) gives brief mention to dot notation, which is something that can really trip me up.

> To inspect the headers of a response, you can use `response.headers` (...) To do the same with the request headers, you can use `response.request.headers` since request is an attribute of the `Response` object

- (BMR) The `requests.get.json()` method seems like one I'll use a lot, very handy
- (BMR) Curious whether anyone uses anything *besides* requests for API calls? I've heard tell that [the HTTPX library](https://www.python-httpx.org/) is good
    - (ThomasJ) In UW-IT on my team we mainly use requests. Though we are experimenting with [AIOHTTP](https://docs.aiohttp.org/en/stable/) for one of our apps. I think it is similar to HTTPX in that it allows you to make _asynchronous_ requests. We tried HTTPX, but I think it was missing one feature we needed, which might come in the future because HTTPX is a little newer and still being actively developed.

### Discussion
- Some notes and the example code implemented in a [Jupyter notebook file available online](https://gist.github.com/briesenberg07/f0821bd4218751ce038470a2b9392423)
- I make API calls all the time! Others teams in UW IT create APIs and we make calls
- I use APIs for research purposes; we teach students to do this kind of work in communication leadership, using a tutorial similar to this
    - We teach a similar process; this is the syllabus for the course -- https://wiki.communitydata.science/Community_Data_Science_Course_(Spring_2023) - we do some things differently
    - I didn't like the way the tutorial handled API keys - it's bad security practice to type an API key in a flatfile! People need to get it into their heads that a key is a password
    - Don't put a key in the Python code, put it separate! So many vulnerabilities! People are scanning GitHub all the time looking for this mistake - never put an API key directly into Python code 
    - I agree with the security concerns here! 
- "Aren't some companies, like X, now making it impossible or expensive to use their APIs for research purposes?"
    - Yes, companies are trying to figure out how to create income from user data
    - The X changes have been really bad; there was a blossoming of research work for user data in then-Twitter! But the changes have shut a lot of that down
    - Similar things are happening for reddit, impacting lots of use cases besides research
- I actually use other things for API calls - 
    - Postman in my browser, JavaScript 
- API availability sort of levels the playing field for research; even if someone doesn't have access to large sets of curated data from an institution, APIs can provide access to datasets 
- Was the tutorial helpful?
    - I liked the context; I appreciated the 'digestible chunks', and the examples
    - *"Python + APIs is important knowledge to have"* - I seem to be getting this message
- Reading documentation is challenging!
    - We send students to use StackExchange; note that 'real developers' use this too!
    - Another strategy - ask ChatGPT to help you; note that it sometimes works to ask ChatGPT to provide another code example if the first one isn't readable for you
- Not python, but something I had some students try - https://academy.postman.com/
    - APIs are language independent; the above link is a way to play with APIs without using a scripting environment
- On authentication, see also https://softwareengineering.stackexchange.com/questions/419533/api-key-vs-jwt-which-authentication-to-use-and-when
- There's a certain kind of computational literacy, it's not just the magic of wizards, many of us use this magic
    - Think about the times when you've used an online tool and you can see the API call with params (`?`, `=`, `&`) building out in the URL
- More fun resources: https://dog.ceo/dog-api/
    - You're seeing the construction of the URL and you are using dog pictures!





