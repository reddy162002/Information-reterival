# Text Parser for Information Retrieval (IR) Engine

## Overview

This project is a text parser designed as a foundational tool for an Information Retrieval (IR) engine. The parser tokenizes text, removes stopwords, and applies stemming to reduce words to their root forms. It also generates unique word and file dictionaries, associating each word and document with a unique ID. The parsed data is saved in the `parser_output.txt` file, with additional output files for word and file IDs.

## Features

1. **Tokenizer**: 
   - Tokenizes text by splitting it into lowercase words.
   - Filters out numbers and special characters.
   
2. **Stopword Removal**: 
   - Removes common stopwords using a predefined stopword list.
   
3. **Stemming**: 
   - Applies the Porter stemming algorithm to reduce words to their base or root form.

4. **Word Dictionary**: 
   - Each unique word is assigned a unique ID and saved in `WordDictionary.txt`.
   
5. **File Dictionary**: 
   - Each document is assigned a unique ID and saved in `FileDictionary.txt`.

## Project Files

- **Python_Code**: Main Python script that contains all the parsing functionality.
- **input_files**: Folder where the input text files to be parsed are stored.
- **stopwordlist.txt**: A file containing stopwords to be filtered out during parsing.
- **parser_output.txt**: File containing parsed output with word and document IDs.
- **WordDictionary.txt**: Dictionary mapping each unique word to a unique ID.
- **FileDictionary.txt**: Dictionary mapping each file name to a unique ID.

## Requirements

### Python Version:
- Python 3.x or higher is required.

### Python Libraries:
- `nltk`: Required for stemming. Install it by running:

```bash
pip install nltk
```

## How to Use

### Input Files:
1. Put all of the `.txt} files in the `input_files} folder that require parsing.
2. Verify that the stopwords to be filtered out are contained in the `stopwordlist.txt` file, one stopword per line.


### Running the Script:
1. Run the `Python_Code.py` script. 
   ```bash
   python Python_Code.py
   ```
2. The script will process each `.txt` file in the `input_files` folder, tokenize the content, remove stopwords, stem the words, and save the output to:
   - `parser_output.txt`: Contains the parsed document text with word and document IDs.
   - `WordDictionary.txt`: Lists unique words and their respective IDs.
   - `FileDictionary.txt`: Lists document names and their respective IDs.

### Example Output (from `parser_output.txt`):
```txt
Document: sample1.txt, ID: 1
example    1
test       2
sample     3

Document: sample2.txt, ID: 2
...
```

## Troubleshooting

1. **Input directory not found**:
   - Ensure that the `input_files` directory exists and contains valid `.txt` files.

2. **Stopwords file not found**:
   - Verify that the `stopwordlist.txt` file is located in the correct directory.



## Author Information

**Name**: Namitha Padigapati  
**Email**: NamithaPadigapati@my.unt.edu
