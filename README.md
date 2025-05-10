# Gen AI Bistro Cafe Assistant
*A Smart Conversational AI Solution for Cafe Service Automation*

## 📖 About the Project

Gen AI Bistro Cafe Assistant is a virtual AI chatbot built using IBM Watson Assistant,
designed to automate customer interactions in a café setting. It simulates real-world
ordering, FAQs, and navigation using natural language conversation.

This project was created to enhance user experience, reduce staff load, and demonstrate
the power of conversational AI in hospitality environments.

## Key Features

- Guided conversation with user-friendly flow
- Drink and food menu display on demand
- Slot-filling for order details (drink type, size, sweetener)
- Location and timing FAQs
- Easy web deployment via IBM Web Chat
- Python launcher for simplified access

## 📁 Project Structure

```bash
Gen-AI-Bistro-Cafe-Assistant/
├── Bistro.html                 # Webpage with Watson Web Chat embed
├── run_chatbot.py            # Python script to auto-open the HTML in browser
├── workspace.json            # Exported Watson Assistant skill
├── README.md                 # Project documentation
└── LICENSE                   # Project license
```

## ▶️ How to Run the Project

### Step 1: Clone the Repository
```bash
$ git clone https://github.com/yourusername/gen-ai-bistro-cafe-assistant.git
$ cd gen-ai-bistro-cafe-assistant
```

### Step 2: Launch the Chatbot Interface

#### Option A – Static Web View
- Open `index.html` in any modern browser.
- This will load the chatbot using the embedded Watson Web Chat.

#### Option B – Python Launcher (Windows only)
- Ensure Python 3.x is installed.
- Run the following to open the bot in your default browser:
```bash
$ python run_chatbot.py
```

### Step 3: Import and Customize Watson Assistant

1. Go to [IBM Cloud](https://cloud.ibm.com/) and sign in or create a free Lite account.
2. Launch **Watson Assistant** from your IBM Cloud dashboard.
3. Create a new Assistant instance if you don't have one.
4. Go to `Skills` → Click `Upload / Download` → Choose `Upload Skill`.
5. Select the provided `workspace.json` file from this project.
6. The skill will now include:
   - Predefined intents (e.g., `#order_drink`, `#view_menu`)
   - Entities (e.g., `@drinks`, `@sizes`, `@food_items`)
   - Dialog nodes and slot-based logic

💡 **Note:**
Each user must import the workspace into **their own IBM Cloud account**.  
The chatbot runs independently in your personal Watson Assistant instance.  
This project does **not** give others access to your dashboard or credentials.

### Step 4: (Optional) Update Integration Settings

- If you generate a new integration in Watson Assistant:
  - Copy the new `integrationID`, `region`, and `serviceInstanceID`
  - Replace them in the `index.html` file where the Watson embed script is configured


## 🚀 Future Enhancements

- Voice input and speech-to-text interaction
- Integration with backend databases (for orders)
- Personalized suggestions using Watsonx.ai
- Multilingual support
- WhatsApp / Messenger deployment


