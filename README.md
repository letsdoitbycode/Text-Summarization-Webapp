# Text Summarization Project with Flask and Pegasus Transformer

This Flask application utilizes the Pegasus Transformer model by Google for conditional text summarization. It allows users to input large text and receive a concise summary, making it ideal for processing articles, reports, or any long-form text data.

### Features
- Text Summarization: Uses the PegasusForConditionalGeneration model to generate a summary for the input text.
- CUDA Optimization: Leverages CUDA if available, allowing for faster summarization on GPU devices.
- Responsive Web Interface: The application provides a user-friendly interface with index.html for input and output.html to display results.

### How It Works
- Input: The user submits text via a form on the home page.
- Text Tokenization: The input text is tokenized and encoded for the Pegasus model.
- Summarization: The model generates a summary with specified minimum and maximum length constraints.
- Output: The summary is decoded and displayed on the output page.

### Requirement 
- Python >= 3.10
- Flask
- Transformers
- gunicorn
- sentencepiece
- torch

### Installation
1. Clone the repository
   ```sh
   git clone https://github.com/letsdoitbycode/Text-Summarization-Webapp.git
   cd Text-Summarization-Webapp
   ```

3. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```sh
   pip install flask transformers torch sentencepiece gunicorn
   pip install requirements.txt   #else you can do this directly
   ```
   
4. Run the Flask app:
    ```sh
    python app.py
    ```

### Project Structure
```plaintext
Text-Summarization-Webapp/
│
├── app.py                  # Main Flask application
├── templates/
│   └── index.html          # Main HTML file
│   └── index.html          # Main HTML file
└── README.md               # This README file
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.
