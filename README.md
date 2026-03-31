# TrackTracker 🏃‍♂️🏃‍♀️

A completely self-contained, offline-first Single-Page Application (SPA) designed to track middle school track and field events and athlete performance for the Ohio 2026 season.

## Key Features

*   **Zero Dependencies:** Everything is contained within a single `TrackTracker.html` file. No build processes, no npm, no servers.
*   **Offline-First:** All data is saved directly in your browser's LocalStorage. It works completely without an internet connection.
*   **Data Portability:** Quickly export your entire season's data to a JSON file for backup or sharing, and import it on any other device.
*   **Pre-configured Rules:** Includes the complete 2026 Ohio Middle School Track and Field event list, cleanly segregated by boys/girls divisions.
*   **Core Modules:** 
    *   **Athletes:** Manage your team roster.
    *   **Meets:** Log upcoming and past meet locations and dates.
    *   **Results:** Quick-add entry forms for race times and field distances/heights with live search and filtering.

## How to Use

1.  Download or clone this repository.
2.  Open `TrackTracker.html` in any modern web browser (Chrome, Firefox, Safari, Edge, Mobile Safari/Chrome).
3.  Add your Athletes in the "Athletes" tab.
4.  Add a Meet in the "Meets" tab.
5.  Start entering times and distances in the "Results" tab.
6.  *Important:* Periodically hit the "Export JSON" button in the top right to safely back up your team's data to a file.

## Requirements Document

Full design specifications, user requirements, and future stretch goals can be found in `PROMPT.md`.
