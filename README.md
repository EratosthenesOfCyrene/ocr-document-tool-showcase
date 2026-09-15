# OCR & Document Research Tool

A software project focused on OCR, document processing and the practical use of digitised material in research-oriented workflows.

The project combines several technologies for working with PDF and image documents across desktop and mobile components.

This repository is a **public showcase** of selected aspects of the project.  
The complete implementation and source code are maintained privately.

## Project Overview

The project started as an OCR application for analysing PDF and image documents and has gradually developed into a broader document-processing system.

Its current scope includes:

- importing and processing PDF and image documents
- OCR using multiple recognition engines
- image preprocessing and correction
- analysis and review of recognised text
- document navigation and structured workflows
- integration with complementary desktop and mobile components

The application is designed with research-oriented document workflows in mind.

## Preview

Screenshots and additional visual documentation will be added to this showcase repository.

## Core Features

### OCR and text recognition

The application supports multiple OCR workflows and recognition engines.

Current functionality includes:

- OCR of PDF and image files
- support for scanned and digitally generated PDFs
- integration of multiple OCR engines
- comparison of OCR results
- confidence-based evaluation of recognised text
- identification of low-confidence words
- word frequency analysis
- contextual display of recognised words
- export of OCR results

OCR technologies used in the project include:

- PaddleOCR
- Scribe.js
- Tesseract.js

### Example of text recognition
  ![Text recognition example](./assets/screenshots/text_recognition_example.png)

### Document image processing

Before OCR, document images can be prepared and corrected.

Features include:

- contrast enhancement
- sharpening
- adaptive thresholding
- automatic inversion
- deskewing
- document corner detection
- perspective correction
- page dewarping
- manual correction of detected document boundaries

Several local processing components are used so that document images can be processed without depending entirely on external cloud services.

### Example of manual deskewing
![Document deskew example](./assets/screenshots/deskew_example.png)

### PDF processing

The application supports document-oriented PDF workflows, including:

- PDF import
- scanned document processing
- page-based OCR analysis
- searchable PDF generation
- merging OCR results with document pages
- navigation between recognised text and the original page

## Text Analysis

Recognised text can be analysed directly inside the application.

The interface provides functionality such as:

- word frequency lists
- text contexts
- word highlighting
- confidence information
- navigation between occurrences
- identification of potentially incorrect OCR results

The aim is not only to extract text, but also to make OCR results easier to inspect and use in research workflows.

### Recognized words overview placed over the initial recognized image
![Word confidence overview](./assets/screenshots/word_confidence_overview.png)

### Clickable List of low confidence words 
![Word confidence details](./assets/screenshots/word_confidence.png)

### List of the word frequency within the analyzed text
![Word frequency list](./assets/screenshots/word_frequency_list.png)


## Document Integration

The project includes functionality for connecting document-processing workflows with external applications.

This allows recognised and processed document content to be used beyond the OCR application itself while keeping the individual software components clearly separated.

### Microsoft Word Integration

The application includes an integration with Microsoft Word based on Microsoft Office.js.

The integration demonstrates communication between the desktop application and an external productivity application and forms part of the project's broader document-processing architecture.
### Word add-in
![Microsoft Word add-in](./assets/screenshots/word_addin.png)

<!--  ### Links opened in the OCR & Document Research Tool  -->
<!--![Cited PDF in the OCR tool](./assets/screenshots/cited_pdf_ocr-tool.png) -->



## Document Identity and Versioning

Historical and research documents may change over time.

Pages can be inserted, removed, reordered or replaced while references to the document already exist.

The application therefore includes a document identity and versioning concept designed to preserve reliable references across changing document versions.

This requires the application to distinguish between documents, document versions and individual pages while maintaining the relationship between existing source references and the underlying material.

The long-term goal is to keep source references usable even when a document is replaced by a modified version.

The detailed matching and identification mechanisms are part of the private implementation.



## `.ocrproject` Exchange Format

The desktop and mobile components exchange document projects through a dedicated project format.

The format preserves the structure of a capture project together with the information required for continued processing on the desktop application.

This allows document capture and OCR processing to remain separate while maintaining project structure and source provenance.

The detailed format specification and internal data model are intentionally not part of this public showcase.

The mobile application intentionally focuses on document capture rather than performing OCR directly on the phone.

Captured projects can then be transferred to the desktop application for further processing.

### Android app overview
![Android app main screen](./assets/screenshots/android_app_main.jpg)

<!--   ### Android app project overview

![Android app project overview](./assets/screenshots/android_app_project.jpg)

### List of images in a project

![Images within an Android app project](./assets/screenshots/android_app_project_images.jpg)   -->

### Taking a photo 

![Taking a document photo with the Android app](./assets/screenshots/android_app_take_photo.jpg)



<!--
## Architecture

![OCR Document Tool project overview](./assets/screenshots/project_overview.png)
-->


## Technologies

### Desktop application

- JavaScript
- HTML5
- CSS3
- Electron
- Node.js

### Backend and document processing

- Python
- FastAPI
- REST APIs
- OpenCV
- PaddleOCR
- image-processing services

### OCR

- PaddleOCR
- Scribe.js
- Tesseract.js

### Mobile application

- Kotlin
- Android
- Android Studio

### Document integration

- PDF processing
- Microsoft Office.js
- Word Add-in
- JSON
- local application APIs
- custom deep links

### Development and architecture

- Git / GitHub
- REST-based communication
- asynchronous processing
- document identity management
- data validation
- versioned project formats

## Technical Challenges

The project involves several problems that go beyond basic OCR.

Examples include:

- coordinating multiple OCR engines
- evaluating different OCR results
- processing large documents
- maintaining page and document identity
- keeping citations valid when documents change
- connecting desktop and mobile applications
- exchanging structured document projects
- integrating a desktop application with Microsoft Word
- coordinating multiple local processing services
- preserving document provenance throughout the workflow

These challenges have required not only implementation work, but also the design of data structures, interfaces and application workflows.

## What I Have Learned

Working on this project has given me practical experience with:

- designing a larger software application
- breaking complex requirements into separate components
- frontend and backend communication
- REST interfaces
- asynchronous workflows
- desktop application development with Electron
- Python backend services
- OCR and document-processing technologies
- Android development with Kotlin
- document metadata and identity
- versioning concepts
- integration between independent applications
- debugging multi-component systems
- designing software around real user workflows

An important part of the project has been translating problems from practical document work into technical requirements and software functionality.

## Project Context

The project is independently developed and is currently under active development.

It combines my interests and experience in:

- software development
- document processing
- archives and historical sources
- research workflows
- digitisation
- OCR
- digital source referencing

The project is independently developed and remains under active development.


