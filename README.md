# Iris-voice-assistant
This Python script is a voice-activated personal assistant, named Iris, that can perform a variety of tasks such as browsing the internet, sending emails, playing YouTube videos, checking battery status, reading the latest news headlines, and controlling basic computer operations like shutdown and restart.
It integrates speech recognition for taking voice commands and text-to-speech (TTS) to respond to the user, providing a hands-free, interactive experience. The assistant can automate web tasks using Selenium, scrape news headlines with BeautifulSoup, and access system features using os and psutil libraries.

✨ Key Features:
🗣 Voice Interaction
Speech Recognition: Listens and recognizes user's voice commands using speech_recognition.

Text-to-Speech: Responds back with voice using pyttsx3 with a selected female voice.

⏰ Greetings Based on Time
Greets the user appropriately depending on the current time of day (morning, afternoon, evening).

🌐 Web Automation and Browsing
Open Facebook: Automatically logs into Facebook with provided credentials.

YouTube Video Player: Searches and plays a video on YouTube based on the user's voice command.

Google Search: Opens Chrome and searches the specified query on Google.

Open StackOverflow: Quickly opens StackOverflow for programming help.

📰 News Headlines Reader
Scrapes news headlines from BBC News (India) and reads them aloud.

🔋 System Monitoring
Battery Status Checker: Checks the battery level and advises when to plug in or unplug the charger based on best practices.

🎵 Media Playback
Play Local Music: Plays music files from a specified folder on the computer.

Custom Notification Sound: Plays a sound upon activation when user says "hello".

📩 Email Sending
Sends emails via Gmail SMTP server after taking the content via voice (though note: credentials are hardcoded, which is unsafe for production).

⏳ System Control
Shutdown or Restart Computer: Shuts down or restarts the PC based on voice confirmation.

🛠 Additional Tools
Opens Visual Studio Code directly via voice command.

⚙️ Libraries and Tools Used:
pyttsx3 for Text-to-Speech (offline TTS engine).

speech_recognition for capturing and interpreting voice commands.

wikipedia for fetching summaries from Wikipedia.

selenium for web automation (Facebook login, YouTube video click, Google search).

requests and BeautifulSoup for web scraping (getting news headlines).

psutil for checking battery status.

playsound for playing notification sounds.

smtplib for sending emails.

Standard libraries: datetime, os, webbrowser, time.

⚠️ Notes for Improvement:
Security: Sensitive data like email credentials are hardcoded. You should encrypt them or use environment variables.

Error Handling: Selenium web elements are directly accessed without proper exception handling — it could break if pages change.

Optimization: The code could be modularized into separate functions or classes for better maintainability.

Voice Command Flexibility: More natural command handling (with NLP) could improve usability.

