E-oxu - Static Book Platform
Overview
E-oxu is a simple, static website designed to showcase a collection of books, primarily focusing on Azerbaijani literature and translated international works. Built with HTML, Tailwind CSS, and vanilla JavaScript, it serves as a digital platform to browse book details and contact the site administrators. The project is intentionally lightweight, with no backend or database, making it easy to deploy and maintain.
Features

Book Details Page: Displays information about individual books (title, author, genre, image, and description) fetched from a static books.json file. Accessible via URL query parameters (e.g., index.html?id=1).
Contact Form: Includes a mock contact form with a "Message Sent" modal for user feedback (no actual submission occurs).
Responsive Design: Built with Tailwind CSS for a modern, mobile-friendly interface with a blue-orange color scheme.
Static Content: All data is stored in a books.json file, and no server-side processing is required.
Navigation: Simple navbar and footer with links to Home, Books, About, and Contact pages (some pages are placeholders).

Project Structure
e-oxu/
├── index.html          # Book details page (fetches book data from books.json)
├── contact-us.html     # Contact page with mock form and modal
├── books.json          # Static JSON file containing book data (id, title, author, genre, image, description)
└── README.md           # Project documentation

Setup Instructions

Clone or Download:
Clone the repository or download the project files to your local machine.


Serve the Website:
Use a local web server (e.g., VS Code Live Server, http-server, or Python’s python -m http.server) to serve the files.
Direct file access (file://) may not work for fetching books.json due to browser security restrictions.


Access the Site:
Open the site in a browser (e.g., http://localhost:3000/index.html?id=1 to view a book).
Navigate to contact-us.html to test the contact form.


Dependencies:
No external dependencies are required except for Tailwind CSS, which is included via CDN (https://cdn.tailwindcss.com).
Ensure an internet connection for the Tailwind CDN to load styles.



Usage

Book Details: Visit index.html?id=<id> (e.g., id=1 to id=10) to view details of a specific book from books.json. If an invalid id is provided, the page redirects to index.html.
Contact Form: On contact-us.html, fill out the form and click "Göndər" to see a mock "Message Sent" modal. No data is sent; the modal is for visual feedback.
Customization: Edit books.json to add or modify book entries. Ensure each book has an id, title, author, genre, image, and description.

Technologies Used

HTML: Structure of the website.
Tailwind CSS: Styling and responsive design.
JavaScript: Client-side logic for fetching books.json and handling the contact form modal.
JSON: Static data storage for book information.

Limitations

Static Nature: No backend or database; all data is hardcoded in books.json.
Mock Contact Form: The contact form does not send data to a server; it only shows a modal.
Placeholder Pages: Links to "Əsas Səhifə," "Kitablar," and "Haqqında" are placeholders and require additional pages (e.g., a homepage with a book grid).
Image Dependency: Book images are sourced from qanun.az and require an internet connection to load.

Future Improvements

Add a homepage (index.html) with a grid of books linking to individual detail pages.
Implement actual form submission for the contact page using a backend service (e.g., Formspree or Node.js).
Include form validation to ensure required fields are filled before showing the modal.
Create additional pages (about.html, homepage) to complete the navigation.
Host images locally to avoid reliance on external URLs.

Contributing
Feel free to fork the project, make improvements, and submit pull requests. Suggestions for additional features, bug fixes, or design enhancements are welcome.
License
This project is open-source and available under the MIT License. 
Contact
For questions or feedback, reach out via the mock contact form on contact-us.html (just kidding—it’s static!). Alternatively, contact the project maintainers at info@eoxu.az (placeholder email).

Built with 📚 and ☕ by the E-oxu team.
