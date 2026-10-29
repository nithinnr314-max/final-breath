Breathe IQ — authentication and profile data fix

Files:
- index.html: original website structure and design; Tailwind configuration is embedded to keep the package to HTML/CSS/JavaScript files.
- style.css: original custom CSS, unchanged.
- script.js: original app logic with localStorage registration/login/profile fixes.

Registration:
1. Name
2. Username
3. Email ID
4. Password
5. Confirm password

Rules:
- Email IDs are normalized (trimmed and case-insensitive) and cannot be registered twice.
- Usernames are normalized and cannot be duplicated.
- Password and confirm password must match; password must be at least 6 characters.
- Sign-in uses the same email ID and password saved during registration.
- User profile edits are saved to localStorage and loaded again on the next sign-in.

Run:
1. Extract the ZIP.
2. Open the folder in VS Code.
3. Open index.html with Live Server, or open index.html in a browser.
4. Registration data remains in the same browser and origin's localStorage.

Important security note:
This is a front-end demonstration. localStorage is browser-local and is not secure authentication; passwords are stored in the browser and can be read by someone with access to the device. Do not use real/reused passwords. A production app needs a backend and password hashing.
