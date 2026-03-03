                                      🚀 AutoPayNews: Python to LinkedIn Automation

💡 About This Script
_________________

What it is: A fully automated Python script that finds the latest news about electronic payments, uses AI to write a professional summary, and posts it directly to LinkedIn with a relevant image.

Why I built it: As an e-payment monitoring engineer, staying updated on fintech, scheme rules, and transaction technology is crucial. I wanted a hands-off way to curate and share industry insights without having to manually draft posts every day.

⚙️ How It Works (The Pipeline)
________________________________

Step 1: Python Scraper 🐍: The script searches for the latest articles on electronic payments and fintech.

Step 2: AI Processing 🧠: It sends the article to the Google Gemini API, which rewrites it into an educational, engaging LinkedIn post under 3,000 characters.

Step 3: Image Selection 🖼️: The script automatically selects a high-quality, royalty-free image (like a POS terminal or digital banking app) from Unsplash to avoid AI-generator bot blocks.

Step 4: The Webhook 🪝: Python packages the text and the image link and fires it to a Make.com webhook.

Step 5: Publishing 📲: Make.com catches the payload, downloads the image, and pushes the final post live to LinkedIn via their API.

🛠️ What You Need to Run This
_____________________________

If you want to clone this and run it yourself, you will need:

Python installed (or just use Google Colab).

A free Google Gemini API Key.

A free Make.com account.

Your LinkedIn account connected to Make.com.

🏗️ Setup Instructions
_______________________


The Code: Clone this repository and open the Python script.

The Keys: Paste your Gemini API key into the GOOGLE_AI_KEY variable.

The Webhook: Create a new scenario in Make.com with a "Custom Webhook". Copy that URL and paste it into the WEBHOOK_URL variable in the script.

Make.com Modules: Connect your Webhook to an "HTTP - Download a file" module (to grab the Unsplash image), and connect that to a "LinkedIn - Create an Image Post" module.

▶️ Running the Script
_______________________

Simply hit run on the Python file. It will fetch the news, generate the post, send it to Make.com, and print a success message in the terminal when it's done!

<img width="2816" height="1536" alt="Gemini_Generated_Image_r2sr11r2sr11r2sr" src="https://github.com/user-attachments/assets/bbacc42b-f1a5-4900-b199-6f647cadbed4" />
