# 🤖 AI Chatbot for Fun Conversations  

This project is a **GPT-powered AI chatbot** designed for **fun and engaging conversations**.  
The chatbot can **tell jokes, generate short stories, and role-play as different characters**.

---

## 📌 Features
✅ **Installs Required Libraries** – `transformers`, `torch`, `openai`.  
✅ **Loads a GPT-2 Model** – Uses a **pre-trained conversational AI**.  
✅ **Basic Chatbot** – Responds to user **input and questions**.  
✅ **Roleplaying Mode** – AI can take on **different character personalities**.  
✅ **Joke Mode** – Tells **funny AI-generated jokes**.  
✅ **Storytelling Mode** – Creates **short AI-generated stories**.  
✅ **Interactive Chatbot** – Runs a **continuous chat loop**.  

---

## 🎮 How to Use  

### **1️⃣ Run the Colab Notebook**  
Simply open **Google Colab** and run the provided script.

### **2️⃣ Start Chatting!**  
Type one of the following commands:  
- 🃏 `"Tell me a joke"` – The AI will **tell a joke**.  
- 📖 `"Tell me a story"` – The AI will **generate a short story**.  
- 🧙 `"Roleplay as a wizard"` – The AI will **pretend to be a wizard**.  
- 💬 Or **ask anything you want**!  

### **3️⃣ Exit the Chatbot**  
Simply type:

🔧 Roleplaying Mode (Character-Based Chatbot)
Make the chatbot act like a character (wizard, pirate, futuristic AI).
def roleplay_chat(persona, user_input):
    prompt = f"You are {persona}. Respond to: {user_input}"
    return chat(prompt)

print(roleplay_chat("a wise old wizard", "Tell me a spell to become invisible."))
print(roleplay_chat("a futuristic AI", "What will the world look like in 100 years?"))
😂 Joke Mode (Humor Chatbot)
Make the chatbot tell jokes.
def tell_joke():
    joke_prompt = "Tell me a funny joke about AI."
    return chat(joke_prompt)

print("😂", tell_joke())
📖 Storytelling Mode (AI as a Storyteller)
Let the chatbot generate short creative stories.
def generate_story():
    story_prompt = "Once upon a time, in a distant galaxy, there was a robot who discovered..."
    return chat(story_prompt)

print("📖", generate_story())
🔄 Interactive Chatbot
To chat continuously:
def interactive_chat():
    print("🤖 AI Chatbot: Hello! Let's chat. Type 'exit' to stop.")
    while True:
        user_input = input("You: ")
        if user_input.lower() == "exit":
            print("🤖 AI Chatbot: Goodbye! Have a great day! 👋")
            break
        elif user_input.lower().startswith("roleplay"):
            persona = user_input.split("roleplay as")[-1].strip()
            response = roleplay_chat(persona, "Introduce yourself.") if persona else "Please specify a roleplay character!"
        elif user_input.lower() == "tell me a joke":
            response = tell_joke()
        elif user_input.lower() == "tell me a story":
            response = generate_story()
        else:
            response = chat(user_input)

        print(f"\n🤖 AI Chatbot:\n{response}\n")

interactive_chat()
🛠️ Future Improvements
✅ Memory Feature – Make the chatbot remember past responses.
✅ Speech-to-Text – Allow voice input for interactions.
✅ Fine-Tuning GPT-3/4 – Train the chatbot on custom datasets.
✅ Deploy Online – Convert it into a Flask web app or Telegram bot.

📜 License
This project is licensed under the MIT License.

📧 Contact
For questions or suggestions, feel free to reach out:
👨‍💻 Duncan Kibet
📌 GitHub Profile: github.com/Duncan1738

🎯 Want to enhance your AI chatbot? Fork the repo & start experimenting! 🚀🔥
📢 Feel free to contribute & submit pull requests! 🤖💬
---

## **🚀 Next Steps**
- ✅ Add **voice interaction** using **speech-to-text and text-to-speech**.  
- ✅ Fine-tune GPT **for more conversational depth**.  
- ✅ Deploy a **web version (Flask, Streamlit, or React UI)**.  

Would you like **multi-language support, chatbot memory, or API integration**? 🚀🤖
