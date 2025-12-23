
1. Pre-Requisite![Uploading Screenshot 2025-12-19 093646.png…]()
2. <img width="1892" height="918" alt="Screenshot 2025-12-19 093700" src="https://github.com/user-attachments/assets/822830a6-a067-47f7-a312-721e8812fe65" />
3.<img width="1779" height="890" alt="Screenshot 2025-12-19 093801" src="https://github.com/user-attachments/assets/4646a751-8e30-4d58-ae30-07626281e3a1" />

4.<img width="1904" height="885" alt="Screenshot 2025-12-19 093814" src="https://github.com/user-attachments/assets/6334f919-218c-4fd3-9d1f-e9ced8cc58dd" />

(Software Requirements)
Before running the project, make sure the following software is installed on your system:
1. Node.js (Version 18 or above)
Download and install from: https://nodejs.org
2. MongoDB (Local or Cloud – e.g., MongoDB Atlas)
Download and install from: https://www.mongodb.com
3. npm (comes with Node.js)
4. Code Editor – Visual Studio Code (Recommended)
Download from: https://code.visualstudio.com
5. Internet Connection – Required for Gemini API access.

2.  Login Credentials (for Testing)
This project supports individual user authentication.
Each user can register with their own email and password through the signup feature.
* No default or shared admin credentials are provided.
* All login information is securely stored in the database after registration.
* Passwords are encrypted before being saved.

3. Step-by-Step Installation and Execution Guide
Follow these steps carefully to set up and run the backend server:
Step 1: Copy the Project
Copy the entire VisionMateAI folder to your local system.
Step 2: Set Up Environment File
Inside the backend/ folder, create a new file named .env by copying from .env.example.
Fill in the following environment variables:
MONGO_URI = your_mongodb_connection_string
JWT_SECRET = your_random_secret_key
GEMINI_API_KEY = your_gemini_api_key
Step 3: Install Dependencies
Open a terminal inside the backend/ folder and run:
npm install
This will download and install all the required Node.js dependencies listed in package.json.
Step 4: Run Development Server
To start the backend server, run:
npm run dev
By default, the server will start on:
http://localhost:5000

4. Project Usage Instructions
1. Open your web browser and go to http://localhost:5000.
2. Log in with the default credentials or register a new account (if the feature is available).
3. Explore AI features such as:
o Text generation
o Smart response suggestion
o Summarization or analysis (depending on your implementation)
4. Check the console or terminal for API logs or error messages.
5. To stop the server, press Ctrl + C in the terminal.

5. Important Notes
* Replace placeholder Gemini API URLs in src/services/geminiProxy.ts with the actual Gemini endpoints before deployment.
* Never upload the .env file publicly. It contains secret keys.
* For production deployment:
o Use HTTPS instead of HTTP.
o Use a strong JWT secret.
o Enable proper CORS configuration.
* Make sure MongoDB service is running before starting the server.
* If you get a connection error, verify your MONGO_URI in .env.

		


User manual


