# Multi-Language Wordsearch Generator

A static website that generates wordsearch puzzles with vocabulary in multiple languages and themes. Choose a theme, which language appears in the grid, and which language appears in the word list, then find the word list language words hidden in the grid.

## Features

- Multiple themes: Food vocabulary and Family member names
- Pre-loaded vocabulary words from `food.json` and `family.json` with Spanish, French, and English translations
- Supports all combinations of grid and word list languages
- Generates a 15x15 wordsearch grid with words placed in random directions
- Translation words displayed in the list for lookup
- Interactive selection: click and drag to find words
- Visual feedback for found words (highlighted in yellow, struck through in list)

## How to Use

1. Open `index.html` in a web browser
2. Select a theme: Food or Family Members
3. Select the language for the grid (where words will be hidden)
4. Select the language for the word list (the translations to find)
5. Click the "Load Wordsearch" button to generate the puzzle
6. Click and drag on the grid to select sequences of letters
7. Find all the word list language words - reference translations are in the list
8. Found words are highlighted and marked complete
9. Click "New Wordsearch" to change settings and generate a new puzzle

## Adding More Words

Edit the appropriate JSON file to add more word pairs. Each entry should have all three languages:

### Food words (`food.json`):
```json
[
  {
    "spanish": "PAN",
    "french": "PAIN",
    "english": "BREAD"
  }
]
```

### Family member words (`family.json`):
```json
[
  {
    "spanish": "PADRE",
    "french": "PERE",
    "english": "FATHER"
  }
]
```

## Hosting on GitHub Pages

1. Create a new repository on GitHub
2. Upload these files: `index.html`, `styles.css`, `script.js`, `food.json`, `family.json`
3. Go to repository Settings > Pages
4. Set source to "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Save and wait for deployment

Your wordsearch will be available at `https://yourusername.github.io/repositoryname/`

## Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript