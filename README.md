# Testing Instructions Generator

## Overview
The Testing Instructions Generator is a web-based tool designed to create detailed, step-by-step testing instructions for any digital product's features based on provided screenshots. It leverages a multimodal LLM (Google Generative AI’s Gemini model) to generate comprehensive test cases, including descriptions, pre-conditions, testing steps, and expected results.

## Features
- **Contextual Input:** Optional text input for additional context about the screenshots.
- **Multi-Image Upload:** Upload multiple screenshots of the digital product's features.
- **Instructions Generation:** Generate detailed test cases based on the screenshots and optional context.
- **Result Display:** View generated instructions in a user-friendly format with Markdown rendering.

## Technology Stack

### Front-End
- **React:** For building the user interface.
- **Axios:** For making HTTP requests to the backend.
- **React Markdown:** For rendering Markdown content in the result.

### Back-End
- **Express:** For creating the server and handling API requests.

## Project Structure


## Installation and Setup

### Front-End
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/your-repository.git
    ```
2. Navigate to the front-end directory:
    ```bash
    cd your-repository/src
    ```
3. Install dependencies:
    ```bash
    npm install
    ```
4. Start the development server:
    ```bash
    npm start
    ```

### Back-End
1. Navigate to the server directory:
    ```bash
    cd your-repository/backend
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the server:
    ```bash
    node server.js
    ```

## How to Use

1. **Open the Web Application:** Navigate to `http://localhost:3000` in your web browser.
2. **Enter Context (Optional):** Provide any additional context about the screenshots in the "Optional Context" text area.
3. **Upload Screenshots:** Click on the file upload area to select and upload multiple screenshots.
4. **Generate Testing Instructions:** Click the "Generate Testing Instructions" button to process the screenshots and context.
5. **View Results:** The generated instructions will be displayed in the results section below the form.

## Prompting Strategy

### Overview
The prompting strategy guides the multimodal LLM to generate detailed test cases based on the provided screenshots and optional context. The prompt is designed to ensure that the generated instructions are clear, actionable, and comprehensive.

### Prompt Construction

1. **Base Prompt:**
   The base prompt is structured to request detailed test cases:
   ```text
   Generate a detailed, step-by-step guide on how to test each functionality based on the provided screenshots. For each test case, include the following details:
   
   1. **Description**: What is this test case about?
   2. **Pre-conditions**: What needs to be set up or ensured before starting the test?
   3. **Testing Steps**: Provide clear, step-by-step instructions on how to perform the test.
   4. **Expected Result**: What should happen if the feature works correctly?
   
   The screenshots provided are as follows:

- **Multer:** For handling file uploads.
- **Google Generative AI:** For generating testing instructions based on screenshots.
- **Base64 Encoding:** For embedding screenshots in the prompt to the AI model.



