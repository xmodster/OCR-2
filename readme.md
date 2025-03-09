# Mistral AI OCR Document Viewer

This web application allows you to perform Optical Character Recognition (OCR) on PDF documents using the Mistral AI API.  It provides a user-friendly interface to upload a PDF, preview it, and then process it to extract text and images. The results are displayed in Markdown, image, and raw JSON formats.

## Features

*   **PDF Preview:**  View your PDF document directly in the browser before processing.
*   **Drag and Drop Upload:** Easily upload PDF files by dragging and dropping them onto the designated area, or by using the file selection button.
*   **Mistral AI OCR Processing:** Leverages the Mistral AI API to perform OCR on the uploaded PDF.
*   **API Key Input:** Securely enter your Mistral AI API key to access the OCR service.
*   **Results in Multiple Formats:** View the OCR output as:
    *   **Markdown:**  Clean, formatted text representation of the document.
    *   **Images:** Extracted images from the PDF, displayed with optional captions.
    *   **Raw JSON:**  The complete, unprocessed JSON response from the Mistral AI API for debugging or advanced use.
*   **Loading Indicator:**  Visual feedback during the OCR processing to inform the user of the ongoing operation.
*   **MathJax Support:** Renders mathematical expressions in the Markdown output using MathJax.

## How to Use

1.  **Obtain a Mistral AI API Key:** You will need an API key from Mistral AI to use this application. If you don't have one, you can sign up on the [Mistral AI platform](https://mistral.ai/) to get your API key.
2.  **Enter your API Key:**  In the "Mistral AI API Key" section, enter your API key into the provided input field. This key is stored in your browser's memory for the current session and is not persisted or sent to any third-party server by this application itself (all API calls are made directly from your browser to Mistral AI).
3.  **Upload a PDF Document:**
    *   **Drag and Drop:** Drag a PDF file from your computer and drop it into the "Drag & drop PDF file here" area.
    *   **Select PDF:** Click the "Select PDF" button to open a file dialog and choose a PDF file from your computer.
4.  **Preview the PDF:** Once uploaded, the PDF document will be displayed in the "PDF Preview" section. You can navigate through the pages using the "Previous" and "Next" buttons below the preview.
5.  **Process with OCR:** Click the "Process with OCR" button. The application will then:
    *   Display a "Processing document with Mistral AI..." loading indicator.
    *   Upload the PDF to the Mistral AI API for OCR processing.
    *   Retrieve the OCR results from the API.
6.  **View OCR Results:** After processing is complete, the "OCR Results" section will appear. You can switch between different tabs to view the results in:
    *   **Markdown:** (Default view) Formatted text output.
    *   **Images:** Extracted images.
    *   **Raw JSON:**  The raw API response.

## Prerequisites

*   **Mistral AI API Key:**  Required to access the Mistral AI OCR service.
*   **Modern Web Browser:**  The application is designed to work with modern web browsers that support JavaScript and HTML5 (e.g., Chrome, Firefox, Safari, Edge).

## Technologies Used

*   **HTML, CSS, JavaScript:** For the user interface and application logic.
*   **PDF.js:**  (from Mozilla) For rendering PDF documents in the browser.
    *   [https://mozilla.github.io/pdf.js/](https://mozilla.github.io/pdf.js/)
*   **marked.js:** For parsing and rendering Markdown text to HTML.
    *   [https://github.com/markedjs/marked](https://github.com/markedjs/marked)
*   **MathJax:** For rendering mathematical expressions in the browser.
    *   [https://www.mathjax.org/](https://www.mathjax.org/)
*   **Mistral AI API:**  For performing Optical Character Recognition.
    *   [https://mistral.ai/api/](https://mistral.ai/api/)
*   **jsDelivr CDN:** For hosting and delivering libraries (PDF.js, marked.js, MathJax).
    *   [https://www.jsdelivr.com/](https://www.jsdelivr.com/)

##  Potential Improvements (Future Enhancements)

*   **Error Handling Enhancements:**  More detailed and user-friendly error messages for API failures and other issues.
*   **Progress Indication during OCR:**  More granular progress updates during the OCR process, potentially showing page-by-page processing.
*   **Download Results:**  Option to download the OCR results in Markdown, JSON, or text format.
*   **Language Selection:**  Allow users to specify the language of the document for potentially improved OCR accuracy.
*   **API Key Persistence:**  Option to store the API key locally (using browser local storage) for convenience across sessions (with appropriate security warnings).

---

**Disclaimer:** This is a viewer application that utilizes the Mistral AI API. Usage is subject to Mistral AI's terms of service and API usage guidelines. Please ensure you are aware of any usage limits and costs associated with the Mistral AI API.