# stash-lf-pyscraper
Python-based Loyalfans scraper for Stash

## Dependencies
This is a Python scraper, and as such, Python (Python3) needs to be installed.
- The official Stash docker container already contains python and all needed modules.
- For Windows systems, install python from [python.org](https://www.python.org/downloads/windows/) ([instructions](https://phoenixnap.com/kb/how-to-install-python-3-windows)), NOT from the Windows store.
- For Linux systems please consult the relevant distro instructions.
- For Μac systems either use homebrew eg `brew install python3` or use the python.org installer ([instructions](https://www.lifewire.com/how-to-install-python-on-mac-4781318))

## pip requirements
- bs4
- lxml
- requests

## Features
- Uses the Loyalfans API to pull data relating to a given URL. This was an absolute sod to work out - lots of pre-flight cookie setting involved in this one.
- No dependency on a Chrome CDP.

## Pitfalls
- No search functionality - only manual URL entry is supported at this time.
- Tested with a few dozen clips and haven't encountered any major bugs, but caveat emptor.

## Special thanks
I'd like to thank the writers of the following scrapers on the CommunityScrapers git repository - their code has proven very useful in helping this come together:
- bnkai, who wrote the ManyVids Python scraper: https://github.com/stashapp/CommunityScrapers/commits/master/scrapers/ManyVids
- estellaarrieta, who wrote the WowNetworkVenus Python scraper, from which I managed to work out a lot about the structure of Python scrapers, etc.

Also, mention has to go to ChatGPT, without which I wouldn't have been able to fumble blindly through this project.
