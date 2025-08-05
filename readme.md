
This repository contains the frontend code for a multi-page educational website, "CodeWithHarry," designed to offer tutorials, courses, blogs, and notes on various programming technologies. The project features a responsive design, a dynamic navigation bar, and interactive elements.

✨ Features
Responsive Navbar: A fully responsive navigation bar that adapts to different screen sizes, including a mobile menu toggle.

Multi-Page Structure: Separate dedicated pages for:

Home (index.html): Main landing page with hero section, technology carousel, features, testimonials, and trusted stats.

Courses (courses.html): Displays various programming courses with details.

Tutorials (tutorials-full.html): Lists comprehensive programming tutorials.

Blog (blogs.html): Features articles and blog posts on tech topics.

Notes (notes.html): Provides concise summaries and quick references.

Contact Us (contact.html): A page with contact information and a message form.

Theme Toggle: A dark/light mode switcher that persists user preference using localStorage.

Search Modal: An overlay search interface (triggered by Ctrl+K or search icon) with category filtering.

Simulated Authentication: Basic login and signup functionality using localStorage to simulate user sessions. Upon successful login, the "Login" and "Signup" buttons are replaced by a "Profile" button displaying the username and a "Logout" button.

🚀 Technologies Used
HTML5: For structuring the web content.

CSS3: For styling, primarily utilizing:

Tailwind CSS: A utility-first CSS framework for rapid UI development.

Custom CSS: Additional styles for specific components and overrides.

JavaScript (ES6+): For interactive elements, dynamic content, and client-side logic, including:

DOM Manipulation: Handling element visibility and content changes.

Event Listeners: Managing user interactions.

localStorage: For persisting theme preferences and simulating user authentication.

Fetch API (Placeholder): The code includes placeholders for fetch API calls, demonstrating where backend integration would occur if implemented.

📁 Project Structure
.
├── index.html
├── courses.html
├── tutorials-full.html
├── blogs.html
├── notes.html
├── contact.html
└── README.md

🛠️ Setup and Running Locally
This project is a frontend-only application. You do not need a web server (like Apache or Nginx) or a backend language (like PHP) to run it, as all authentication and data persistence are simulated using localStorage directly in the browser.

Clone the repository (or download the files):

git clone <repository-url>
cd <project-folder>

(Replace <repository-url> and <project-folder> with your actual project details if applicable).

Open the HTML files:
Simply open any of the .html files (e.g., index.html, contact.html) directly in your web browser. All linked CSS and JavaScript will load automatically.

index.html is the homepage.

Navigate between pages using the navbar links.

🔑 Authentication Simulation
The login and signup functionality is simulated using your browser's localStorage.

Signup: When you sign up, your chosen username and password (unhashed for this frontend-only simulation) are stored in your browser's localStorage under the key users.

Login: When you log in, the provided credentials are checked against the users data in localStorage. If they match, a isLoggedIn flag and your username are stored in localStorage, and the navbar UI updates.

Logout: Clears the isLoggedIn flag and username from localStorage, reverting the navbar to its default state.

Note: This localStorage based authentication is not secure for real-world applications. It is purely for demonstration purposes within this frontend-only project. For a production application, a secure backend with proper database and session management is essential.