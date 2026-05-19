<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=AuthentiQ&fontSize=56&fontColor=fff&animation=twinkling&fontAlignY=38&desc=Cryptographic%20Certificate%20Verification%20Platform&descSize=16&descColor=fff&descAlignY=60" />

<br/>

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://mongodb.com)
[![SHA256](https://img.shields.io/badge/SHA--256-Cryptography-FF6B6B?style=for-the-badge)](https://en.wikipedia.org/wiki/SHA-2)

![License](https://img.shields.io/badge/License-MIT-00d4ff?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![PRs](https://img.shields.io/badge/PRs-Welcome-7c3aed?style=flat-square)

</div>

---

## 🔐 What is AuthentiQ?

**AuthentiQ** is a trust-minimized certificate verification platform that lets institutions issue cryptographically verifiable academic credentials. Anyone can verify a certificate's authenticity instantly — no blockchain, no third-party trust required.

> Verify in seconds. Tamper-proof by design. No intermediaries needed.

---

## ✨ Features

- 🔒 **SHA-256 Cryptographic Hashing** — Each certificate gets a unique, unforgeable hash
- ⚡ **Instant Verification** — Anyone can verify authenticity by uploading the file
- 🏫 **Institution Dashboard** — Issue and manage certificates at scale
- 📜 **Bulk Issuance** — Generate and hash hundreds of certificates at once
- 🌐 **Public Verification API** — Integrate verification into any system
- 🔑 **Role-based Access** — Separate flows for institutions and verifiers
- 📁 **File-based Proof** — The document itself is the proof — no QR codes needed
- 🔄 **Tamper Detection** — Any modification to the file instantly fails verification

---

## 🛠️ Tech Stack

| Layer | Technology |
|:---|:---|
| **Language** | JavaScript |
| **Backend** | Node.js, Express |
| **Hashing** | SHA-256 (Node.js crypto module) |
| **Database** | MongoDB |
| **Auth** | JWT |
| **Frontend** | HTML, CSS, Vanilla JS |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- MongoDB (local or Atlas)

### Installation

```bash
git clone https://github.com/shaktivijayas/AuthentiQ.git
cd AuthentiQ
npm install
cp .env.example .env
```

### Environment Variables

```env
MONGODB_URI=mongodb://localhost:27017/authentiq
JWT_SECRET=your_jwt_secret
PORT=3000
```

### Run Locally

```bash
npm run dev    # development with nodemon
npm start      # production server
```

App runs at `http://localhost:3000`

---

## 📁 Project Structure

```
AuthentiQ/
├── src/
│   ├── controllers/      # Route handlers
│   ├── models/           # MongoDB schemas (Certificate, Institution, User)
│   ├── routes/           # API route definitions
│   ├── middleware/        # Auth, error handling
│   ├── utils/            # SHA-256 hashing helpers
│   └── app.js            # Express app entry
├── public/               # Frontend HTML/CSS/JS
├── .env.example
└── package.json
```

---

## 🏗️ How Verification Works

```
Institution                    AuthentiQ                    Verifier
    │                              │                            │
    │── Upload Certificate ───────►│                            │
    │                    SHA-256 Hash Generated                 │
    │                    Hash stored in MongoDB                 │
    │◄── Certificate + Hash ID ────│                            │
    │                              │                            │
    │                              │◄── Upload Certificate ─────│
    │                              │    Recompute SHA-256        │
    │                              │    Compare with stored hash │
    │                              │── VALID / INVALID ─────────►│
```

---

## 👨‍💻 Author

**Shakti Vijay A S** — [GitHub](https://github.com/shaktivijayas) · [LinkedIn](https://www.linkedin.com/in/shaktidev/)

<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling" />
</div>
