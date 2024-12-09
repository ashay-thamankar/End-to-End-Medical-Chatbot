# End-to-End Medical Chatbot 🤖💊

An end-to-end medical chatbot that enables **semantic search** and leverages **GPT** to provide accurate answers from a medical book. 🌟 Whether you're seeking medical information or performing knowledge-based searches, this chatbot is here to assist you! 🩺✨

---

## Features 🚀

### 🌐 Backend:
- 📚 Extracts content from a medical book (PDF) using **LangChain**.
- 🧠 Generates vector embeddings with **Huggingface models**.
- 📂 Builds a **semantic search knowledge base** stored in **Pinecone Vector DB**.

### 💻 Frontend:
- 🎨 User-friendly **Flask UI** for submitting queries.
- 🔍 Retrieves ranked results using query embeddings.
- 🧾 Provides **contextual answers** powered by **OpenAI GPT**.

---

## Chatbot in Action! 🎉  
![Chatbot Screenshot](https://github.com/ashay-thamankar/End-to-End-Medical-Chatbot/blob/main/media/Medical%20ChatBot%20Screenshot.png)

---

## How to Run? 🛠️  

### Steps  

1. **Clone the Repository** 🗂️  
   ```bash
   git clone https://github.com/ashay-thamankar/End-to-End-Medical-Chatbot.git
   cd End-to-End-Medical-Chatbot
   ```

2. **Create a Conda Environment** 🐍  
   ```bash
   conda create -n medibot python=3.10 -y
   conda activate medibot
   ```

3. **Install the Requirements** 📦  
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Environment Variables** 🔑  
   Create a `.env` file in the root directory with the following:  
   ```ini
   PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
   OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
   ```

5. **Prepare the Knowledge Base** 🧩  
   ```bash
   python store_index.py
   ```

6. **Start the Chatbot** 🖥️  
   ```bash
   python app.py
   ```

7. **Access the Application** 🌐  
   Open your browser and visit:  
   ```plaintext
   http://localhost:8080
   ```

---

## Tech Stack 🛠️  
- **Python** 🐍: Backend logic and data processing.  
- **LangChain** 🛠️: Chunking and embedding text data.  
- **Huggingface** 🤗: Generating vector embeddings.  
- **Pinecone** 🌲: Storing and retrieving embeddings.  
- **OpenAI GPT** 🧠: Providing intelligent and context-aware responses.  
- **Flask** 🌐: User-friendly web interface for interaction.  

---

🎉 Happy chatting with your intelligent medical assistant! 😊