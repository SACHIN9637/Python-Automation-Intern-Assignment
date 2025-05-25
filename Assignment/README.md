# 📊 Event Data Cleaner & Personalized Messaging Bot

A Python-based automation project that processes participant data from events, generates personalized messages based on engagement, and optionally sends them using email or Telegram.

---

## 🚀 Features

### ✅ Step 1: Data Cleaning
- Removes duplicate email entries.
- Normalizes `has_joined_event` values to `True/False`.
- Flags rows with:
  - Missing or incomplete LinkedIn profiles.
  - Blank job titles.
- Saves the cleaned data to `cleaned_output.csv`.

### ✉️ Step 2: Personalized Messaging
- Customizes messages based on:
  - Event participation (joined or not)
  - Name
  - Job title
  - Presence/absence of LinkedIn profile
- Outputs:
  - `messages_output.csv` (email, message)
  - Individual message `.txt` files (optional)

### 🧪 Step 3: Optional Automation (Bonus)
- Send emails using SMTP (e.g., Gmail).
- OR Push messages to a Telegram bot queue.

---

## 📁 Folder Structure
```plaintext
├── clean_data.py # Cleans raw Excel data
├── cleaned_output.csv # Cleaned participant data
├── generate_messages.py # Personalized message generation
├── messages_output.csv # Final message CSV
├── messages_txt/ # Individual messages (optional)
├── send_emails_smtp.py # Email automation via SMTP (optional)
├── send_to_telegram.py # Telegram bot integration (optional)
└── README.md
```

---

## 🛠️ Tech Stack

- Python 3.x
- pandas
- openpyxl
- smtplib (for email)
- Telegram Bot API (optional)

---

## 📌 Usage
Run clean_data.py to clean your raw data (Data.xlsx).

Run generate_messages.py to generate customized messages.

Optionally, run send_emails_smtp.py or send_to_telegram.py to dispatch messages.

---

##👤 Author

Sachin Ganesh Jadhav

🎓 TY B.Tech CSE @ MITAOE, Pune

🔗 LinkedIn: https://www.linkedin.com/in/sachin-jadhav9637

