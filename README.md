# DoodleDraw

```markdown
# ✏️ DoodleDraw

A **real-time multiplayer drawing and guessing game** built with **TypeScript, Node.js, Express, and Socket.IO** for scalable, low-latency fun with friends.

---

## 🎯 Features

✅ **Real-time multiplayer** using Socket.IO  
✅ **Room-based gameplay** (play with friends using room codes)  
✅ **One player draws**, others guess the word  
✅ **Masked letter reveal** as the timer counts down  
✅ **Score calculation** based on how quickly users guess  
✅ **Round rotation** after correct guess or timeout  
✅ **TypeScript clean architecture** for scalability  
✅ In-memory store for **zero DB dependency** (perfect for learning and MVPs)

---

## 🗂️ Project Structure

```

doodledraw-backend/
│
├── src/
│   ├── controllers/       # Socket event handlers
│   │    └── gameController.ts
│   ├── services/          # Game logic and helpers
│   │    └── gameService.ts
│   ├── models/            # In-memory room management
│   │    └── rooms.ts
│   └── server.ts          # Entry point
│
├── dist/                  # Compiled JS files after build
├── package.json
└── tsconfig.json

````

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
https://github.com/sriramalavalapati3/DoodleDraw.git
cd doodledraw-backend
````

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Development server (with live reload)

```bash
npm run dev
```

Server will run on:

```
http://localhost:3000
```

### 4️⃣ Production build

```bash
npm run build
npm run start
```

---

## ⚙️ Tech Stack

* **Node.js** – Runtime
* **TypeScript** – Type-safe backend development
* **Express** – HTTP server
* **Socket.IO** – Real-time communication
* **ts-node-dev** – Live reload for development
* **In-memory data storage** – For simplicity and speed

---

## 🚩 How It Works

1️⃣ **Room Creation & Joining**:

* Players join a room using a `roomCode` and `username`.
* If the room doesn't exist, it is created automatically.

2️⃣ **Game Flow**:

* One player (rotating drawer) receives a secret word to draw.
* Other players see a masked version (`_ _ _ _`) and try to guess.
* Every 5 seconds, one letter is revealed to assist guessing.
* Players receive **higher scores for faster guesses**.
* After a correct guess or timeout, the next player becomes the drawer.

3️⃣ **Drawing & Guessing**:

* The drawer’s canvas is shared live with other players.
* Guessing happens in real-time with immediate feedback.

4️⃣ **No Database**:

* All rooms and game states are stored in-memory.
* Ideal for learning, MVPs, and low-cost deployment.
* If the server restarts, all data resets.

---

## 🧩 Potential Future Enhancements

✅ **Frontend with Tailwind + Canvas Drawing**
✅ **Room reconnection support on refresh**
✅ **Persistent scores using Redis/Postgres**
✅ **Rate limiting & validation for production**
✅ **Redis adapter for Socket.IO to support horizontal scaling**
✅ **Deploy on Render/Fly.io/Hetzner for low-latency**

---

## 🧑‍💻 Contributing & Learning

This project is designed to **boost your real-time backend skills using TypeScript** while understanding:

✅ Socket.IO architecture
✅ Real-time room and player management
✅ Round-based multiplayer game flow
✅ Type-safe backend development

Feel free to fork and build your own variations, add authentication, or build a frontend using React/Next.js/Vue as you grow.

---

## 📜 License

MIT – Feel free to use, modify, and build upon it for your portfolio and learning.

---

## ✨ Author

**Sriram Alavalapati**

> Learning by building **scalable, fun projects**.

---

## 📞 Contact

If you have questions while learning or building on top of this:

* Drop your queries anytime, and we will debug together.
* I will assist you step-by-step with frontend, Redis integration, and deployment when you are ready.

---

Happy Building 🚀✨

```

---

### ✅ What to do next:
1️⃣ Create `README.md` in your `doodledraw-backend` folder.  
2️⃣ Copy-paste the above content.

✅ This will **make your GitHub repository professional and clear for your portfolio**.

---

If you want, I can also prepare:
✅ A **clean `frontend/` plan** with Tailwind, canvas, and Socket.IO integration step-by-step next.  
✅ Or add **Redis scaling guide** when you’re ready for production readiness.

Let me know your **next priority** so we continue your learning efficiently.
```
