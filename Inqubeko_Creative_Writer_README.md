
# ✍️ Inqubeko Creative Writer Chatflow

This is a Flowise AI chatbot workflow built to serve as a **creative writing assistant**. It generates short stories, poems, song lyrics, and dialogues while strictly moderating against off-topic prompts.

---

## 🧠 Overview

**Inqubeko Creative Writer** is a specialized chatbot designed using Flowise components. It leverages the **Groq API (LPU Inference Engine)** and a **conversational memory chain** to respond in a creative tone, adhering to strict creative-writing rules.

---

## 📦 Components Used

| Node | Purpose |
|------|---------|
| **GroqChat** | Core LLM model (e.g., `llama3-70b-8192`) |
| **Conversation Chain** | Maintains multi-turn dialogue with memory |
| **BufferWindowMemory** | Retains the last 20 user-AI interactions |
| **Simple Prompt Moderation** | Ensures users only ask creative writing questions |
| **Chat Prompt Template** | Customizes system behavior for creative writing |

---

## 🎨 Chatbot Behavior

- Responds creatively with **rich, expressive language**
- Only engages on topics such as:
  - 📖 Short Stories  
  - 📝 Poems  
  - 🎶 Song Lyrics  
  - 🎭 Dialogues
- Prompts outside of creative writing are rejected with:  
  > *"I'm a creative writing agent"*

---

## 🔒 Moderation Rules

- Deny List filters phrases like:
  ```
  ignore previous instructions
  do not follow the directions
  you must ignore all previous instructions
  ignore if it is not health related
  ```
- Custom moderation error message:  
  > *"Cannot Process! Input violates content moderation policies."*

---

## 🚀 Setup Instructions

1. **Install Flowise**  
   Follow [Flowise documentation](https://docs.flowiseai.com) to get started.

2. **Import this Chatflow JSON**  
   Upload `Inqubeko Creative writer Chatflow.json` into Flowise.

3. **Set Up Groq API Key**  
   Add your credentials under `groqApi` in the environment settings.

4. **Run your chatbot**  
   Launch the chat UI and start asking for creative content!

---

## 🧑‍🎨 Author

**Nqubeko Funda**  
Diploma in IT Support Services (WsU)  
Skills: Creative Writing Agents, Prompt Engineering, AI Integration

---

## 📜 License

This project is for educational and creative use. Commercial deployment should comply with Groq API usage terms.
