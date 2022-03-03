# IR2022_A1_42

### Information Retrieval Assignment 1

Group members: Avishi Gupta (2019155) and Manvi Goel (2019472)
Contact info: avishi19155@iiitd.ac.in, manvi19472@iiitd.ac.in

----

### Question 1
**Input**
- Enter number of queries.
- Enter two line input for each query.
- Enter words in first line and operators in second. Enter operators seperated by ", " and in uppercase. 

**Output**
- The number of documents retrieved.
- The minimum number of total comparisons done (if any).
- The list of document names retrieved.

**Libraries Used**
- The library os for handling the directory
- The libraries nltk and string for preprocessing.

**Assumptions**
- The drive is loaded, and an appropriate path is provided to the folder.
- The type and number of operators should be valid. Number of operators should be one less than total number of words. Available operators are: AND, OR, AND NOT, OR NOT.
- Words are input in space separated format.
- Operators are input in uppercase and separated by ", ". Example: AND, OR.
- Number of valid tokens should be greater than two. Valid tokens are those words which are present in the given dataset after preprocessing.
- Minimum number of comparisons in NOT operator is length of the list. 

**Preprocessing Steps**
- Converting the text to lowercase
- Performing word tokenization
- Removing stopwords
- Removing punctuation marks
- Removing the words with non-alphabet characters
- Stripping the word of extra spaces.
- Remove blank spaces.

**Methodology**
- Process the raw data from each file and generate tokens
- Use a dictionary to store the frequency, document IDs in which the token is present.
- Process the input query.
- Check if all the words from the input query are available in the dictionary. Check if the given inputs and operators are valid.
- Apply operators on list of documents for subsequent "tokens" and add the total number of comparisons for all operations.
- Return the documents and number of comparisons which satisfy the above condition.

---- 
