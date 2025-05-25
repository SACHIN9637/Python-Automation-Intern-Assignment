📊 Event Data Cleaner & Personalized Messaging Bot

A Python-based automation project that processes participant data from events, generates personalized messages based on engagement, and optionally sends them using Email or Telegram.

---

🚀 Features

✅ Step 1: Data Cleaning
- Removes duplicate email entries.
- Normalizes `has_joined_event` values to `True` / `False`.
- Flags rows with:
  - Missing or incomplete LinkedIn profiles.
  - Blank job titles.
- Saves the cleaned data to `cleaned_output.csv`.

✉️ Step 2: Personalized Messaging
- Customizes messages based on:
  - Event participation (joined or not)
  - Name
  - Job title
  - LinkedIn profile presence
- Outputs:
  - `messages_output.csv` (columns: email, message)
  - Individual `.txt` files per message (optional)

🧪 Step 3: Optional Automation (Bonus)
- Send messages via Gmail SMTP.
- OR push messages into a Telegram bot queue.

---

📁 Folder Structure

.
├── clean_data.py              # Cleans raw Excel/CSV data
├── cleaned_output.csv         # Cleaned participant data
├── generate_messages.py       # Personalized message generation
├── messages_output.csv        # Output file with messages
├── messages_txt/              # Optional: Individual message text files
├── send_emails_smtp.py        # Optional: Email automation using SMTP
├── send_to_telegram.py        # Optional: Telegram bot integration
└── README.md                  # Project documentation

---

🛠️ Tech Stack

- Python 3.x
- pandas
- openpyxl
- smtplib (for email automation)
- Telegram Bot API (for Telegram integration)

---

📦 Installation

Install the required Python libraries using:

pip install pandas openpyxl

💡 For email automation, configure your Gmail SMTP or use a dummy SMTP server.

---

📌 Usage

1. Clean the data
   Run the following script to clean your raw dataset:

   python clean_data.py

2. Generate messages
   Create personalized messages based on the cleaned data:

   python generate_messages.py

3. Send messages (optional)
   Send messages via email or Telegram:

   - Using SMTP:

     python send_emails_smtp.py

   - Using Telegram Bot:

     python send_to_telegram.py

---

👤 Author

Sachin Ganesh Jadhav
🎓 TY B.Tech CSE @ MITAOE, Pune
🔗 LinkedIn: https://www.linkedin.com/in/sachin-jadhav9637

---

📄 License

This project is intended for learning and demonstration purposes only.
