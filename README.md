# Randomised-Wikipedia-Scraper
This takes a randomised Wikipedia page, and traverses a randomised link chain, scraping the main body text, as well as the titles of the page, and saving both to respective .txt files, that can be easily retrieved.

Randomised-Wikipedia-Scraper.txt contains the Python 3 code that makes use of the forbidden_ends.txt file, something that contains (mostly) disallowed url endings by the Wikipedia robots.txt file, as well as some awkward page types at the end. This should generate two files, one called keyfile.txt, which contains the listing of all of the scraped topics, and writefile.txt, which contains all of the scraped data. Copy-pasting into a workspace should suffice, but if not, create those .txt files in the chosen directory.

This is quite a rudimentary method of scraping, however for small-scale html parsing, BeautifulSoup works well.

A known issue is that sometimes the link will belong to the disallowed subset, and the code will not pick up on this. In order to divert from this, an error message shows when this happens, and the program redirects back to the Wikipedia contents page automatically. 
