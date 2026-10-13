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

__________________________________________________________________-

Photo Gallery

A self-contained, browser-based photo gallery for organizing images into date-based sections.

The gallery runs entirely in the browser and does not require a backend, build process, or installation.

Features





Upload multiple images by clicking the upload area or dragging files onto it.



Automatically read year and month from JPEG EXIF metadata.



Group images by year or by year and month.



Sort sections from oldest to newest or newest to oldest.



Rename section titles, for example changing 2024 to Summer Holiday.



Manually assign or change an image's year and month.



Drag images between date sections.



Automatically ignore unsupported formats and duplicate inputs.



Open images in a fullscreen viewer with previous/next navigation.



Switch between light and dark mode.



Save a standalone HTML gallery with images embedded directly in the file.



Resize exported images proportionally to a maximum of 600 × 800 pixels.

Supported formats





JPG



JPEG



PNG



GIF



WEBP

Unsupported files are ignored automatically.

Getting started





Place image_gallery.html in your project directory.



Open image_gallery.html in a modern web browser.



Upload your images.



Use the grouping, sorting, editing, and theme controls as needed.

No server or package installation is required.

EXIF dates

For JPEG images, the gallery checks EXIF date fields in this order:





DateTimeOriginal



DateTimeDigitized



DateTime

If no usable EXIF date is found, the image is placed in the No EXIF Date section. Its year or month can be assigned manually.

Duplicate detection

Duplicate uploads are ignored using the file name, file size, and last-modified timestamp. This applies both when selecting multiple files at once and when uploading files later.

Saving a standalone gallery

Click Save as HTML to download a self-contained gallery snapshot.

The exported file:





Embeds images as JPEG data.



Resizes images proportionally to a maximum of 600 × 800 pixels.



Preserves date sections, custom section titles, grouping mode, and theme.



Includes fullscreen viewing and previous/next navigation.



Can be opened offline in a browser.

GitHub Pages

To publish the gallery with GitHub Pages:





Create a GitHub repository.



Add image_gallery.html and this README.md file.



Enable GitHub Pages from the repository's Settings tab.



Open the generated Pages URL.

For the default GitHub Pages entry point, rename image_gallery.html to index.html.

Privacy

Images are processed locally in the browser. They are not uploaded to a server by the gallery.

License

Add the license appropriate for your project, for example MIT, Apache-2.0, or a proprietary license.

License

No license is included yet. Add a license file before distributing the project publicly.
