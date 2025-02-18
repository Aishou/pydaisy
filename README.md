# pydaisy

pydaisy is a Python port of the Daisy chatbot. The Daisy chatbot is a conversational AI that learns from user input and generates responses based on its memory. This project aims to provide a modern implementation of the Daisy chatbot using Python.

## Features

- Conversational AI that learns from user input
- Generates responses based on its memory
- Supports multiple chatbots with different personalities
- Easy to extend and customize

## Installation

To install pydaisy, you need to have Python 3.x installed on your system. You can install the required dependencies using pip:

```bash
pip install -r requirements.txt
```

## Usage

### Importing the original Daisy memory file

To import the original Daisy memory file (e.g., `MEM.DSY`), use the following command:

```bash
python sqlite/ImportText.py botname ../MEM.DSY
```

### Running the chatbot with learning support

To run the chatbot with learning support, set the `BOTNAME` and `LEARN` variables in the `sqlite/Tests.py` file, and then execute the following command:

```bash
python sqlite/Tests.py chatbot
```

### Running the chatbot without learning support

To run the chatbot without learning support, use the following command:

```bash
python sqlite/Memory.py botname
```

## Available Scripts

### `sqlite/ImportText.py`

This script imports the original Daisy memory file into the SQLite database. It takes two arguments: the bot name and the path to the memory file.

### `sqlite/Tests.py`

This script provides a command-line interface for interacting with the chatbot. It supports two modes: `chatbot` and `respbenchmark`. The `chatbot` mode allows you to chat with the bot, while the `respbenchmark` mode measures the response generation speed.

### `sqlite/Memory.py`

This script provides functions for managing the chatbot's memory, including inserting new phrases, generating responses, and learning from user input.

## Project Structure

The project is organized as follows:

- `funstuff/`: Contains various scripts and files related to the chatbot.
- `sqlite/`: Contains scripts and files related to the SQLite database and memory management.
- `MEM.DSY`: The original Daisy memory file.
- `LICENSE`: The license file for the project.
- `README.md`: This file.

## License

This project is licensed under the GNU General Public License v2.0. See the `LICENSE` file for more information.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any suggestions or improvements.

## Contact

For any questions or inquiries, please contact the project maintainer at [email@example.com].

## Related Resources

- [ChatterBot API](http://code.google.com/p/chatter-bot-api/): The original library used for the Daisy chatbot.
