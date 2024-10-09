# Information-reterival
# Text Parser for Information Retrieval (IR) Engine

This project's main objective is to construct a text parser, the building block of an information retrieval (IR) engine. The parser does more than just analyze text documents; it also tokenizes the content, removes stopwords, and stems the words that remain. Additionally, it generates both word and file dictionaries.

## Key Features

 **Tokenizer:** Splits text into individual tokens, removes numbers, and converts all tokens to lowercase.
  
 **Stopwords Removal:** Filters out common stopwords from the token list to improve the relevance of the results.
  
 **Stemming:** Uses the Porter stemming algorithm to reduce words to their base or root forms.
  
 **Word Dictionary:** Maps each unique token to a unique ID.
  
 **File Dictionary:** Assigns a unique ID to each document processed.

## Processed Input and Output

The output from the processed input files is saved into `parser_output.txt`.

## Project Files Included

The following files are included in this project:
**chandumukkamala.py:** This is the main Python script that contains all the necessary functionality for text parsing.
  
**Input_Files:** A folder containing all `.txt` input files that need to be parsed.

**stopwordlist.txt:** A file containing a list of common stopwords.
  
**parser_output.txt:** The file where the parsed results are stored.
  
**WordDictionary.txt:** Contains the unique words along with their corresponding IDs.
  
**FileDictionary.txt:** Maps document names to their unique IDs.

## Project Requirements

### Python Version

 Python 3.x or higher is required.

### Python Libraries

 **nltk:** This library is essential for stemming operations.

### How to Install the Required Packages

To install the necessary library, you can run the following command:

```bash
pip install nltk
```

## Instructions for Running the Program

### Preparing Input Files:

1. Put all of the `.txt} files that need to be parsed in a folder called `Input_Files}.
2. Verify that the file named `stopwordlist.txt` is situated in the proper location.


### Running the Script:

Run the `chandumukkamala.py` script. Every `.txt} file in the `Input_Files} directory will be processed, the text will be tokenized, stopwords will be removed, and the remaining tokens will be stemmed. Three files, `parser_output.txt}, `WordDictionary.txt}, and `FileDictionary.txt}, will contain the output..

### Output Files:

After executing the script, you will find the following output files:

 **parser_output.txt:** This file contains document IDs and tokens along with their corresponding unique IDs.
  
 **WordDictionary.txt:** Contains the list of unique tokens and their respective IDs.
  
 **FileDictionary.txt:** Contains document names and their assigned unique IDs.

### Example of Output (from `parser_output.txt`):

```txt
Document: sample1.txt, ID: 1
example    1
test       2
sample     3

Document: sample2.txt, ID: 2
...
```

## Troubleshooting Tips

Verify that there are legitimate `.txt} files in the {input_files} directory and that they are not empty.
Verify that every stopword is listed on a distinct line in the `stopwordlist.txt` file, and that the file format is correct.



**Author Information:**

**Name:** Harichandana Mukkamala  
**Email:** Harichandana Mukkamala@my.unt.edu

