# Gemini API Postman Template (GSoC Proposal)

This repository contains Postman template files (a Collection and an Environment) for interacting with the Google Gemini API.

It was created as a demonstration for a Google Summer of Code (GSoC) 2025 proposal submitted to Google DeepMind (Project Idea #1: Develop a Gemini Workspace in Postman).

**This is a template and requires configuration before use.**

## How to Use

1.  **Download:** Download the `Gemini-API-Collection.postman_collection.json` and `Gemini-API-Environment.postman_environment.json` files from this repository.
2.  **Import into Postman:**
    *   Open Postman.
    *   Click the "Import" button (usually near the top left).
    *   Drag and drop both downloaded `.json` files into the import window, or use the "Upload Files" button.
    *   Confirm the import. You should now see "Gemini API Collection" under Collections and "Gemini API Environment" under Environments.

## ⚠️ Configuration Required!

The imported collection **will not work** until you configure the environment with your credentials:

1.  **Get your Gemini API Key:**
    *   Obtain an API key from Google AI Studio: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

2.  **(Optional) Find your Google Cloud Project ID:**
    *   You **only** need this if you plan to adapt requests to use Google Cloud Vertex AI endpoints (e.g., `https://[region]-aiplatform.googleapis.com/...`).
    *   Find your Project ID in the [Google Cloud Console](https://console.cloud.google.com/) (it's listed in the project selection dropdown at the top).

3.  **Edit the Postman Environment:**
    *   In Postman, go to the "Environments" tab on the left.
    *   Click on "Gemini API Environment".
    *   In the table that appears, locate the `GEMINI_API_KEY` variable. Paste **your own API key** into the **CURRENT VALUE** column.
    *   If needed, locate the `PROJECT_ID` variable and paste your Project ID into the **CURRENT VALUE** column.
    *   **Click "Save"** (top right of the environment tab) to save your changes.

## Running Requests

1.  Make sure the "Gemini API Environment" is selected as the active environment in Postman (dropdown menu usually at the top right).
2.  Navigate the "Gemini API Collection" folders and requests.
3.  Modify request bodies (e.g., change the prompt text) as needed.
4.  Click "Send".

---

**Disclaimer:** This is a template provided for proposal demonstration purposes. It needs your personal API key (and potentially Project ID) to function.
