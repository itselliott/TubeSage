# TubeSage – Initial Setup & API Key Configuration

## Prerequisites
Before running TubeSage, ensure you have the following installed on your system:
- Python 3.8 or later  
- pip (Python package manager)  

---

## 1️⃣ Clone the Repository
Open a terminal and run:
```bash
git clone https://github.com/yourusername/tubesage.git
cd tubesage
```

---

## 2️⃣ Install Dependencies
Install the required Python libraries:
```bash
pip install -r requirements.txt
```

---

## 3️⃣ Get Your API Keys
### OpenAI API Key (For AI Analysis)
1. Go to OpenAI's API Page: [OpenAI API Keys](https://platform.openai.com/account/api-keys)  
2. Sign in or create an account.  
3. Click “Create API Key” and copy the generated key.  
4. Do not share your key – it is private and linked to your OpenAI account.  

### YouTube API Key (For Video Stats & Transcripts)
1. Go to Google Cloud Console: [Google Cloud Console](https://console.cloud.google.com/)  
2. Create a new project or select an existing one.  
3. Enable the YouTube Data API v3:  
   - Navigate to the **API Library**.  
   - Search for **YouTube Data API v3** and click **Enable**.  
4. Generate an API Key:  
   - Go to **Credentials** > Click **Create Credentials** > Select **API Key**.  
   - Copy the generated key.  

---

## 4️⃣ Store API Keys Securely
You need to set up a `.env` file to store your API keys securely.

1. Create a `.env` file in the root directory:
   ```bash
   touch .env
   ```
2. Open `.env` in a text editor and add:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   YOUTUBE_API_KEY=your_youtube_api_key_here
   ```
   Replace `your_openai_api_key_here` and `your_youtube_api_key_here` with your actual API keys.  

---

## 5️⃣ Run the Application
Once everything is set up, start the app by running:
```bash
python main.py
```
This will launch the **TubeSage GUI**, allowing you to analyze YouTube videos.

---

## Troubleshooting
- If you get an **API key missing** error, ensure your `.env` file is correctly formatted and saved.
- If dependencies are missing, try:
  ```bash
  pip install -r requirements.txt
  ```
- If the app crashes, restart your terminal and run:
  ```bash
  python main.py
  ```

---

Now you can set up TubeSage independently and start analyzing YouTube videos.

