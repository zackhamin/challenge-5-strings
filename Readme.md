# Challenge 05: Word Counter

## Overview
In this challenge, you'll create a function that analyses text and finds the most frequent words.

The function should:
- Take a text string and a number N as input
- Return an array of the N most common words and their counts
- Handle different cases and punctuation appropriately

### Examples:
```javascript
const text = "The quick brown fox jumps over the lazy dog. The dog sleeps."

getTopWords(text, 2) 
// returns [
//   { word: 'the', count: 2 },
//   { word: 'dog', count: 2 }
// ]

getTopWords(text, 3) 
// returns [
//   { word: 'the', count: 2 },
//   { word: 'dog', count: 2 },
//   { word: 'quick', count: 1 }
// ]
```

## Rules
Follow the same Git workflow practices:

1. Fork this repo to your own Git
2. Create your working branch using this naming convention:
   - `feat/` - for the main work
   - `fix/` - for things you need to improve
   - `chore/` - for things you need to clean up

Example:
```bash
git checkout -b feat/CC-challenge-5-word-counter
```

## Requirements
Your function should:
- Ignore case (treat "The" and "the" as the same word)
- Remove punctuation
- Ignore common punctuation (.,!?)
- Handle multiple spaces
- Sort words with same frequency alphabetically
- Handle empty strings or invalid input

## Edge Cases to Consider
- Empty string
- Text with only spaces/punctuation
- N larger than number of unique words
- N less than or equal to 0
- Text with numbers
- Special characters
- Multiple spaces/newlines

## Project Setup
```bash
npm init -y
npm install --save-dev jest
npm install --save-dev eslint prettier
```

Update your package.json with:
```json
{
  "scripts": {
    "test": "jest",
    "test:watch": "jest --watch",
    "lint": "eslint .",
    "format": "prettier --write ."
  }
}
```

## Tips
- Consider using:
  - Object to store word counts
  - Array methods for sorting
  - Regular expressions for cleaning text
  - String methods for splitting and cleaning

## Submission
- Complete your solution
- Merge everything into main
- Post your solution link in the challenge thread

Good luck! 📚