# random-bible-verse-picker

This is a simple Python script that helps you pick a random verse from any book and chapter of the Bible (KJV). It uses a predefined structure of the Bible (number of chapters and verses per book) and the `requests` library for potential API integration (not included yet).

## Features

- Randomly selects a Bible verse from any book and chapter.
- Easy to extend for retrieving actual verse text via APIs.
- Useful for Bible study tools or daily verse generators.

Install the required packages with:

```bash
pip install -r requirements.txt
```
## Usage

```python
import random
import requests
import time

# your code here, e.g.:
book = random.choice(list(bible_structure.keys()))
chapter = random.randint(1, len(bible_structure[book]))
verse = random.randint(1, bible_structure[book][chapter - 1])
print(f"Random verse: {book} {chapter}:{verse}")
```
> You can integrate an API like bible-api.com or esv.org to fetch the verse text.



