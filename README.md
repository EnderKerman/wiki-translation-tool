# Wiki Translation Tool

This is a proposal of a text editor designed for wiki translators. Intended features are:

- Automatically get wikitext from wiki servers and upload translated text back to it.
- Highlight wiki syntaxes
- Auto completion or repalcement and quick access for templates and internal links and grammar
- Glossary
- Preview pages (might need internet)
- Link to habitica
- Progress overview
- Show wiki activities and track changes in source pages
- Recommend unfinished/stub/most wanted/important pages to work on.
- Help with mass editing (how?)
- And more...

As far as I know, there has not been any text editor that specifies in wiki translation. I hope it will simplify wiki translation by relieving translators from endless grammar details and CN/EN switching and so on.

Below is unfinished blueprint of the code (might be reallly bad):
- servercommunication.py: communicate with the server; we are using pwb, but we may switch to other libs in the future for pwb (seems to) relies on command line. It also makes files that contain raw wiki text.
- textprocessing.py: parses wikitext in both .wiki files and text area of UI, stores some global results(e.g. outline of each page) and suggests completion.
- UI part: I have no idea how UIs are made, only of desired appearance. It should consist of 2 windows, one for origin text and another for translation, with other small parts to show competion etc. Multiple themes should be provided, including classical, dark, and Habitica-styled, which will contain SFX from Habitica itself. (Yes I spend more time imagining UI hhh)
- data part: see trello card: https://trello.com/b/HJFWDtHy/wiki-translation-tool
  * For invitation please click [here](https://trello.com/invite/b/HJFWDtHy/a29767b55917ff16dcd4a02206adf82c/wiki-translation-tool)
