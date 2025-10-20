# Telegram Translator Bot 

A simple Telegram bot that translates text into different languages. This project was developed as a Software as a Service (SAAS) for a university Cloud Computing course.

## Features

* Translate any text to a specified destination language.
* Set a default destination language for translations.
* List all available languages for translation.
* Easy to deploy and run.

## Deployment (SAAS Model)

This bot is a practical implementation of the **Software as a Service (SAAS)** model. Instead of requiring users to run the code on their own machines, the bot is deployed and runs continuously on a cloud platform, providing translation services on demand.

* **Platform:** The application is hosted on **PythonAnywhere**, a cloud-based platform (PaaS) that allows for easy deployment and management of Python web applications.
* **SAAS Concept:** Users interact with the service (the translator bot) via the Telegram interface without needing to worry about the underlying code, servers, or maintenance. The service is available 24/7, just like any commercial SAAS product. This approach was central to fulfilling the requirements of the Cloud Computing course.

## How to Run Locally

If you want to run your own instance of the bot, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/nimabgr/telegram-translator-bot.git
    cd telegram-translator-bot
    ```

2.  **Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your environment variables:**
    You need an API key from BotFather on Telegram. Create a file named `.env` in the project root and add your API key:
    ```
    API_KEY="YOUR_TELEGRAM_BOT_API_KEY"
    ```
    *Note: The `.env` file is included in `.gitignore` and will not be uploaded to GitHub.*

5.  **Run the bot:**
    ```bash
    python Bot.py
    ```

## Technologies Used

* **Language:** Python
* **Libraries:**
    * [pyTelegramBotAPI](https://github.com/eternnoir/pyTelegramBotAPI)
    * [googletrans](https://pypi.org/project/googletrans/)
* **Deployment:** PythonAnywhere (Cloud Platform)
