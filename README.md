# Semantic Search with Universal Sentence Encoder

This project is a simple semantic search prototype that uses the [Universal Sentence Encoder (USE)](https://tfhub.dev/google/universal-sentence-encoder/4) to search through mock data based on semantic similarity. The entire functionality is implemented in a single HTML file (`index.html`) and runs completely in the browser using [TensorFlow.js](https://www.tensorflow.org/js).

## Overview

The project demonstrates how to use the Universal Sentence Encoder to embed text data into vector representations and perform similarity-based searches using cosine similarity. The results are ranked according to their semantic closeness to the user's search query.

### Features
- Load the Universal Sentence Encoder model directly in the browser.
- Perform semantic search on a small dataset of mock phrases.
- Compute cosine similarity between the query and dataset items to rank results.
- Display ranked results in a simple UI.

## Getting Started

To run the project, simply open the `index.html` file in a web browser. There is no need for a server or any backend configuration. All processing happens in the user's browser.

### Prerequisites
- A modern web browser (e.g., Chrome, Firefox) that supports JavaScript and can handle TensorFlow.js operations.
- Internet connection to load TensorFlow.js and the Universal Sentence Encoder model from the CDN.

### Running the Project
1. Clone this repository or download the `index.html` file.
2. Open `index.html` in your browser.
3. Enter a search term in the input box and click the "Search" button.
4. The search results, ranked by similarity to the query, will be displayed below.

## How It Works

- The Universal Sentence Encoder model is loaded using TensorFlow.js.
- The mock dataset contains five items with distinct descriptions.
- When the user enters a query, the model computes vector embeddings for both the query and each item in the dataset.
- Cosine similarity is used to determine how closely each item matches the query.
- The items are then sorted by similarity and displayed to the user.

## Mock Data
The mock dataset consists of the following items:
- "A red apple on the table"
- "A fast sports car driving on the highway"
- "A cat sitting on the windowsill"
- "A book about quantum physics"
- "Delicious homemade pizza recipe"

These items have intentionally distinct topics to showcase the semantic capabilities of the Universal Sentence Encoder.

## Technologies Used
- **HTML/CSS**: For basic layout and styling.
- **JavaScript**: For user interaction and handling search functionality.
- **TensorFlow.js**: For running the Universal Sentence Encoder in the browser.
- **Universal Sentence Encoder**: To convert phrases into vector embeddings for semantic similarity calculations.

## Improvements
This project is a simple prototype. Future improvements could include:
- Adding a larger, more diverse dataset for testing the model.
- Optimizing embedding calculations to handle larger datasets more efficiently.
- Adding pagination or more complex UI components for better user experience.

## License
This project is licensed under the MIT License. Feel free to use, modify, and distribute it.

## Acknowledgments
- [TensorFlow.js](https://www.tensorflow.org/js) for enabling machine learning in the browser.
- [Universal Sentence Encoder](https://tfhub.dev/google/universal-sentence-encoder/4) for providing powerful semantic embeddings.

## Contact
For any questions or suggestions, please feel free to open an issue or reach out.

Happy coding!
