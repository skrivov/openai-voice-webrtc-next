# OpenAI WebRTC Audio Next.js App

This is a WebRTC-based audio streaming application using OpenAI's API, developed with Next.js under the Deno runtime. It supports real-time audio interaction with OpenAI's models.

## Features
- **WebRTC Audio Streaming**: Stream audio in real-time.
- **OpenAI Integration**: Connects to OpenAI's real-time models via their API.
- **Next.js Framework**: Built with Next.js for server-side rendering and API routes.
- **Tailwind CSS**: Styled using Tailwind CSS.

## Requirements
- **Deno runtime**
- **Node.js** (optional, if not using Deno)
- OpenAI API Key

## Key WebRTC Concepts and Code Walkthrough

 Check out the [tutorial](./tutorial.md) for a brief explanation of WebRTC and code walkthrough.

## Docker setup

### 1. Clone the Repository
```bash
git clone https://github.com/skrivov/openai-webrtc-audio-next.git
cd openai-webrtc-audio
```
### 2. Build image and start container

`docker build -t voice -f Dockerfile`

`docker run -d -p 3000:3000 --name voice-app -e OPENAI_API_KEY=<key> voice`

### 3. Usage
1. Open the app in your browser: `http://localhost:3000`.

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/skrivov/openai-webrtc-audio-next.git
cd openai-webrtc-audio
```

### 2. Environment Setup
Create a `.env` file in the root directory:
```env
OPENAI_API_KEY=your-openai-api-key
```

### 3. Install Dependencies
If using **Node.js**:
```bash
npm install
```

If using **Deno**:
```bash
deno install
```

### 4. Run the Application

#### Using Node.js:
```bash
npm run dev
```

#### Using Deno:
```bash
deno task dev
```

The application will be available at `http://localhost:3000`.



## Usage
1. Open the app in your browser: `http://localhost:3000`.
3. Select a voice and start the audio session.

## Technologies Used
- **Next.js**: Framework for building React applications with server-side rendering.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **OpenAI API**: Integration with OpenAI's real-time models.
- **WebRTC**: Real-time communication API.
- **Deno**: Alternative runtime for the app.

## Contributing
1. Fork the repository.
2. Create a new branch.
3. Make your changes and commit them.
4. Push your branch and create a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements
- [OpenAI](https://openai.com/) for their API and models.
- [Next.js](https://nextjs.org/) for the framework.
- [Tailwind CSS](https://tailwindcss.com/) for styling.
- [Simon Willison’s Weblog](https://simonwillison.net/2024/Dec/17/openai-webrtc/) for inspiration
