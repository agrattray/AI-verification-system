# 🧠 AI Assistant for Purely Cakes

This project powers the AI voice assistant for **Purely Cakes**, enabling smart, automated responses to customer phone calls using Twilio and OpenAI.

## 📌 Overview

When a customer calls the Purely Cakes business number, this assistant handles the call by:

* Answering with a professional greeting
* Transcribing the caller’s voice using **Twilio Voice + Whisper (optional)**
* Sending the transcription to **OpenAI GPT-4** for intelligent replies
* Optionally forwarding the call or saving voicemails

The assistant is live and connected to the custom domain:
🔗 **[https://purelycakes.com](https://purelycakes.com)**

---

## ⚙️ Technologies Used

* **Twilio Voice** – Handles incoming calls and call flow
* **OpenAI API** – Generates conversational responses
* **Node.js / Express** (or serverless functions) – Processes requests
* **Vercel** – Handles deployment and live endpoint hosting
* **TwiML / Webhooks** – Manages Twilio call routing

---

## 🚀 Deployment Instructions

1. Clone the repo or upload your project to [Vercel](https://vercel.com)
2. Set environment variables:

   * `OPENAI_API_KEY`
   * `TWILIO_ACCOUNT_SID`
   * `TWILIO_AUTH_TOKEN`
3. Make sure the endpoint (e.g., `/api/voice`) is publicly accessible
4. In the Twilio Console, go to **Phone Numbers > A Call Comes In**

   * Set to: `https://purelycakes.com/api/voice`

---

## 📞 Call Flow Example

1. Caller dials the Purely Cakes number
2. Twilio hits the `/api/voice` endpoint
3. The assistant:

   * Says: “Hi, thanks for calling Purely Cakes. How can I help you?”
   * Sends the spoken question to OpenAI
   * Replies with a spoken AI-generated response

---

## 📬 Contact

Created by **Arthur Rattray**
📧 [arthur@vilowebdevelopment.com](mailto:arthur@vilowebdevelopment.com)
🌐 [https://purelycakes.com](https://purelycakes.com)
