# Text-to-Speech Translator

This project is a Text-to-Speech (TTS) Translator that combines translation and speech synthesis capabilities to convert user input into audio in a selected language. It leverages browser speech synthesis APIs and a serverless translation service.

## Features
- Translate text into multiple supported languages.
- Convert translated text into speech using Text-to-Speech (TTS).
- Dynamic voice selection for available voices on the user's browser.
- User-friendly interface with language and voice dropdowns.

## Technologies Used
- **JavaScript** for client-side logic.
- **SpeechSynthesis API** for Text-to-Speech functionality.
- **Fetch API** for serverless translation requests.
- **HTML** and **CSS** for the user interface.

## Getting Started
### Prerequisites
- A modern web browser (e.g., Chrome, Firefox) that supports the SpeechSynthesis API.
- A serverless backend or API endpoint for translation (e.g., Google Cloud Translation API).

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/swapnildubey29/Translate-App.git
   ```
2. Navigate to the project directory:
   ```bash
   cd text-to-speech-translator
   ```
3. Open the `index.html` file in your web browser.

### Configuration
Ensure that your serverless translation API is set up to handle requests at the `/api/translate` endpoint. You may need to modify the fetch URL and headers in the `translateText` function to match your API configuration.

### Running the Project
1. Enter text into the provided text area.
2. Select a target language from the dropdown.
3. Choose a voice from the available options.
4. Click the "Play" button to hear the translated text.

## Project Structure
```
project-root/
├── index.html         # Main HTML file
├── styles.css         # Styling for the application
├── script.js          # JavaScript logic for TTS and translation
API/
├── translate.js       # API Integraion 
└── README.md          # Project documentation
```

## API Reference
### Translation Endpoint
- **URL**: `/api/translate`
- **Method**: POST
- **Request Body** (JSON):
  ```json
  {
    "text": "Your text here",
    "target": "Language code (e.g., en, es)"
  }
  ```
- **Response** (JSON):
  ```json
  {
    "data": {
      "translations": [
        {
          "translatedText": "Translated text here"
        }
      ]
    }
  }
  ```

## Supported Languages
The following languages are supported:
- English (`en`)
- Spanish (`es`)
- French (`fr`)
- German (`de`)
- Italian (`it`)

## Browser Compatibility
- Chrome
- Firefox
- Edge
- Safari (limited TTS support)

## Contributing
1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Create a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments
- [MDN Web Docs](https://developer.mozilla.org/) for SpeechSynthesis API documentation.
- [Google Cloud Translation API](https://cloud.google.com/translate) for translation services.

---

