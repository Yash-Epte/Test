# ChatEzy

> *Where Chat Made Simple*

ChatEzy is a lightweight, user-friendly chatbot application that provides interactive conversations along with relevant follow-up suggestions. The application features a clean, modern interface with a responsive design.

![WhatsApp Image 2025-03-19 at 22 59 31](https://github.com/user-attachments/assets/580a42c9-b629-482b-b72c-4caabc877939)

![WhatsApp Image 2025-03-19 at 23 01 59](https://github.com/user-attachments/assets/12e2edb8-3f15-4381-99e9-33d459c2324a)

![WhatsApp Image 2025-03-19 at 23 00 43](https://github.com/user-attachments/assets/c2df4b1e-e7ac-446e-8fc8-652495d18242)

## Features

- 🤖 **AI-Powered Chat**: Conversational interface powered by OpenAI's GPT models
- 💡 **Smart Suggestions**: Automatically generates relevant follow-up questions
- ⚡ **Real-time Responses**: Quick and responsive chat experience
- 🧩 **Simple UI/UX**: Clean, intuitive interface for seamless interaction

## Tech Stack

- **Frontend**: React with TypeScript
- **Backend**: Flask (Python)
- **AI Integration**: OpenAI API
- **Styling**: Custom CSS with responsive design

## Getting Started

### Prerequisites

- Node.js (v16.0 or later)
- Python (v3.8 or later)
- OpenAI API key

### Installation

#### Clone the repository

```bash
git clone https://github.com/yourusername/chatezy.git
cd chatezy
```

#### Frontend Setup

```bash
# Navigate to the frontend directory (if not already in the root)
cd frontend  # If your frontend is in a separate directory

# Install dependencies
npm install

# Start the development server
npm run dev
```

The frontend will be available at http://localhost:5173 (or another port if configured differently).

#### Backend Setup

```bash
# Navigate to the backend directory (if not already in the root)
cd backend  # If your backend is in a separate directory

# Create and activate a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Set your OpenAI API key
export OPENAI_API_KEY="your-api-key-here"  # On Windows, use `set OPENAI_API_KEY=your-api-key-here`

# Start the Flask server
python app.py
```

The backend API will be available at http://localhost:4254.

## Usage

1. Open your browser and navigate to the frontend URL (default: http://localhost:5173)
2. Type your question or message in the input field
3. Press Enter or click the Send button
4. View the AI response and suggested follow-up questions
5. Click on any suggestion to automatically fill the input field

## Project Structure

```
chatezy/
├── frontend/               # React frontend
│   ├── src/
│   │   ├── App.tsx         # Main application component
│   │   └── App.css         # Styling
│   └── package.json
│
├── backend/                # Flask backend
│   ├── app.py              # Main Flask application
│   └── requirements.txt    # Python dependencies
│
└── README.md               # Project documentation
```

## Environment Variables

### Backend

- `OPENAI_API_KEY`: Your OpenAI API key

## Customization

### Changing the Theme Colors

You can modify the theme colors by editing the CSS variables in `App.css`:

```css
:root {
  --text-color: #333;
  --orange-theme: #F86A38;
  --ai-message-color: #948f8f;
  --user-message-color: #F86A38;
}
```

### Changing the Model

To use a different AI model, modify the `model` parameter in the `chat()` function in `app.py`:

```python
response = client.chat.completions.create(
    model="your-preferred-model",  # Change this line
    messages=openai_messages
)
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [OpenAI](https://openai.com/) for providing the API that powers the chat functionality
- [React](https://react.dev/) for the frontend framework
- [Flask](https://flask.palletsprojects.com/) for the backend framework

---

Created with ❤️ by [Your Name]
