# Remember every StackOverflow question you read using ChatGPT, Anki flashcards and Vonage Messages API

If you are a software developer, I can bet $1,000 you keep visiting the same StackOverflow (SO) questions multiple times. Will you take the bet?

Developer productivity is not a concern for employers only. Personally, being productive makes me feel proud and confident in myself.

Naturally, having to read the same SO question multiple times takes a toll on my productivity and confidence.

We can fix that with Spaced Repetition, a technique supported by academic research that helps with learning and memorization.

Every time we visit a relevant SO question, ChatGPT API will create flashcards, which will be stored in Anki, an open-source spaced repetition system (SRS).

Anki's schedule will determine when we need to review that information to keep it fresh in memory. Reviews will happen conveniently on WhatsApp, powered by Vonage Messages API.


## Requirements and Setup

Apart from ChatGPT to create flashcards and Vonage to send WhatsApp messages, we will use PythonAnywhere to run our app in the cloud.

Let's create every account and install all the software we need to start building this productivity app.


### Vonage

Create a free account at [Vonage](https://ui.idp.vonage.com/ui/auth/registration). Login and go to the [Messages API Sandbox](https://dashboard.nexmo.com/messages/sandbox) to enable WhatsApp. Follow instructions to validate your phone number.

Finally, get an API key at [API Settings](https://dashboard.nexmo.com/settings).


### Python Anywhere

Go to [www.pythonanywhere.com](www.pythonanywhere.com) and create a free account.

>>> Pending: instructions to setup a new app


### OpenAI / ChatGPT

Visit [platform.openai.com/signup](platform.openai.com/signup) and create an account. Enter a payment method to setup billing. Then go to [View API Keys](https://platform.openai.com/account/api-keys) and create a new secret key.


### Python

Download it from [python.org](https://www.python.org/downloads) (version 3.11 recommended).

Now setup a virtual environment:

```bash
python3.11 -m venv .env
```

Install dependencies:

```bash
pip install anki
pip install flask
```

## Let's go down to coding



