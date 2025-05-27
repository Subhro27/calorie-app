# 🍔 CALORIE TRACKER - AI POWERED FOOD ANALYZER 
Link : https://subhro27.github.io/calorie-app/

A modern, sleek Calorie Tracker web application that uses the **Groq LLaMA-4 Scout API** to detect food and estimate nutritional values (Calories, Protein, Carbs, Fats) from an uploaded image or a live photo. It also integrates **ImgBB API** to securely host and retrieve image URLs.

## 🚀 Features

- 📸 Upload or take a live photo of your food.
- 🧠 AI-powered food detection and calorie estimation using **Meta LLaMA-4 Scout via Groq API**.
-☁️ Image hosting via **ImgBB API** for smooth and secure file handling.
- ✨ Stunning UI with animated sliders and glowing neon aesthetics.
- 📊 Nutrition breakdown for each detected food item.
- ⚡ Fast response with minimal latency using Groq’s ultra-performant inference engine.

---

## 🛠️ Tech Stack

- **Frontend**: HTML, CSS (with Tailwind-style neon UI), JavaScript
- **Image Hosting**: [ImgBB API](https://api.imgbb.com/)
- **Food Detection & Nutrition Estimation**: Groq LLaMA-4 Scout (17B) API

---

## 🧠 How It Works

1. User uploads or takes a food photo.
2. Image is uploaded to ImgBB → returns a hosted image URL.
3. This URL is sent to the **Groq LLaMA-4 Scout API**.
4. Groq processes the image and returns food names + estimated nutrition info.
5. UI updates with real-time sliders and values for each food item.

---

## 🔑 Setup & Usage

### 1. Clone the Repo

```bash
git clone https://github.com/Subhro27/calorie-app.git
cd calorie-app
````

### 2. Add Your API Keys

Create a `config.js` file in the root directory with your credentials:

```js
// config.js
const GROQ_API_KEY = 'your-groq-api-key-here';
const IMGBB_API_KEY = 'your-imgbb-api-key-here';
```

### 3. Start the Project

You can use Live Server or simply open `index.html` in your browser:

```bash
# Using VS Code extension: Live Server
Right-click index.html -> "Open with Live Server"
```

Or double-click `index.html` manually.

---

## 🔐 APIs Used

### 🧠 Groq LLaMA-4 Scout (Food Image Understanding)

* Model: `llama-4-vision-17b`
* Task: Object detection + nutrition estimation from image
* Provider: [Groq](https://console.groq.com/)

### ☁️ ImgBB API

* Purpose: Secure image hosting & temporary storage
* Docs: [https://api.imgbb.com/](https://api.imgbb.com/)

---


## 🙌 Acknowledgements

* **Groq AI** for LLaMA-4 Scout blazing-fast inference
* **ImgBB** for free image hosting
* Inspired by real-world fitness apps and powered by open APIs.

---

