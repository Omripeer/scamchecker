בודק אתרים - Hebrew Phishing & Scam Website Checker
A simple, user-friendly, and free web application designed to help users, especially older adults, check if a website is potentially a phishing or scam site. The interface is in Hebrew and built for maximum clarity and ease of use.
➡️ Live Demo Link (Replace this with your actual GitHub Pages URL after deploying!)
🌟 Project Purpose
The internet can be a dangerous place, with many fraudulent websites trying to trick people into giving away personal information. This tool was created to provide a quick and easy first line of defense. Users can paste a suspicious URL, and the app will check it against Google's extensive database of unsafe websites, providing a clear, color-coded answer about its safety.
The project is designed with accessibility in mind, featuring large text, high-contrast colors, and a simple, single-purpose interface.
✨ Features
 * 🛡️ Real-time Safety Check: Utilizes the Google Safe Browsing API to check URLs against known malware, phishing, and unwanted software threats.
 * 📈 Top 10 Searched Sites: A live-updating list of the most frequently checked URLs by all users of the app, powered by Firebase Firestore. This helps identify currently trending suspicious sites.
 * 🔢 Visitor Counter: A simple client-side counter to show community engagement.
 * 👴 User-Friendly Design: A clean, responsive, and accessible interface built with Tailwind CSS, specifically designed for users who may not be tech-savvy.
 * 🌐 Fully Self-Contained: The entire application runs from a single index.html file, making it incredibly easy to deploy.
🛠️ Technology Stack
 * Frontend: HTML, Tailwind CSS
 * Backend & Database: Firebase (for Firestore DB and Anonymous Authentication)
 * APIs: Google Safe Browsing API V4
🚀 How to Set Up and Deploy
This project is very easy to set up. Follow these steps:
 * Clone or download the repository. All you need is the index.html file.
 * Get a Google Safe Browsing API Key:
   * Go to the Google Cloud Console.
   * Create a new project and enable the Safe Browsing API.
   * Create an API Key in the "Credentials" section.
 * Add Your API Key:
   * Open the index.html file in a text editor.
   * Find the line const apiKey = 'AIzaSy...'; inside the <script> tag.
   * Replace the existing key with your own API key.
 * Set up Firebase (Optional but Recommended):
   * The code is pre-configured to work with a Firebase backend for the "Top 10 Searches" feature.
   * For this to work in your own deployment, you would need to create a free project on Firebase and replace the firebaseConfig and appId variables in the code.
 * Deploy for Free:
   * GitHub Pages: Upload the index.html file to a public GitHub repository and enable GitHub Pages in the repository settings.
   * Netlify: Simply drag and drop the index.html file into the Netlify dashboard.
‼️ IMPORTANT SECURITY NOTE
Your Google API key is included in the frontend code. To prevent others from misusing it, you must restrict it.
In your Google Cloud Console, under Credentials, edit your API key and add "HTTP referrers (web sites)" restrictions. Add the URL of your deployed website (e.g., https://your-username.github.io/*). This ensures the key will only work on your site.
🤝 Contributing & Feedback
This is a free tool for the community. If you have suggestions for improvement or find any bugs, please feel free to open an issue in this repository.
