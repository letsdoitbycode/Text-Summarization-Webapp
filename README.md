### Features
- Enter text directly into the text area to generate a summary.
- Flashy and interactive UI elements for an engaging user experience.

### Requirement 
- Python >= 3.10
- Flask
- Transformers
- gunicorn
- sentencepiece

### Installation
1. Clone the repository
   ```sh
   git clone https://github.com/Kabilduke/Text_Summarizer_BART.git
   cd Text_Summarizer_BART
   ```

3. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```sh
   pip install flask PyPDF2 transformers
   ```
   
4. Run the Flask app:
    ```sh
    python app.py
    ```

### Project Structure
```plaintext
Text_summarizer_BART/
│
├── app.py                  # Main Flask application
├── templates/
│   └── index.html          # Main HTML file
├── static/
│   ├── style.css           # CSS styles
├── uploads/                # Directory to store uploaded PDF files
└── README.md               # This README file
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.
