# PDF & Image Utility (Client-Side)

This is a simple web application designed for converting PDF files to image formats (PNG/JPG) and adding watermarks to both PDF and image files (PNG/JPG). The application is built to run entirely on the client-side using JavaScript, thus requiring no backend server for file processing.

## Key Features

  * **PDF Conversion:** Converts every page of a PDF file into a high-quality PNG image file.

  * **PDF Watermark:** Adds a transparent and repeating (diagonal) or centered text watermark to all pages of the PDF.

  * **Image Watermark:** Adds a text watermark to PNG or JPG image files.

  * **Flexible Input:** Supports file upload, drag & drop, and direct paste into the workspace.

## Technology Stack

The application uses third-party JavaScript libraries loaded via CDN, making it very lightweight and easy to deploy:

  * **Tailwind CSS:** For responsive styling and design.

  * **PDF.js:** Used to render PDF files to a Canvas element (necessary for conversion to images).

  * **PDF-lib:** Used for modifying PDF files and adding watermarks.

## Project Structure

The project consists only of the following files in the root directory:

```
/
|-- tool_konversi_watermark.html  <-- Main application file
|-- README.md                     <-- Indonesian guide
|-- README_EN.md                  <-- English guide (This file)
|-- serve.json                    <-- Local server configuration file
```

## Running Locally

You can run this application using a simple local web server (like `serve` from NPM) to ensure all features (especially file operations) are functioning correctly.

### 1\. Prerequisites

Ensure you have [Node.js](https://nodejs.org/) and NPM installed.

### 2\. Installing `serve`

`serve` is a lightweight static server that is easy to use:

```bash
npm install -g serve
```

### 3\. Starting the Server

The `serve.json` file automatically sets the default port to **8080**.

1.  Open your terminal in the directory containing `tool_konversi_watermark.html` and `serve.json`.

2.  Execute the following command:

      * **Foreground (Normal/Blocking Terminal):**
        ```bash
        serve .
        ```
      * **Background (Non-blocking Terminal - Linux/macOS Only):**
        Add the ampersand symbol (`&`) at the end.
        ```bash
        serve . &
        ```
        > **Note:** When running in the background, remember to note the *Process ID* (PID) that appears so you can stop the server later (use `kill [PID]`).

The application will be available at: `http://localhost:8080`.

> **Changing the Default Port:** To change the port, simply edit the `"port"` value inside the `serve.json` file.

## Deployment to GitHub Pages

Since this is a purely client-side application, deployment is straightforward:

1.  **Create Repository:** Create a new repository on GitHub (e.g., `pdf-image-utility`).

2.  **Upload Files:** Upload all files (`tool_konversi_watermark.html`, `README.md`, `README_EN.md`, and `serve.json`) to the repository.

3.  **Setup GitHub Pages:**

      * Go to your repository's **Settings**.

      * Select **Pages** from the side menu.

      * Under **Source**, pilih `Deploy from a branch` and pastikan **Branch** diatur ke `main` (atau `master`) and folder diatur ke `/(root)`.

      * Click **Save**.

GitHub Pages may take a few minutes to build and serve your site. Your application will be available at a URL like: `https://<username>.github.io/pdf-image-utility/tool_konversi_watermark.html`
