# 🏋️‍♂️ Personal Fitness AI Agent

**Personal Fitness AI Agent** is a **chat-based AI assistant** built using **Langflow**, **Streamlit**, and **Datastax Astra**. This tool provides personalized fitness guidance — from workout routines to nutrition advice — powered by a custom Langflow flow that delivers smart, contextual responses.

---

## 🚀 Features

- 💬 **Interactive chat interface** built with **Streamlit**
- 🔗 **Connects to Langflow API** hosted on **Astra**
- 🧠 **Understands user fitness queries** and provides contextual responses
- 🔐 **Secure** API key management with environment variables
- ⚙️ **Modular design** for easy customization of flows

---

## 🧰 Tech Stack

| Tech         | Purpose                             |
|--------------|-------------------------------------|
| 🧩 Langflow   | Visual framework for LLM workflows  |
| 🌐 Streamlit | Web-based UI for Python apps        |
| ☁️ Astra DB  | Langflow hosting and flow API       |
| 🐍 Python    | Core scripting & logic              |

---

## 📦 Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/personal-fitness-ai.git
cd personal-fitness-ai
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Create a `.env` file

Add your Astra **Application Token**:

```env
APP_TOKEN=your_application_token
```

### 4️⃣ Update flow configuration

Open `main.py` and edit the following lines:

```python
LANGFLOW_ID = "your-langflow-id"
FLOW_ID = "your-flow-id"
ENDPOINT = "customer"  # or your flow's actual endpoint
```

You can find these values in the Langflow dashboard under **API configuration**.

---

## ▶️ Usage

Start the Streamlit app:

```bash
streamlit run main.py
```

Once the app launches, enter a fitness-related message like:

> 🗨️ *"Create a 7-day beginner-friendly workout plan with rest days."*

And get instant AI-generated suggestions!

---

## 💡 Example Query Ideas

- *"What should I eat post-workout?"*
- *"Suggest a 4-day muscle-building plan."*
- *"Tips for staying consistent with home workouts?"*

---

## 🛠 Troubleshooting

| Issue                            | Fix                                                                 |
|----------------------------------|----------------------------------------------------------------------|
| `401 Unauthorized`               | Check your `APP_TOKEN` and make sure it’s valid                     |
| Output field errors              | Ensure your Langflow flow has properly configured output components |
| Flow not responding              | Make sure the flow is published and not in draft mode               |

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- 🎨 [Langflow](https://langflow.org) by Logspace
- ☁️ [Datastax Astra](https://www.datastax.com/astra)
- 🌟 [Streamlit](https://streamlit.io)
