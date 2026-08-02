🎓 TUP Computer Studies: Thesis & Capstone Roadmap

A fully responsive, interactive single-page web application serving as the centralized digital handbook for the Technological University of the Philippines (TUP) - Manila, Computer Studies Department.

📖 Overview

The TUP Thesis & Capstone Roadmap is designed to guide BSIS, BSCS, and BSIT students through the complex, multi-phase process of completing their academic requirements. Instead of relying on static PDFs or scattered documents, this application provides a chronological, step-by-step breakdown of every phase, complete with assigned actors, critical deadlines, and documentation formats.

✨ Key Features

Interactive Phase Navigation: Seamlessly toggle between five distinct academic phases (Topic Defense, Proposal, Final Defense, Post-Defense, and Submission Guidelines).

Analytics Dashboard: Visual insights using Chart.js to track task volume and monitor critical quality thresholds (e.g., Similarity and AI writing indexes).

Built-in Document Viewer: A custom HTML/CSS modal allows students to preview required physical document formats (Cover Pages, Approval Sheets) directly within the app.

Mobile-First Design: Features a sticky desktop sidebar that transforms into an intuitive, app-like bottom navigation bar on mobile devices.

Zero Dependencies: Built entirely with pure vanilla HTML, CSS, and JavaScript. No build steps, bundlers, or heavy frameworks required!

📑 Table of Contents

Overview

Project Structure

Local Development & Setup

Deployment (GitHub Pages)

Customizing the Content

License

📂 Project Structure

Because this project prioritizes simplicity and easy deployment, the entire application is contained within a single index.html file.

tup-thesis-roadmap/
├── index.html           # The main application (HTML, CSS, JS)
├── README.md            # Project documentation
└── assets/              # Directory for all local images
    ├── cos_logo.png
    ├── tup_logo.png
    ├── ched_logo.png
    ├── cover-page.jpg
    ├── approval-sheet.jpg
    └── table-of-contents.jpg


🚀 Local Development & Setup

You can run this project locally in seconds without installing Node.js, NPM, or any backend servers.

Clone the repository:

git clone https://github.com/your-username/tup-thesis-roadmap.git
cd tup-thesis-roadmap


Add your assets:
Create an assets/ folder in the root directory and add your required images (ensure the filenames exactly match those listed in the Project Structure above).

Run the application:

Using VS Code: Open the project folder, right-click index.html, and select "Open with Live Server" (requires the Live Server extension).

Using a browser: Simply double-click index.html to open it directly in Chrome, Firefox, or Safari.

🌐 Deployment (GitHub Pages)

This project is perfectly optimized for free, instant hosting via GitHub Pages.

Push your code (including the assets/ folder) to a public GitHub repository.

Navigate to your repository on GitHub.

Click on Settings > Pages (on the left sidebar).

Under Build and deployment, set the Source to Deploy from a branch.

Under Branch, select main (or master) and / (root).

Click Save.

Within 1-2 minutes, your interactive roadmap will be live and accessible globally!

🛠️ Customizing the Content

All the text, steps, and phase data are stored in a simple JavaScript object inside index.html. You do not need to edit complex HTML to update the steps!

To add or modify a step, scroll down to the <script> section and locate the phaseData object:

const phaseData = {
    // ...
    proposal: {
        id: 'proposal',
        label: '2. Proposal Defense',
        icon: 'fa-file-lines',
        intro: 'Description of the phase...',
        steps: [
            // Simply edit the title, actor, or desc here!
            { 
                title: "Adviser Selection", 
                actor: "Teacher / Dept. Head", 
                desc: "Selection based on expertise..." 
            },
        ]
    }
}


📜 License

This project is created for the Technological University of the Philippines (TUP) - Manila. Feel free to fork, modify, and use this template for your own academic or departmental needs.
