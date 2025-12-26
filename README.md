🛡️ YSENTRY: Phishing Website Detection System
"Empowering Digital Safety through Intelligent Machine Learning Analysis"

📚 Table of Contents
🌟 Overview

🚀 Getting Started

🛠️ Required Libraries & Stack

💻 Project Execution Commands

🧠 Model Logic & Technical Explanation

⚙️ How It Works (Workflow)

✨ Future Enhancements

👨‍💻 Author

🌟 Overview <a name="overview"></a>
Digital security is a growing concern as phishing attacks become more sophisticated. YSENTRY is a specialized tool designed to detect malicious URLs before they can cause harm.

Intelligent Analysis: Unlike basic filters, YSentry uses Machine Learning to understand the structural patterns of a URL.

User-Centric Design: Built with a clean Flask interface, making it accessible for non-technical users to verify links.

Speed & Reliability: The system provides results in milliseconds, ensuring no delay in your browsing experience.

Activity Intelligence: Automatically tracks the last 21 ⚡ scans, allowing users to review their history and stay informed about potential threats.

🚀 Getting Started <a name="getting-started"></a>
To set up YSentry on your local environment, follow this detailed procedure:

Repository Cloning: Use the command git clone followed by the URL to download all project files, including the pre-trained model and web templates.

Directory Navigation: Move into the project folder using the cd command to access the application's root directory.

Environment Isolation: Create and activate a Virtual Environment (.venv) to prevent library conflicts with your global Python installation.

Dependency Sync: Run the installer to download specific versions of libraries like Flask and Scikit-learn required for the model to function.

🛠️ Required Libraries & Stack <a name="required-libraries"></a>
The project utilizes a robust stack of technologies to ensure accuracy and stability:

🐍 Python 3.13+: The core engine used for data processing and model inference.

🔥 Flask Framework: Acts as the bridge between the ML model and the user interface, handling all web requests.

📊 Scikit-learn: The primary ML library used to load the Multinomial Naive Bayes model and perform classification.

🧪 Pandas & NumPy: Used for handling the URL data as numerical arrays during the prediction phase.

🌐 Requests: Facilitates the real-time checking of URL headers and SSL certificates.

💻 Project Execution Commands <a name="project-commands"></a>
Execute these steps in your terminal to bring the system online:

Bash

# 1. Activate the environment to use local dependencies
.\.venv\Scripts\activate

# 2. Install the necessary stack from requirements.txt
pip install -r requirements.txt

# 3. Start the Flask server on your local machine
python app.py
After execution, the terminal will provide a local link (typically http://127.0.0.1:5000) to access the dashboard.

🧠 Model Logic & Technical Explanation <a name="logic"></a>
The "Brain" of YSENTRY is based on high-performance text classification logic:

Algorithm: Multinomial Naive Bayes was chosen for its high efficiency in classifying discrete features like characters and symbols in a URL string.

Feature Extraction: The system performs "Lexical Analysis," extracting features such as URL length, the count of special characters (e.g., @, ?, -), and domain-specific markers.

Vectorization: Raw URLs are converted into numerical form using a vectorizer.pkl. This allows the AI to calculate the statistical probability of a link being malicious based on its training.

Accuracy: The model was trained on 21,000+ samples, achieving a verified 96.4% Accuracy rate, making it highly reliable for daily use.

⚙️ How It Works (Workflow) <a name="how-it-works"></a>
The YSentry workflow is designed for transparency and speed:

Input Phase: The user pastes a URL into the dashboard's input field.

Analysis Phase: The backend script cleans the input and passes it through the Lexical Engine and the ML Classifier.

Verification Phase: Simultaneous checks are performed to see if the site has a valid SSL certificate or is present on known blacklists.

Result Phase: The UI updates instantly, showing a "MALICIOUS" (Red) or "SAFE" (Green) badge based on the model's prediction.

Logging Phase: The scan is added to the history log, ensuring the user can refer back to their previous 21 ⚡ scans.

✨ Future Enhancements <a name="future"></a>
We are committed to evolving YSentry into a complete security suite:

🌐 Browser Integration: Developing a Chrome/Edge extension for automatic, "click-less" protection while browsing.

🤖 Deep Learning Transition: Implementing LSTM (Long Short-Term Memory) models to detect even more complex and evolving phishing patterns.

📲 Mobile Security: Creating an API that can be used by mobile apps to scan links within SMS or messaging platforms.

🛡️ Global Threat Intelligence: Connecting the engine to live databases for even more robust verification.

👨‍💻 Author <a name="author"></a>
Yasir Ali | IT Enthusiast 🚀

© 2025 YSENTRY | Committed to Digital Safety and ML Innovation

I am a developer passionate about building tools that solve real-world problems. YSENTRY is part of my journey to bridge the gap between Artificial Intelligence and Cybersecurity. My focus remains on creating accessible, high-performance security software for everyone.

🔗 GitHub Profile | 💼 LinkedIn