# uni-entranceExam-words-database
This repository is containing Iran's university computer entrance exam English words database.

English words are from exam year 90 to 99 (2011 to 2021)

## Tables schema 

### Words
- **_id_** INTEGER
- **_word_** TEXT

Notes:
- This table contains words that we define.
- _word_ is our actual word that we are trying to define.
### Definition
- **_definitions_** TEXT
- **_example_** TEXT
- **_word_id_** INTEGER

Notes:
- This table is the definition of our words.
- A word may have more than one definition, So _word_id_ is foreign key.
- A definition may have an example.

### Synonym
- _**word_id**_ INTEGER
- _**synonym**_ TEXT

Notes:
- This table contains synonym for words, A word may have a synonym or not. 
- _word_id_ is foreign key from Words table.

### Phonetics
- **_text_** TEXT
- _**audio**_ TEXT
- **_word_id_** INTEGER

Notes:
- This table contains phonetic for words.
- _text_ is the phonetic characters.
- _audio_ is a link to play audio
- _word_id_ is foreign key from Words table.

Tables are not well defined because it was extracted from an android app using room database (https://github.com/amindadgar/VocabularyBook).

# مجموعه کلمات انگلیسی کنکور ارشد کامپیوتر
این دیتابیس شامل تمام کلمات انگلیسی موجود در کنکورارشد کامپیوتر از سال 90 الی 99 می‌باشد
