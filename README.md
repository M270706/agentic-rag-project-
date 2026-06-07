🤖 Playing with Agentic RAG

Hey! 👋 

This is a personal project I put together to finally understand how Artificial Intelligence actually searches for and retrieves information (RAG: Retrieval-Augmented Generation). 

I started out just to build a basic AI that could read my documents, but I ended up with "Agents"—basically giving the AI the ability to loop back and double-check its own work before answering.

## 🧰 What I used to build this:
* **The Brains:** LangChain (for the basics) and LangGraph (for the complex, looping agents).
* **The Memory:** I couldn't pick just one vector database, so I experimented with three of them to see how they compared: **ChromaDB**, **FAISS**, and **Typesense**.
* **The AI:** Groq (because it generates answers incredibly fast).

## 📁 What's in here?
* `document.ipynb` — Me figuring out the basics: chunking up text and turning it into numbers.
* `1-agenticrag.ipynb` — The fun stuff. Testing out LangGraph to make the AI act a bit more on its own.
* `typesense.ipynb` — A separate notebook where I specifically messed around with Typesense.
* `main.py` — The main script tying it all together.

## 🚀 Want to run it yourself?
If you want to download this and poke around, it's pretty easy to set up:

1. **Download the code** to your computer.

2. **Install the required packages** (I'd recommend using a virtual environment!):
   ```bash
   pip install -r requirements.txt

3. **Get an API Key:** You'll need a free API key from Groq. Once you have it, create a file named `.env` in this folder and paste it in like this:
```text
GROQ_API_KEY=your_actual_key_here
```

*(I added `.env` to the `.gitignore` file, so your key stays safe and won't upload to GitHub).*
4. **Play around!** Open up the Jupyter notebooks to run the code block-by-block, or just run the `main.py` file.
