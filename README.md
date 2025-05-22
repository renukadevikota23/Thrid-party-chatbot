# Chatbot Web App with Together.ai API

A simple web-based chatbot application built with **Flask** (Python backend) and **HTML/JavaScript** frontend. It sends user input to the **Together.ai LLM API** (Mistral 7B model) and displays AI-generated responses in real time.

---

## Features

* Interactive chat interface in the browser
* Uses Together.ai API to generate responses with a powerful LLM
* Clean, minimal UI built with HTML and vanilla JavaScript
* Runs locally on your machine or server
* Easy to customize and extend

---

## Prerequisites

* Python 3.7 or higher
* Together.ai API key ([Sign up here](https://www.together.xyz))
* `pip` to install dependencies

---

## Installation & Setup

1. **Clone the repository** (or copy the project files):

   ```bash
   git clone https://github.com/yourusername/chatbot-togetherai.git
   cd chatbot-togetherai
   ```

2. **Install required Python packages:**

   ```bash
   pip install flask requests
   ```

3. **Add your Together.ai API key**

   Open `app.py`, replace:

   ```python
   API_KEY = "your_together_api_key"
   ```

   with your actual API key.

4. **Run the Flask app**

   ```bash
   python app.py
   ```

5. **Open your browser**

   Go to [http://localhost:5000](http://localhost:5000) to use the chatbot.

---

## Project Structure

```
chatbot-togetherai/
│
├── app.py                # Flask backend code
├── requirements.txt      # Python dependencies (optional)
└── templates/
    └── index.html        # Frontend HTML + JavaScript
```

---

## How It Works

* The user types a message in the browser input box.
* JavaScript sends the message via POST request to `/chat` endpoint.
* Flask backend receives the message, calls the Together.ai API with it.
* The API returns an AI-generated response.
* Flask sends the response back to the frontend.
* The frontend displays the bot reply under the chat.

---

## Customize

* Change the LLM model by editing `model` in `app.py` payload
* Modify UI styles in `templates/index.html`
* Add session/chat history for better context
* Deploy to cloud platforms like Heroku, Render, or VPS

---

## Troubleshooting

* **Flask server not running?** Check Python version and dependencies.
* **API errors?** Confirm your API key is valid and has access.
* **"Refused to connect"?** Make sure Flask runs and you open the right URL.
* **Port in use?** Change port in `app.run(port=xxxx)`.

---

## License

MIT License — free to use and modify.

---

## Contact

For questions or support, reach me at:
* GitHub: [github.com/yourusername](https://github.com/renukadevikota23)
