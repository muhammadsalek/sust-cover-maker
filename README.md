<div align="center">SUST Cover Maker
A simple, professional way to create university assignment cover pages.
A responsive, browser-based A4 assignment cover generator for students of Shahjalal University of Science and Technology (SUST), Sylhet, Bangladesh.





Designed for academic clarity · Built for everyday student use
</div>Overview
SUST Cover Maker is a lightweight academic utility that lets students create a polished assignment cover page without wrestling with document formatting. Enter the relevant academic details, watch the A4 cover preview update instantly, then download a PDF or print it directly from the browser.

The project emphasizes clean typography, consistent spacing, an accessible form, responsive layout, and client-side processing. It runs from one self-contained HTML application file with no application server, account registration, or build pipeline.
Note: This is an independently developed student utility, not an official SUST website or university-administered service. Use the official university logo only as permitted by the university.

Features
Capability	What it does
Live A4 preview	Reflects form changes on the cover page as they are entered.
Student details	Student name, ID, department, degree, academic year, term, session, and optional batch.
Assignment details	Assignment title and number, course title/code, and submission date.
Instructor details	Teacher's name, designation, department, and optional faculty.
Group assignments	Optional group number, member list, and remarks.
University logo	Lets users select the official logo for display in the header and generated cover.
PDF export	Creates an A4 PDF in the browser using html2canvas and jsPDF.
Print-friendly output	Dedicated print action and A4 print styles.
Field validation	Highlights required information before printing or exporting.
Reset controls	Clears the form after confirmation.
Responsive interface	Adapts the input form and preview layout to desktop and smaller screens.
No server-side form storage	Academic form details are handled in the browser rather than submitted to a backend.


How to use
1. Open the deployed website in a modern browser.
2. Complete the Student Information, Assignment Information, and Course Teacher Information sections.
3. Add any optional group information or remarks.
4. Upload the official SUST logo. The application uses the uploaded image in the header and the cover. On supported browsers, it remembers the logo locally on that device.
5. Check the Live Cover Page Preview for spelling, dates, and alignment.
6. Select Download Cover Page (PDF), or choose Print Cover Page for a print/PDF workflow.
Important: The current implementation requires the logo to be uploaded before PDF export or printing. It is not permanently bundled inside index.html.

Technology stack
- HTML5 — semantic structure and form controls
- CSS3 — responsive layouts, academic styling, and print styles
- Vanilla JavaScript — form interaction, preview rendering, validation, logo handling, and export actions
- html2canvas 1.4.1 — browser-side cover rendering for PDF generation
- jsPDF 2.5.2 — A4 PDF creation
- localStorage — optional device-local storage of the uploaded logo
No React, Node.js, database, server API, or build process is required. The two PDF-generation libraries load from a CDN, so PDF download requires an internet connection unless those dependencies are cached by the browser.
Project structure
sust-cover-maker/
├── index.html     # Complete application: markup, styles, and JavaScript
└── README.md      # Project documentation (this file)
Run locally
1. Download or clone the repository.
2. Open index.html in a modern browser.
3. Enter the assignment information and upload the university logo.
There are no installation commands and no dependencies to install locally. An internet connection is needed to load the PDF libraries from their CDNs.
Deployment
Vercel with GitHub
1. Push index.html to the root of a GitHub repository.
2. In Vercel, choose Add New Project and import the repository.
3. Select the Other framework preset and keep the root directory as ./.
4. Deploy as a static site without a build step.
5. Open the production domain shown in the Vercel dashboard.
Future commits to the connected production branch can trigger automatic deployments.
Netlify or GitHub Pages
Because the site is static, it can also be deployed on Netlify or GitHub Pages. Keep index.html at the deployment root.
Privacy and limitations
- The application does not ask users to create accounts or send their form inputs to a project backend.
- The uploaded university logo can be saved in browser localStorage on the current device; clearing browser storage may remove it.
- PDF generation is performed client-side. Download quality and text rendering can vary by browser and font availability, especially for complex Bengali text. Always inspect the PDF before submission.
- A stable internet connection is needed to retrieve CDN-hosted PDF dependencies on their first load.
- The current application generates assignment cover pages; it is not a university submission or grading portal.
Project goals
This project was created to make routine academic document preparation more efficient while applying practical frontend-development principles: usable forms, live visual feedback, client-side document generation, mobile responsiveness, and straightforward static deployment.
Developer
Developed & Maintained by Md Salek Miah
B.Sc. (Honours) in Statistics
Shahjalal University of Science and Technology (SUST)
Sylhet, Bangladesh

Contact: saleksta@gmail.com
<div align="center">SUST Cover Maker · Built to simplify the first page of every assignment.

Independent academic utility for the SUST student community.
</div>
