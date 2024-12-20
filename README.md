# Simple Code Editor

## Description

This is a web-based code editor application built with React and Vite. The project allows users to write, execute, and view the results of code snippets in two programming languages: JavaScript and Python. It includes syntax highlighting, a simple UI, and a mock server to simulate code execution.

## Features

- Code Editing: Write code with syntax highlighting for JavaScript and Python using CodeMirror.
- Language Selection: Switch between JavaScript and Python via a dropdown.
- Code Execution: Send code to a mock server and view the output or error messages.
- Responsive Design: Optimized for different screen sizes.

## Live Demo

The project is deployed and accessible at Live URL.

## Installation and Setup

Follow these steps to run the project locally:

### Prerequisites

- Node.js (v14 or higher)
```bash
npm or yarn
```
### Steps

1. Clone the repository:
```bash
git clone https://github.com/<your-username>/<your-repository-name>.git
```

2. Navigate to the project directory:
```bash
cd <my_project>
```

3. Install dependencies:
```bash
npm install
```

4. Start the development server:
```bash
npm run dev
```

5. Open your browser and navigate to the URL provided in the terminal (e.g., http://localhost:5173).

## Folder Structure
```bash
<my_project>/
├── public/        # Static assets
├── src/           # Source files
│   ├── components/   # React components
│   ├── App.jsx       # Main application file
│   ├── main.jsx      # Application entry point
│   ├── styles/       # Stylesheets
├── vercel.json   # Configuration for deployment on Vercel
├── package.json  # Dependencies and scripts

```

## Mock Server

The application uses miragejs to mock a backend server for code execution. The mock server simulates processing the submitted code and returns either a success message or an error.

## Example Request

Endpoint: /api/execute

Request Body:

{
  "language": "javascript",
  "code": "console.log('Hello, world!');"
}

Response:

Success:

{
  "status": "success",
  "output": "Hello, world!\n"
}

Error:

{
  "status": "error",
  "error": "SyntaxError: Unexpected token"
}

## Deployment

The project is deployed on Vercel. The deployment process includes the following steps:

1. Push the latest code to GitHub.

2. Log in to Vercel and import the repository.

3. Configure the deployment settings:

4. Specify the root directory if necessary (e.g., frontend).

5. Add a vercel.json file for custom builds if required.

6. Deploy the project.

## Future Enhancements

- Add support for additional programming languages.

- Implement real backend execution using a cloud-based API or server.

- Improve error handling and feedback.

- Enhance the UI/UX with more themes and customization options.

## License

This project is open-source and available under the MIT License.

![MIT License](https://img.shields.io/badge/license-MIT-green)
