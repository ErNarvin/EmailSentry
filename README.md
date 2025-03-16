# EmailSentry

Welcome to the EmailSentry tool! This application is my first script project for Cyber securitry tech, designed to demonstrate programming concepts by solving a parctical problem. The tool genrates a unique and meaningful name for each session, verifiles the user via their mobile number, and them manage email account associated with that number. It Provides into email activity, tracks account usage websites application, and allows users to remove unwanted email form the server. When you're done, it says a friendly "bye bye!"

**Note:** This is a demonstration tool using mock data for email analysis and simulated SMS verification.

---

## Features
- **Unique Name Genration:** Create a session ID that is expensive (valuable), beautiful (well-carfted), interactive (user-friendly), and deeply meaningful (unique to your message).
- **User Verification:** Verifies your identity using a simulated mobile number check.
- **Email Count:** Shows how many email accounts are linked to your mobile number.
- **Email Activity Analysis:**
  - **Active Emails:** Emails that send/receive messages 4–5 times a week.
  - **Rarely Used Emails:** Emails with minimal activity (e.g., messages sent/received once a month or less).
- **Account Usage Details:** Select an email to see how many websites or applications it’s registered with and how many of those accounts are unused.
- **Email Removal:** Remove a selected email from the server (simulated for this demo).
- **Friendly Exit:** Displays "Bye bye!" when you close the tool.

---

## Installation

To set up the tool on your machine:

1. **Prerequisites:** Ensure you have python 3.x installed.
2. **Clone the Repositiry:** 
``` bash
git clone https://github.com/ErNarvin/EmailSentry
```  
3. **Navigate to the Directory:**
``` bash
cd EmailSentry
```
4. **Install Dependencies:**
``` bash
pip install -r requirements.txt
```
(Note: Create a requirements.txt file with libraries like requests or sqlite3 if used in your code.)

---

## Usage

Run the tool and follow the interactive prompts:
``` bash
$ python email_manager.py

Welcome to Email Manager!

Generating your unique session name: ElegantHarmony_123

Please enter your mobile number (e.g., +1234567890): +1234567890

Sending verification code... (simulated)

Please enter the verification code: 123456

Verification successful!

Fetching email data for session ElegantHarmony_123...

Emails linked to +1234567890:
1. user@example.com - Active (5 messages/week)
2. olduser@example.com - Rarely used (1 message/month)
3. another@example.com - Active (10 messages/week)

Select an email by number (1-3) or type 'exit' to quit: 1

Details for user@example.com:
- Registered on 5 websites/applications
- 2 accounts are unused

Remove this email from the server? (yes/no): no

Select another email or type 'exit': exit

Thank you for using Email Manager. Bye bye!
```

---

## How It Works

Here’s a breakdown of the tool’s process:

1. **Name Generation:** A unique session ID ***(e.g., ElegantHarmony_123)*** is created using a combination of meaningful words and a random number.
2. **User Verification:** You enter your mobile number, and the tool simulates sending and verifying a code.
3. **Data Retrieval:** The tool queries a mock database to find emails linked to your mobile number.
4. **Analysis:** The tool queries a mock database to find emails linked to your mobile number.
Analysis: Emails are categorized as "Active" (4–5 messages/week) or "Rarely Used" (e.g., 1 message/month) based on mock data.
5. **Detailed View:** Selecting an email shows its usage across websites/apps and identifies unused accounts.
6. **Removal:** You can choose to "remove" an email (simulated deletion from the mock server).
7. **Exit:** The tool closes with a "Bye bye!" message.

---


