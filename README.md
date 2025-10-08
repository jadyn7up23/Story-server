# Story Server

An interactive mystery-solving game where players act as detectives to solve dynamic murder cases. The game features dynamic story generation, NLP sentiment analysis, and real-time character interactions.

## Table of Contents
- [Features](#features)
- [Installation & Setup](#installation--setup)
- [How to Play](#how-to-play)
- [Advanced Configuration](#advanced-configuration)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Features
- Dynamic mystery generation with randomized victims, suspects, motives, and clues.
- Sentiment analysis using NLTK's `SentimentIntensityAnalyzer`.
- Real-time API integration for character responses.
- Interactive gameplay with interrogation and accusation mechanics.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<jadyn7up23>/story-server.git
   cd story-server

   ## Features
| Feature                  | Description                                      |
|--------------------------|--------------------------------------------------|
| Dynamic Story Generation | Randomized victims, suspects, motives, and clues.|
| Sentiment Analysis       | Analyzes user messages and AI responses.         |
| Real-Time Interaction    | Characters respond dynamically via LM Studio.    |

## 🛠 Installation & Setup

### 0️⃣ Clone the repository (code)
Git is a little language widely used to help people update and download software projects. Make sure you have git by entering `git` in your terminal. If it doesn't recognize that command, [install it](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Now, clone the repository to whatever location you would like, using `git clone https://github.com/jadyn7up23/story-server.git':

![image](https://github.com/user-attachments/assets/dc328965-fc46-47b0-85db-ac4af7c820c1)

Then, **navigate to the folder where the project files are** with "cd story-server"
![image](https://github.com/user-attachments/assets/f64973f6-8b3f-41b9-86d8-7302c10924f3)

### 1️⃣ Install Dependencies
Make sure you have **Python 3.9+** installed in your system or in a [virtual enviroment](https://realpython.com/python-virtual-environments-a-primer/#how-can-you-work-with-a-python-virtual-environment). 

and install the required packages:
```bash
pip install -r requirements.txt
```

### 2️⃣ Run LM Studio
This project uses **LM Studio** to serve the Mistral model locally. Download and install [LM Studio](https://lmstudio.ai/), download mistral-7b-instruct-v0.3 from the 🔍discover tab of LM Studio, then load the model and start the server at the ▶️ developer tab:

![image](https://github.com/user-attachments/assets/a212c3b0-3681-410d-9e90-1f795f14d65a)


### 3️⃣ Launch the Chainlit App
Run the interactive storytelling app from the story-server 📂 folder with:
```bash
chainlit run app.py
```
Your chat adventure will open in a browser tab! 🏹📜

---

## 🗣 How to Play
- Start the story and read the **narrator’s introduction**.
- Chat with characters by mentioning them: `@crow` or `@wolf`.
- Make decisions that shape the journey.
- Watch the AI **stream responses in real-time**!

💡 *Pro Tip:* You can modify character behavior in `cast_of_characters.py`.

---

## 🔧 Advanced Configuration
Want to customize the storytelling experience? Try these:
- **Modify the Story Opening**: Edit `story.py` to change how the adventure begins.
- **Adjust AI Personalities**: Change attributes in `cast_of_characters.py`.
- **Fine-Tune Responses**: Implement text analysis in `app.py` to process dialogue.

---

## 🛠 Troubleshooting
❌ **Issue:** "Connection refused at localhost:1234"  
✅ **Solution:** Ensure LM Studio is running and serving the API.

❌ **Issue:** "Characters not responding properly"  
✅ **Solution:** Check `cast_of_characters.py` for errors in character definitions.

❌ **Issue:** "Chainlit not launching"  
✅ **Solution:** Ensure `chainlit` is installed (`pip show chainlit`) and restart the app.

---

## 💬 Join the Community
Need help or want to share your adventure? Join the [Chainlit Discord](https://discord.gg/k73SQ3FyUh)!

Happy storytelling! 🎭📚
## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
