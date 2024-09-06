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
- **Multer:** For handling file uploads.
- **Google Generative AI:** For generating testing instructions based on screenshots.
- **Base64 Encoding:** For embedding screenshots in the prompt to the AI model.



