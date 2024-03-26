# Fiction Book Generator

This project utilizes OpenAI's API to automatically generate a fiction book. It creates an outline, populates the narrative with characters, settings, and plots, and sequentially generates text for each chapter and page.

## Prerequisites

Ensure you have Node.js installed on your system. You can download Node.js from [here](https://nodejs.org/).

## Setup

Follow these steps to set up and run the project:

### 1. Install Dependencies

Navigate to the project's root directory and run the following command to install the required dependencies:

```bash
npm install
```

### 2. Set Up Environment Variables

The application requires your OpenAI API key to interact with OpenAI's API. Create a `.env` file in the root directory and add your API key as follows:

```plaintext
API_KEY=your_openai_api_key_here
```

Replace `your_openai_api_key_here` with your actual OpenAI API key.

## Running the Application

The main script accepts four optional arguments:

- `modelChoice`: The AI model to use (e.g., 'gpt4'). Defaults to 'gpt4'.
- `desiredPages`: The total number of pages for the book. Defaults to 200.
- `chapterLength`: The number of pages each chapter should have. Defaults to 20.
- `padAmount`: Additional padding to adjust token limits. Defaults to 500.

To run the application, use the following command format in your terminal or command prompt:

```bash
node [main_script_name].js [modelChoice] [desiredPages] [chapterLength] [padAmount]
```

Replace `[main_script_name]` with the name of your main script file. If you're using the default settings, you can simply run:

```bash
node [main_script_name].js
```

## Output

The script will generate text files with the content of your book, including outlines, chapter summaries, and the full text for each chapter.
