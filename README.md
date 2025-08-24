<img width="830" height="658" alt="Screenshot 2025-08-24 025012" src="https://github.com/user-attachments/assets/c924c1c2-14f4-453a-82f3-976c63db41ce" />
<img width="370" height="200" alt="Screenshot 2025-08-24 025028" src="https://github.com/user-attachments/assets/1b249b1c-764f-418c-b89a-ca62ea8ac850" />
<img width="569" height="254" alt="Screenshot 2025-08-24 025345" src="https://github.com/user-attachments/assets/bab46053-d10d-428c-a101-18b197e7d58e" />

An intelligent Telegram bot that automatically tracks your expenses by adding them to Google Sheets. Simply send a message or voice note with item details, and Yaso AI will organize everything in your spreadsheet with proper categorization.

✨ Features
Feature	Description
💬 Text Message Processing	Understands natural language input for expense tracking
🎤 Voice Message Support	Processes voice messages and converts them to expense entries
📊 Google Sheets Integration	Automatically updates your spreadsheet with new expenses
🏷️ Smart Categorization	Automatically categorizes items based on your spending patterns
📱 Telegram Bot Interface	Easy-to-use interface through familiar Telegram messaging
🌐 Multi-language Support	Handles both English and Arabic content seamlessly

📋 Requirements
n8n Instance (self-hosted or n8n.cloud)

Telegram Bot Token (Create via @BotFather)

Google Service Account (For Sheets API access)

Google Sheets Document (Your expense tracker template)

🛠️ Setup Guide
1. Create Your Telegram Bot
Message @BotFather on Telegram

Use /newbot command to create your bot

Save the API token provided

2. Prepare Google Sheets
Create a new Google Sheet with columns: Item, Amount, Store, Date

Share the sheet with your service account email

Note the Sheet ID from the URL

3. Configure n8n Workflow
1- Import the workflow JSON into your n8n instance

2- Set up credentials:

3- Telegram Bot API token

4- Google Service Account credentials

5- Configure nodes with your Sheet ID and range

4. Deploy the Bot
   
1- Activate the workflow in n8n

2- Start chatting with your bot on Telegram

3- Test with sample messages: "iPhone 1500 on 2024-05-09"

💬 Usage Examples
Text Message:
TV 5000 Amazon 2024-05-14
Voice Message:
"Bought a PlayStation for 1000 from GameStop today"
Bot Response:

text
✅ Added successfully!
Item: PlayStation
Amount: 1000
Store: GameStop
Date: 2024-05-16
