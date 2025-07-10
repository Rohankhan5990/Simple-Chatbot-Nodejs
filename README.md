# Simple Chatbot Node.js API

This is a simple chatbot API built with Node.js and Express. The chatbot can respond to various user messages with predefined answers, including greetings, date/time queries, fun facts, jokes, and more.

## Features
- Responds to common greetings and questions
- Provides current date and time
- Shares fun facts and jokes
- Answers basic knowledge questions
- Offers default responses for unrecognized messages

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v12 or higher recommended)
- [npm](https://www.npmjs.com/)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Simple-Chatbot-Nodejs.git
   cd Simple-Chatbot-Nodejs
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running the Server
Start the server with:
```bash
node server.js
```
The server will run at [http://localhost:3000](http://localhost:3000).

## API Usage

### Endpoint
`POST /chat`

#### Request Body
```json
{
  "message": "Your message here"
}
```

#### Response
```json
{
  "response": "Chatbot's reply"
}
```

#### Example
Request:
```bash
curl -X POST http://localhost:3000/chat -H "Content-Type: application/json" -d '{"message": "hello"}'
```
Response:
```json
{
  "response": "Hello! How can I assist you today?"
}
```

## Customization
You can add more responses or modify existing ones in `server.js` by editing the message handling logic.

## License
This project is licensed under the MIT License.

