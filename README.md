# Multi-Language Wordsearch Generator

A static website that generates wordsearch puzzles with vocabulary in multiple languages. Choose which language appears in the grid and which language appears in the word list, then find the word list language words hidden in the grid.

## Features

- Pre-loaded vocabulary words from `words.json` with Spanish, French, and English translations
- Supports multiple language pairs: Spanish-French, Spanish-English, French-English
- Bidirectional selection: Choose which language to find (source) and which to display (target)
- Generates a 15x15 wordsearch grid with words placed in random directions
- Translation words displayed in the list for lookup
- Interactive selection: click and drag to find words
- Visual feedback for found words (highlighted in yellow, struck through in list)

## How to Use

1. Open `index.html` in a web browser
2. Select the language for the grid (where words will be hidden)
3. Select the language for the word list (the translations to find)
4. Click and drag on the grid to select sequences of letters
5. Find all the word list language words - reference translations are in the list
6. Found words are highlighted and marked complete

## Adding More Words

Edit `words.json` to add more word pairs. Each entry should have all three languages:

```json
[
  {
    "spanish": "PAN",
    "french": "PAIN",
    "english": "BREAD"
  }
]
```

## Hosting on GitHub Pages

1. Create a new repository on GitHub
2. Upload these files: `index.html`, `styles.css`, `script.js`, `words.json`
3. Go to repository Settings > Pages
4. Set source to "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Save and wait for deployment

Your wordsearch will be available at `https://yourusername.github.io/repositoryname/`

## Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript