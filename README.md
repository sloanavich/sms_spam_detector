# sms_spam_detectorSMS Spam Classifier

This project is a machine learning application that classifies SMS text messages as spam or not spam (ham) using a TF-IDF vectorizer and a Linear Support Vector Classifier (LinearSVC). The app is built with Python and deployed through a Gradio interface.

⸻

Files Included
	•	gradio_sms_text_classification.ipynb — Main notebook where the app is built and run.
	•	sms_text_classification_solution.ipynb — Starter code with a full reference implementation.
	•	SMSSpamCollection.csv — The dataset containing labeled SMS messages (spam/ham).

⸻

Technologies Used
	•	Python
	•	Pandas for data handling
	•	Scikit-learn for machine learning and text vectorization
	•	Gradio for building an interactive web interface

⸻

How It Works
	1.	The app loads and cleans the SMS dataset.
	2.	It uses a machine learning pipeline with TfidfVectorizer and LinearSVC.
	3.	A function sms_classification() trains the model.
	4.	A second function sms_prediction() classifies new input text.
	5.	A Gradio interface collects input from the user and displays the prediction result.

⸻

Example Messages to Test

You can try entering the following messages in the Gradio app:
	•	"You are a lucky winner of $5000!" → spam
	•	"Thanks for registering. Text 4343 to receive free updates on medicare." → spam
	•	"Hey! Want to grab lunch today?" → not spam

⸻

How to Run It Locally
	1.	Clone the repo or open the notebook in your Python environment.
	2.	Install dependencies:

    pip install gradio pandas scikit-learn

    3.	Run all cells in gradio_sms_text_classification.ipynb.
	4.	The Gradio app will launch in your browser.

⸻

Optional: Share Publicly

To share the app via a public URL, set share=True when launching:

sms_app.launch(share=True)

