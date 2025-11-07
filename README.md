# TRY Literacy Website

A professional, single-page website built with HTML, Tailwind CSS, and JavaScript to showcase the remote remedial instruction services offered by TRY Literacy, LLC. The site focuses on clear information delivery, call-to-actions (contact form), and student portal security.

## 🌟 Features

* **Responsive Design:** Fully optimized for mobile, tablet, and desktop viewing.
* **Clear Structure:** Sections for Mission, Services, Target Grades (3-8), FAQ, and Contact.
* **Tailwind CSS:** Modern, utility-first styling for a clean and professional aesthetic.
* **Contact Form:** Integrated with **Formspree** (or similar service) for lead generation (no phone number required).
* **Student Portal Security:** Simple password-protected access gate for the Google Classroom link, implemented with vanilla JavaScript.

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need a modern web browser to view the HTML file. No local build tools are required as all dependencies are loaded via CDN (Content Delivery Network).

### Installation

1.  **Clone the Repository (or Download):**
    ```bash
    git clone [YOUR-REPO-URL-HERE]
    ```
2.  **Open the File:**
    Locate the `index.html` file in the project folder and open it directly in your web browser (e.g., Chrome, Firefox).

## 🛠️ Configuration and Customization

The core of the website is contained within the `index.html` file. To customize the site, you need to update the following critical sections within the `<script>` and `<form>` tags.

### 1. Update Contact Form Endpoint

The contact form uses a service like Formspree to send emails without server-side code.

* **File:** `index.html`
* **Section:** ``
* **Action:** Update the `action` attribute in the `<form>` tag:
    ```html
    <form action="REPLACE_WITH_YOUR_FORMSPREE_ENDPOINT" method="post" class="space-y-4">
    ```

### 2. Update Student Portal Password

The student portal access uses a simple JavaScript password gate.

* **File:** `index.html`
* **Section:** `<script>` tag at the bottom of the body.
* **Variables to Change:**
    ```javascript
    // The URL is correct:
    const CLASSROOM_URL = "REPLACE_WITH_YOUR_GOOGLE_CLASSROOM_INVITE_LINK"; 

    // CRITICAL: REPLACE "Literacy030608" with your desired password
    const CORRECT_PASSWORD = "REPLACE_WITH_YOUR_NEW_PASSWORD"; 
    ```

### 3. Change Business Contact Information

Ensure your publicly listed contact information is current. (Note: The phone number was intentionally removed per request.)

* **File:** `index.html`
* **Section:** ``
* **Email:** Update the text within the email `<span>`:
    ```html
    <span class="font-medium">REPLACE_WITH_YOUR_BUSINESS_EMAIL</span>
    ```

## 🔗 Built With

* **HTML5** - The web standard for structure.
* **Tailwind CSS** - CSS utility framework for styling and layout. (Loaded via CDN)
* **Lucide Icons** - Simple, clean open-source icon set. (Loaded via CDN)
* **JavaScript (Vanilla)** - Used for mobile menu toggling, FAQ accordion, and the password gate logic.

## ✍️ Author

* **[Your Name / Business Name]** - Initial Work - [Link to your professional page, if applicable]

## 📝 License

This project is open source and available under the [License Name] License. (e.g., MIT License)