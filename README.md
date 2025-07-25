# KEZEN - Event and Social Interaction Platform

KEZEN is a web platform designed for creating, finding, and participating in various events. It also includes social features for user interaction, a moderation system, and tools for administrators. The project is written in Python using the Flask framework.

## Key Features

* **User Management:** Registration, authentication, user profiles with avatars and interests.
* **Event Creation and Management:**
    * Adding events with descriptions, images, locations (including map coordinates), dates, times, and keywords.
    * Setting participant limits and minimum required ratings for participation.
    * Event moderation (approval/rejection).
* **Event Discovery and Participation:**
    * Convenient search and filtering of events (by name, date, city, categories).
    * Ability to join or leave an event.
    * Displaying events on a map.
* **Social Interaction:**
    * Friend system (requests, acceptance, removal).
    * Private messaging between users.
    * In-event chats (general and for administrators).
    * Likes and comments on events.
    * Reviews and ratings for events and users (organizers and participants).
* **Notifications:** Real-time alerts for new friend requests, messages, event statuses, likes, etc.
* **Tools for Administrators and Moderators:**
    * Moderation panel for managing events and users.
    * Announcement system with view and click tracking statistics.
* **AI Integration:**
    * Automatic event description generation using OpenAI.
    * "KEZEN" support chat powered by GPT to assist users.

## Tech Stack

* **Backend:** Python 3, Flask
* **Database:** SQLite (using Flask-SQLAlchemy)
* **Real-time Communication:** Flask-SocketIO (WebSockets)
* **Authentication:** Flask-Login
* **Artificial Intelligence:** OpenAI API
* **Frontend:** HTML, CSS, JavaScript (for interactivity and display)

## Prerequisites

* Python 3.8 or higher
* pip (Python package manager)
* A valid OpenAI API key (if AI features are to be actively used)

## Installation and Setup

1.  **Clone the repository (or copy the project files):**
    If you received the project as a set of files, simply create a folder for it.

2.  **Navigate to the project folder:**
    ```bash
    cd path/to/your/project
    ```

3.  **Create and activate a virtual environment:**
    * For macOS/Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    * For Windows:
        ```bash
        python -m venv venv
        venv\Scripts\activate
        ```

4.  **Install dependencies:**
    (Ensure you have a `requirements.txt` file. If not, create it with `pip freeze > requirements.txt` after manually installing all packages).
    ```bash
    pip install -r requirements.txt
    ```

5.  **OpenAI API Key:**
    Ensure your OpenAI API key is correctly specified in the `app.py` file (line `openai.api_key = "sk-proj-..."`). For more secure usage, configuring it via environment variables is recommended.

6.  **Run the application:**
    ```bash
    python app.py
    ```

7.  **Open the application in your browser:**
    Go to `http://127.0.0.1:5000`

## Project Structure (Simplified)