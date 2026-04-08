<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Help Desk Chatbot</title>

<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: #f5f7fb;
}

/* HEADER */
header {
  background: linear-gradient(135deg, #4a90e2, #357abd);
  color: white;
  text-align: center;
  padding: 30px 20px;
}

header h1 { margin: 0; }
header p { opacity: 0.9; }

/* HERO */
.hero {
  text-align: center;
  padding: 40px 20px;
}

.hero h2 {
  font-size: 28px;
  margin-bottom: 10px;
}

.hero p {
  color: #555;
}

/* CHAT BUTTON */
#chatBtn {
  position: fixed;
  bottom: 25px;
  right: 25px;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  border: none;
  background: #4a90e2;
  color: white;
  font-size: 22px;
  cursor: pointer;
  box-shadow: 0 8px 20px rgba(0,0,0,0.2);
}

/* CHAT WINDOW */
#chatWindow {
  position: fixed;
  bottom: 100px;
  right: 25px;
  width: 350px;
  height: 500px;
  background: white;
  border-radius: 15px;
  display: none;
  flex-direction: column;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

/* CHAT HEADER */
.chat-header {
  background: #4a90e2;
  color: white;
  padding: 12px;
  font-weight: bold;
}

/* FAQ */
.faq-buttons {
  padding: 10px;
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
  border-bottom: 1px solid #eee;
}

.faq-buttons button {
  background: #e5e7eb;
  border: none;
  padding: 6px 10px;
  border-radius: 10px;
  cursor: pointer;
  font-size: 12px;
}

/* MESSAGES */
.messages {
  flex: 1;
  padding: 10px;
  overflow-y: auto;
}

.message {
  margin: 8px 0;
  padding: 10px;
  border-radius: 12px;
  max-width: 75%;
}

.user {
  background: #4a90e2;
  color: white;
  margin-left: auto;
}

.bot {
  background: #e5e7eb;
}

/* INPUT */
.input-area {
  display: flex;
  border-top: 1px solid #ddd;
}

input {
  flex: 1;
  border: none;
  padding: 10px;
  outline: none;
}

button.send {
  background: #4a90e2;
  color: white;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 15px;
  background: #f1f1f1;
  font-size: 12px;
  color: #666;
}
</style>
</head>

<body>

<header>
  <h1>AI Help Desk Chatbot</h1>
  <p>Smart assistant for student queries, admissions, and support</p>
</header>

<div class="hero">
  <h2>24/7 AI Support for Educational Institutions</h2>
  <p>Ask about admissions, fees, exams, or campus services instantly.</p>
</div>

<button id="chatBtn" onclick="toggleChat()">💬</button>

<div id="chatWindow">
  <div class="chat-header">AI Assistant</div>

  <!-- FAQ BUTTONS -->
  <div class="faq-buttons">
    <button onclick="quickReply('admission')">Admission</button>
    <button onclick="quickReply('fees')">Fees</button>
    <button onclick="quickReply('exam')">Exams</button>
    <button onclick="quickReply('courses')">Courses</button>
  </div>

  <div class="messages" id="messages"></div>

  <div class="input-area">
    <input id="input" placeholder="Ask something..." />
    <button class="send" onclick="sendMessage()">Send</button>
  </div>
</div>

<footer>
  © 2026 AI Help Desk | Educational Support System
</footer>

<script>
const chatWindow = document.getElementById("chatWindow");
const messagesDiv = document.getElementById("messages");
const input = document.getElementById("input");

/* FAQ Answers */
const faqAnswers = {
  admission: "Admissions are open! Apply online or visit campus.",
  fees: "Fees range between ₹20,000 - ₹80,000 per year.",
  exam: "Exams are conducted semester-wise.",
  courses: "We offer BCA, BBA, BA, BSc, MBA and more."
};

/* Toggle Chat */
function toggleChat() {
  chatWindow.style.display =
    chatWindow.style.display === "flex" ? "none" : "flex";
}

/* Add Message */
function addMessage(text, type) {
  const msg = document.createElement("div");
  msg.className = "message " + type;
  msg.innerText = text;
  messagesDiv.appendChild(msg);
  messagesDiv.scrollTop = messagesDiv.scrollHeight;
}

/* Quick Reply */
function quickReply(topic) {
  addMessage(topic, "user");
  addMessage(faqAnswers[topic], "bot");
}

/* Send Message */
async function sendMessage() {
  const userText = input.value.trim();
  if (!userText) return;

  addMessage(userText, "user");
  input.value = "";

  // Check FAQ first
  const lower = userText.toLowerCase();
  for (let key in faqAnswers) {
    if (lower.includes(key)) {
      addMessage(faqAnswers[key], "bot");
      return;
    }
  }

  // Backend AI call (SAFE)
  try {
    const res = await fetch("http://localhost:3000/chat", {
      method: "POST",
      headers: {
        "Content-Type": "application/json"
      },
      body: JSON.stringify({ message: userText })
    });

    const data = await res.json();
    addMessage(data.reply, "bot");

  } catch (err) {
    addMessage("Error connecting to server", "bot");
  }
}

/* Enter key */
input.addEventListener("keypress", function(e) {
  if (e.key === "Enter") sendMessage();
});
</script>

</body>
</html>