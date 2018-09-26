# 3. Text Mininig
## Task
* Find any suitable textual data for processing which will contain at least 500 sentences.
** you can manually collect texts from BBC/CNN/New York Times, or
** use the crawler from the first homework/tutorial and extend it to crawl particular website and collect content for this task, or
** use any other suitable texts
* Perform following NLP tasks
** POS tagging
** NER with entity classification (using nltk.ne_chunk)
** NER with custom patterns
*** e.g. every match of: adjective (optional) and proper noun (singular/plural) is matched as the entity
*** see slides 31 or 38 from lecture 4 for some NLTK examples using RegexpParser or custom NER
* Implement your custom entity classification
** For each detected entity (using both nltk.ne_chunk and custom patterns)
*** Try to find a page in the Wikipedia
*** Extract the first sentence from the summary
*** Detect category from the sentence as a noun phrase
**** Example:
**** for „Wikipedia“ entity the first sentence is „Wikipedia (/?w?k??pi?di?/ or /?w?ki?pi?di?/ WIK-i-PEE-dee-?) is a free online encyclopedia that aims to allow anyone to edit articles.“
**** you can detect pattern “… is/VBZ a/DT free/JJ online/NN encyclopedia/NN …“
**** the output can be „Wikipedia“: „free online encyklopedia“
*** For unknown entities assign default category e.g. „Thing“