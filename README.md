#  NLP Tokenization, Stemming, and Lemmatization (NLTK vs spaCy)

This project demonstrates and compares key text preprocessing techniques using two major NLP libraries in Python: **NLTK** and **spaCy**.

---

##  Features

- Tokenization using NLTK and spaCy
- Stemming with Porter, Lancaster, and Snowball stemmers (NLTK)
- Lemmatization using NLTK (WordNetLemmatizer) and spaCy
- Reads input text from `sample.txt`
- Outputs comparison of results to console


---


##  Usage

1. Add or edit content in the `sample.txt` file.
2. Run the script:

```bash
python tokenization_lemmatization.py
```

3. Output will be printed in the terminal, including:
   - Tokens (NLTK and spaCy)
   - Stems (Porter, Lancaster, Snowball)
   - Lemmas (NLTK and spaCy)

---

##  Sample Text Suggestions

Use the following examples in `sample.txt` to better demonstrate the differences between tokenization, stemming, and lemmatization:

```text
The striped bats are hanging on their feet for best.
He studies all the time, but he studied little yesterday.
They're looking for better solutions than what we had.
Running faster won't always get you the best results.
My friends' bikes were stolen, and the police are investigating.
Better tools can be found in newer technologies.
I was hoping that better results had been achieved.
The children are playing with robotic dogs in the park.
He gave better advice than the older advisor.
Cats chasing mice is a common cartoon scenario.
```

### Why These Sentences?

| Example | Purpose |
|--------|---------|
| `studies` vs `studied` | Highlights lemmatization vs stemming behavior |
| `they're`, `won't` | Tests tokenizer handling of contractions |
| `better`, `best` | Tests comparative/superlative adjectives |
| `running` | Can act as noun or verb – shows context sensitivity |
| `children`, `mice` | Irregular plural forms |
| `advice` vs `advisor` | Meaningful noun/verb root differences |

---

##  Comparison Table

| Feature          | NLTK                            | spaCy                          |
|------------------|----------------------------------|--------------------------------|
| **Tokenization** | Rule-based                      | Statistical + rule-based       |
| **Stemming**     | Porter, Lancaster, Snowball     |  Not supported                |
| **Lemmatization**| WordNet-based (POS-aware)       | Context & POS-aware            |
| **Speed**        | Fast                            | Very Fast (optimized)          |
| **Ease of Use**  | More manual setup               | Built-in pipeline              |

