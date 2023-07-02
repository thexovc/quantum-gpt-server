# Quantum GPT Server

Quantum is a web application built with Express.js that utilizes the OpenAI API for text generation. It allows users to interact with an AI-powered chatbot by providing prompts and receiving responses.

## Installation

To run Quantum locally, follow these steps:

1. Clone the repository:

 ```bash
 git clone https://github.com/thexovc/quantum-gpt-server
```

2. Navigate to the project directory:

  ```bash
  cd quantum-gpt-server
  ```

3. Install the dependencies using npm:

  ```bash
  npm install
  ```

4. Install the dependencies using npm:

  ```bash
  OPEN_AI_KEY=your-api-key
  ```

## Usage
To start the Quantum server, run the following command:
```
npm start
```

The server will start listening on port 5000. You can access the server at http://localhost:5000/.

### Endpoints
#### GET /:

Description: Returns a simple "Hello from Quantum" message.
Example response:

```
{
  "message": "Hello from Quantum"
}
```

#### POST /:

Description: Sends a prompt to the server and receives an AI-generated response.
Request body:

```
{
  "prompt": "Your prompt goes here"
}
```
Example response:
```
{
  "bot": "The AI-generated response"
}
```

## Configuration
The Quantum application uses the following configuration options:

model: The OpenAI model to use for generating text completions. The default value is "text-davinci-003".
temperature: Controls the randomness of the generated output. Set to 0 for deterministic results.
max_tokens: Limits the length of the generated response.
top_p: Controls the diversity of the output. Set to 1 for full diversity.
frequency_penalty: Adjusts the penalty for repeating similar completions.
presence_penalty: Adjusts the penalty for not including keywords from the prompt.

Feel free to modify these options according to your requirements.


## Contributing
Contributions to Quantum are welcome! If you find any issues or want to add new features, please submit a pull request.

## Acknowledgments
The Quantum application is built using the Express framework.
Text completions are generated using the <a href="https://platform.openai.com/docs/api-reference" target="_blank">OpenAI API.</a>
