<!-- A basic project description and setup guide. -->

# Twin Health AI Assistant
- This is an intelligent chatbot powered by Gemini AI and built with Django is developed for Twin Health
- It is designed to classify SMS conversations into three main topics based on specific business rules:
1. *LAB*
2. *TWIN_APPOINTMENT*
3. *OTHERS*
- It utilizes a Retrieval-Augmented Generation (RAG) approach to handle contextual and rule-based classification.


## Features of Twin Health AI Assistant
- AI-powered conversations using Claude Sonnet 4
- Persistent conversation storage
- Beautiful modern UI with animations
- Session management
- Admin panel for managing conversations
- Quick reply buttons
- Chat history loading
- Responsive design


## Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd twin_health_chatbot
    ```

2.  **Set up the Virtual Environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate     # On Windows
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables:**
    Create a `.env` file in the `chatbot_project` directory and add your secret keys:
    ```
    SECRET_KEY='<My_Django_Secret_Key>'
    DEBUG=True
    GEMINI_API_KEY='<My_Gemini_API_Key>'
    ```

5.  **Run Migrations and Server:**
    ```bash
    python manage.py makemigrations chat
    python manage.py migrate
    python manage.py runserver
    ```

The application will be accessible at `http://127.0.0.1:8000/`.

## Admin Panel
Visit http://127.0.0.1:8000/admin/ to manage conversations and messages.

## License
MIT License
