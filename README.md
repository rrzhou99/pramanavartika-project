# Pramāṇavārttika: Multi-Lingual Data Alignment & OCR Pipeline

## Overview
This project is an automated data pipeline and interactive web application designed to digitize, structure, and align complex unstructured visual datasets. Specifically, it processes the classical *Pramāṇavārttika* manuscript, converting raw visual data (ancient Tibetan pecha/folios) into a structured, searchable, multi-lingual digital corpus. 

The system leverages an automated Python/OCR pipeline for text extraction and utilizes Gemini-powered workflows for multi-lingual curation, ultimately aligning the digital output verse-by-verse with the physical ground truth.

## Key Features

*   **Automated OCR & Data Pipeline:** Utilizes Python and the Google Cloud Vision API to batch-process unstructured image files, extract Tibetan script, and structure the raw output.
*   **Agentic AI & Prompt Engineering:** Employs Gemini to source, clean, and structure parallel datasets in three languages: Chinese, Tibetan, and Sanskrit.
*   **Ground-Truth Validation:** Features a precise "Text and Original Image Comparison" architecture, allowing users to cross-reference the extracted multi-lingual digital text directly against the Original Folio Scans (长函原始扫描档).
*   **Interactive Web Deployment:** The structured data is rendered into a responsive, static HTML/JS frontend hosted via GitHub Pages for global accessibility.

## System Architecture & Workflow

1.  **Data Ingestion (Visual):** Raw scans of the original folios are batch-processed and formatted using the Python `Pillow` library.
2.  **Data Extraction (OCR):** The Google Cloud Vision API extracts the physical script into raw digital text strings.
3.  **Data Structuring (LLM):** Gemini-assisted prompt engineering is used to clean the OCR output and perfectly align it with corresponding Sanskrit and Chinese translations.
4.  **Deployment (UI):** A version-controlled frontend merges the text arrays and image assets into a unified, verse-by-verse alignment interface.

## Tech Stack
*   **Backend & Data Processing:** Python, Pillow (PIL)
*   **AI & Telemetry:** Google Cloud Vision API, Gemini (LLM)
*   **Frontend Deployment:** HTML5, CSS3, JavaScript, GitHub Pages
*   **Version Control:** Git, GitHub Actions

## Access the Project
The compiled, user-facing alignment tool is deployed and live via GitHub Pages:
👉 **[Insert your GitHub Pages URL here, e.g., https://rrzhou99.github.io/pramanavartika-project/]**

## Project Context
This repository was developed as a hands-on technical initiative to apply modern ML/AI tooling, prompt engineering, and automated spatial/visual data remediation to classical manuscript preservation.