# AI from Scratch

Tinkering with ai.

## Prerequisites

- **Python 3.9**: Required for TensorFlow compatibility. Install via Homebrew on macOS (`brew install python@3.9`) or from [python.org](https://www.python.org/downloads/release/python-390/).
- **Git**: To clone the repository (`brew install git` on macOS).

## Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/ai_from_scratch.git
   cd ai_from_scratch
   ```

2. **Create and Activate a Virtual Environment**:
   Use Python 3.9 to ensure compatibility:
   ```bash
   python3.9 -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Chatbot**:
   ```bash
   python src/chatbot.py
   ```
   The chatbot trains on a small text corpus (Alice in Wonderland) for 10 epochs (~5–10 minutes) and starts an interactive loop. Type messages (e.g., "Hello!"), and the bot responds. Type `quit` to exit and view the conversation history.

## Project Structure

- `src/`: Python scripts (e.g., `chatbot.py`).
- `data/`: Datasets for training (currently uses online data from Project Gutenberg).
- `requirements.txt`: Lists dependencies (TensorFlow, NumPy, requests).
- `.gitignore`: Excludes virtual environment, data, and model files.

## Notes

- For better responses, increase the `epochs` in `src/chatbot.py` (e.g., `epochs=50`).
- If you encounter TensorFlow issues, ensure you’re using Python 3.9 and run `pip install --upgrade pip`.
- Future plans include adding reinforcement learning and embodiment features.
