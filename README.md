# friend.tech WebSocket Client

This code provides a simple WebSocket client for the blockchain social app named "friend.tech". It allows you to connect to the platform's WebSocket, retrieve messages, and send messages.

## Requirements

- Python 3.x
- Required libraries: `websocket`, `json`, `uuid`, `os`, `dotenv`

You can install these libraries using pip:

```bash
pip install websocket-client python-dotenv
```

## Setup
- Create a .env file in the root directory of the project.
- Add your authentication token to the .env file:

``` AUTH_TOKEN=your_auth_token_here```

Replace your_auth_token_here with your actual authentication token.

## How to Use
1. Run the script:

```python main.py```


Upon running, the script will open a WebSocket connection to "friend.tech" and automatically request chat messages.

If you wish to send a message to the platform, you can utilize the send_message function:

```send_message(ws, "Your message here")```

Replace "Your message here" with the message you want to send.


## Functions
**on_message(ws, message)**: Handles incoming messages and prints them.

**on_open(ws)**: Executed when the WebSocket connection is opened. It sends a request to retrieve chat messages.

**send_message(ws, text)**: Sends a message to the platform.

## Note
Ensure that you keep your AUTH_TOKEN private and do not expose it in any public repositories or platforms.