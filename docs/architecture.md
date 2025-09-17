# System Architecture (Draft)

## Overview
The OER Editor is a modular web application:
- **Frontend:** Next.js, React-based WYSIWYG editor, offline-first PWA
- **Backend:** Node.js REST/GraphQL API for AI orchestration and SCORM/xAPI package generation
- **Storage:** Courses stored as JSON files with Git versioning

## Key Components
- **AI Orchestration Layer:** separates prompts into outline → lesson → quiz → image lookup
- **Validation Layer:** schema checks, WCAG, license compliance
- **Exporters:** SCORM 1.2, SCORM 2004, xAPI (TinCanJS)

## Deployment
Supports Docker Compose for local development and cloud deployment.
