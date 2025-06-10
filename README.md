# Resume-Parser(ATS)

Resume-Parser

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

## About the Project

The ATS (Applicant Tracking System) Resume Checker is a web application designed to help job seekers optimize their resumes for ATS systems. It allows users to upload their resumes (PDF or DOCX) and input keywords relevant to a job description. The application then analyzes the resume against the provided keywords, highlighting matches and suggesting areas for improvement to increase the resume's visibility to ATS.

## Features

* **Resume Upload:** Supports PDF and DOCX file formats.
* **Keyword Analysis:** Compares resume content with user-provided keywords.
* **Match Highlighting:** (If implemented) Visually indicates keyword matches.
* **User-Friendly Interface:** Built with Flask for a simple web interface.

## Technologies Used

* **Backend:**
    * Python 3.x
    * [Flask](https://flask.palletsprojects.com/): Web framework
    * [os](https://docs.python.org/3/library/os.html): For interacting with the operating system (file paths, directories)
    * [python-docx](https://python-docx.readthedocs.io/en/latest/): For reading .docx files
    * [fitz (PyMuPDF)](https://pymupdf.readthedocs.io/): For reading .pdf files
    * `utils.score_resume` (Custom module): For resume scoring logic
    * `doc2txt` (Custom module): For converting document content to plain text

* **Frontend:**
    * HTML
    * (Potentially CSS and JavaScript for styling and interactivity)

## Getting Started

To get a copy of the project up and running on your local machine for development and testing purposes, follow these steps.

### Prerequisites

* Python 3.x installed.
* `pip` (Python package installer).
* `venv` (Python virtual environment - generally comes with Python).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```
    *(Remember to replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME`)*

2.  **Create and activate a virtual environment:**
    ```bash
    python3 -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the Flask application:**
    ```bash
    python app.py
    ```
2.  **Open your web browser** and navigate to `http://127.0.0.1:5000/`.
3.  **Upload your resume** (PDF or DOCX) and enter the relevant keywords separated by commas.
4.  **Click "Submit"** to get your resume analysis.

## Project Structure
