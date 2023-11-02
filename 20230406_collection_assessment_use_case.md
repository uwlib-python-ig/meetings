# 2023-04-06 University of Washington Libraries Python Interest Group meeting
## Announcements
### Python{4}Lib, a Code4Lib Python Interest group
   - The group has assembled Python resources! See code4lib/[python4lib-resources](https://github.com/code4lib/python4lib-resources)
   - The mini_python_intro which was presented on 04-04 may be of interest
      - the notebook file is [available via Google Colab](https://colab.research.google.com/drive/1m3cz4KeozooHFzjswyjgJmbfXZTfG0mP?usp=sharing) or [in uwlib-python-ig/shared-01](https://github.com/uwlib-python-ig/shared-01/mini_python_intro.ipynb) (ask [Benjamin](mailto:ries07@uw.edu) if you'd like help running notebook files)

## Show-and-tell: Python for collection assessment
***Welcome Hana Levay! Note that links require a UW NetID for access. All materials related to Hana's presentation are available [here](https://drive.google.com/drive/folders/1xeA69GdZNzj926kyK5GXWeHwC-yussHe?usp=share_link).***
### Notes
- I've used a couple of strategies (below) to get information about which Orbis-Cascase Alliance libraries hold items.
- More recently, I've been using OCLC's [GreenGlass](https://www.oclc.org/en/greenglass.html) to do this work.

### Stragegy 1
- See [few.py](https://drive.google.com/file/d/10f_PvpMdHHrbU5Lf_wZ_sq1t1q27ETy0/view?usp=share_link)
- This code was written sometime ago by someone who isn't Hana! At one point it stopped working and had to be fixed!
- The `get_api_data()` function may be the most important part
   - The URL passed using the requests library can take different params to adjust results, for example zip code, library time
- Example input would be a list of OCLC numbers for items (see [example-data.txt](https://drive.google.com/file/d/1Rt0z0VaHo-C2vUZHz2Vhx9LNitnOB0Fw/view?usp=share_link))
- Example output is a list of the OCLC numbers, with symbols for each which show which Orbis-cascade Alliance institutions hold them (see [example-results.txt](https://drive.google.com/file/d/1sK5h2cp1rYorxz18mmYACS-Lt_ETVnT1/view?usp=sharing))

- To fun, download deaccession-master directory, add OCLC numbers to checklist.txt (is this right??)
- Modules need to be installed to use the code, learning pip is good for this
- There are also some arguments whhen calling the script
- There are help docs (see [Running Last Copy Script.docx](https://docs.google.com/document/d/1sQ3vQO1J4GcqQN_sFP9Y5ix5UU7_WRtz/edit?usp=sharing&ouid=103235126934628753338&rtpof=true&sd=true))

### Strategy 2
- I did the same thing in OpenRefine (see [Using OpenRefine to find Alliance holdings](https://docs.google.com/document/d/1hD0-5HHe_xUwsKXjje3kMjJO-NttZNl8d5b4x6Vy1mo/edit?usp=sharing))
- Note that this doc assumes some knowledge of OpenRefine

### Q&A
- Are you finding that GreenGlass eliminates the need to use Python?
   - GreenGlass makes a list, but a person is still needed to make a decision
- Suggestion for UWL-PIG How about another very basic session on how to use notebooks??
   - See notes from 2021-06-17 for an introduction to Jupyter notebooks
