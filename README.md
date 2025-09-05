# FastAPI WebSocket Chat 🚀

A simple **real-time chat application** built with **FastAPI** and **WebSockets**.  
This demo lets multiple users join and exchange messages instantly via a minimal frontend.


## 📂 Project Structure
.
├── main.py              # FastAPI backend with WebSocket endpoint
├── static/
│   └── chat.html        # Frontend (basic HTML + JS for WebSocket)
├── requirements.txt     # Dependencies
└── README.md


## ⚙️ Setup & Installation

1. **Clone the repository**
   
   git clone https://github.com/Sricharan7652/fastapi-websockets.git
   cd fastapi-websockets

3. **(Optional) Create a virtual environment**

   python -m venv .venv
   # Activate
   .venv\Scripts\activate      # Windows
   source .venv/bin/activate   # Linux/Mac

4. **Install dependencies**

   pip install -r requirements.txt

---

## ▶️ Run the App

Start the server:

uvicorn main:app --reload

Now open:

http://127.0.0.1:8000

---

## 💬 Usage

* Open the app in **two different browser windows/tabs**.
* Type a message in one and hit **Send** (or press Enter).
* The message will appear in both windows instantly.

---

## 📌 Requirements

* Python 3.8+
* Dependencies from `requirements.txt`:

  * `fastapi`
  * `uvicorn`
  * `websockets`

---

## 🛠️ Development Notes

* The frontend is kept minimal (`chat.html`) for simplicity.
* Messages are broadcasted to all connected WebSocket clients.
* Extendable for:

  * Chat rooms
  * Usernames
  * Message persistence (DB)
