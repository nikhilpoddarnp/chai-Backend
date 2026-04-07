# Chai aur Backend ☕🚀

This is a backend project built using Node.js.

## 📌 Getting Started

Follow these steps to set up the project locally:

### 1️⃣ Initialize npm
```bash
npm init

# 2
Bhai ye **bahut important concept hai Node.js ka** 🔥 (interview me bhi aata hai)

Tumne likha:

```json
"type": "module"
```

Aur pooch rahe ho **kyun likhte hain aur iska matlab kya hai** — chalo simple me samajhte hain 👇

---

## 🧠 `type` kya hota hai?

`package.json` me `"type"` decide karta hai ki tumhara project ka **module system kaunsa hoga**:

### 2 types hote hain:

1. **CommonJS (default)**
2. **ES Modules (modern)**

---

## ✅ 1. CommonJS (default)

Agar tum `"type": "module"` nahi likhte, to Node.js by default ye use karta hai

### Syntax:

```js
const express = require('express');
module.exports = app;
```

👉 Ye **old method** hai

---

## ✅ 2. ES Modules (`"type": "module"`)

Jab tum ye likhte ho:

```json
"type": "module"
```

👉 Tab tum modern JavaScript use kar sakte ho

### Syntax:

```js
import express from 'express';
export default app;
```

👉 Ye **React / frontend jaisa syntax** hai

---

## 🔥 Tumhe `"type": "module"` kyun use karna chahiye?

* Modern syntax (clean & readable) ✅
* Frontend jaisa code (React se match) ✅
* Future-proof (industry standard ban raha hai) ✅

---

## ⚠️ Important Difference

| Feature | CommonJS           | ES Module (`module`)    |
| ------- | ------------------ | ----------------------- |
| Import  | `require()`        | `import`                |
| Export  | `module.exports`   | `export`                |
| Default | Yes (Node default) | Need `"type": "module"` |

---

## ❗ Tumne ek galti boli:

> `common.js` ya `module.js`

👉 Ye galat hai ❌
Sahi kya hai:

```json
"type": "module"
```

👉 `"commonjs"` likhne ki zarurat nahi hoti (default hota hai)

---

## 💡 Simple Line:

👉 `"type": "module"` = ES6 import/export enable karna

---

## 🚀 Example

### Without module:

```js
const fs = require('fs');
```

### With `"type": "module"`:

```js
import fs from 'fs';
```

---
# 3

 Bhai **`nodemon`** backend development ka ek mast tool hai 🔥
Main simple aur practical way me samjhata hoon 👇

---

# 🚀 Nodemon kya hota hai?

👉 **Nodemon ek tool hai jo automatically server restart karta hai**
jab bhi tum code me changes karte ho

---

## 🧠 Problem kya hoti hai normally?

Agar tum simple Node run karte ho:

```bash
node index.js
```

👉 Fir har change ke baad:

* server band karo ❌
* dubara run karo ❌

😤 boring ho jata hai

---

## ✅ Nodemon ka solution

```bash
nodemon index.js
```

👉 Ab:

* file change karo ✏️
* server automatically restart 🔄

🔥 time bach gaya!

---

# 📦 Install kaise kare?

## 🔹 Global install:

```bash
npm install -g nodemon
```

---

## 🔹 Project me (recommended):

```bash
npm install --save-dev nodemon
```

---

# ⚙️ Use kaise kare?

### Direct:

```bash
nodemon index.js
```

---

### Package.json me script bana lo (best 🔥)

```json
"scripts": {
  "start": "node index.js",
  "dev": "nodemon index.js"
}
```

👉 Run:

```bash
npm run dev
```

---

# 💡 Real Example

Tum backend bana rahe ho:

```js
console.log("Server running...");
```

👉 Save karte hi nodemon bolega:

```
[nodemon] restarting due to changes...
```

---

# 🧠 Simple Line:

👉 **Nodemon = auto restart tool for Node.js server**

---

# ⚠️ Important

* Production me use nahi karte ❌
* Sirf development ke liye hota hai ✅

---

# 4
now we install prettier
```
npm i prettier


