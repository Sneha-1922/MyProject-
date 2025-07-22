### Step 1: Start
Begin the program.

### Step 2: Input the Text
Accept a text input from:

A file (.txt, .csv, etc.)

User input (optional)

### Step 3: Preprocessing the Text
Convert the entire text to lowercase.

Remove punctuation, special characters, and extra spaces.

(Optional: Use regex or string.punctuation)

### Step 4: Split the Text into Words
Use split() to break the text into a list of individual words based on spaces.

python
Copy
Edit
words = text.split()
### Step 5: Count Word Frequencies
Initialize an empty dictionary: word_freq = {}

For each word in the list:

If word exists in the dictionary, increment its count.

Else, add the word to the dictionary with count 1.

python
Copy
Edit
for word in words:
    word_freq[word] = word_freq.get(word, 0) + 1
### Step 6: Sort the Frequencies (Optional)
Sort the dictionary by frequency in descending order.

python
Copy
Edit
sorted_words = sorted(word_freq.items(), key=lambda item: item[1], reverse=True)
### Step 7: Output the Results
Display the word-frequency pairs:

On the console, or

Write to a .csv or .json file

### Step 8: End
End the program.
