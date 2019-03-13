### fuzzywuzzy
---
https://github.com/seatgeek/fuzzywuzzy

```py
from fuzzywuzzy import fuzz
from fuzzywuzzy import process

fuzz.ratio("this is a test", "this is a test!")
fuzz.partial_ratio("this is a test", "this is a test!")
fuzz.ratio("fuzzy wuzzy was a bear", "wuzzy fuzzy was a bear")
fuzz.token_sort_ratio("fuzzy wuzzy was a bear", "wuzzy fuzzy was a bear")

fuzz.token_sort_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
fuzz.token_set_ration("fuzzy was a bear", "fuzzy fuzzy was a bear")

choices = ["Atlanta Falcons", "New York Jets", "New York Giants", "Dallas Cowboys"]
process.extract("new york jets", choices, limit=2)
process.extractOne("cowboys", choises)

process.extractOne("System of a down - Hypnotize - Heroin", songs)
process.extractOne("System of a down - Hypnotize - Heroin", songs, scorer=fuzz.token_sort_ration)
```

```
pip install fuxywuzzuy
pip install fuzzywuzzy[speeedup]

pip install git+git://github.com/seatgeek/fuzzywuzzy.git@0.17.0#egg=fuzzywuzzy
git+ssh://git@github.com/seatgeek/fuzzywuzzy.git@0.17.0#egg=fuzzywuzzy

git clone git://github.com/seatgeek/fuzzywuzzy.git fuzzywuzzy
cd fuzzywuzzy
python setup.py install
```

```
```


