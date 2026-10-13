# Image_Gallery_Gen
Stockholm Innovation Lab Testimony Wall

A playful, Ericsson-inspired testimony wall for collecting and displaying reflections from the Stockholm Innovation Lab.

Features





Add testimonies with an optional word or tag



Choose a card color and display each testimony as a pinned note



Delete individual testimonies



Save the current wall in browser storage



Export the wall as a reusable JSON file



Import a previously exported JSON file



Restore saved browser state automatically when the page is reopened



Responsive layout for desktop and mobile screens



Keyboard-accessible controls and reduced-motion support



Print-friendly layout for PDF export or browser printing

Getting started





Download or clone the repository.



Open stockholm_innovation_lab_testimony_wall.html in a modern browser.



Select Add testimony to pin a new message.



Use Save to file to download a backup of the current wall.



Use Import file to restore a wall from a JSON backup.

No server or build step is required.

GitHub Pages

To publish the wall with GitHub Pages:





Rename stockholm_innovation_lab_testimony_wall.html to index.html, or configure the Pages entry point to use the existing filename.



Push the file to the repository's selected branch.



Enable GitHub Pages in the repository settings.



Open the generated Pages URL.

Saving and importing data

The wall uses two storage options:





Browser storage: Save state stores the current wall in localStorage for the current browser.



JSON file: Save to file downloads stockholm-innovation-lab-testimonies.json, which can be archived or shared.

Importing a file replaces the current wall with the testimonies contained in that file. The import flow validates the structure and ignores invalid testimony entries.

Example JSON structure:

{
  "app": "Stockholm Innovation Lab Testimony Wall",
  "version": 1,
  "savedAt": "2026-01-01T12:00:00.000Z",
  "testimonies": [
    {
      "id": "career-ai-cybersecurity",
      "tag": "Punch line",
      "text": "More than an internship, a launchpad for my career in AI and cybersecurity.",
      "color": "blue",
      "tilt": -1.2
    }
  ]
}

Project structure

.
├── index.html
└── README.md

If you keep the original filename, replace index.html in the structure above with stockholm_innovation_lab_testimony_wall.html.

Browser support

The wall uses modern browser features including localStorage, FileReader, Blob, and URL.createObjectURL. Use a current version of Chrome, Edge, Firefox, or Safari.

Privacy

Testimonies are stored locally in the browser and are only exported when the user chooses Save to file. This project does not include a backend or external data service.

License

No license is included yet. Add a license file before distributing the project publicly.
