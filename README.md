# ChatGPT-Gemini-Full-width
Here is a professional and clear **README.md** for your script. It is designed to be hosted on GitHub or GreasyFork, explaining both the purpose and the technical benefits of the tool.

---

# LLM Ultra-Widescreen: ChatGPT & Gemini

A lightweight, privacy-focused Userscript to remove the narrow "reading column" restriction on ChatGPT and Google Gemini. This script forces the interface to use **96% of your screen width**, making it ideal for large monitors, coding, and data analysis.

## 🚀 Key Features

* **Ultra-Widescreen Support:** Expands the chat container from the default ~800px to nearly full screen.
* **Dual Compatibility:** Works seamlessly on both **ChatGPT (https://www.google.com/search?q=chatgpt.com)** and **Google Gemini**.
* **Deep-Selector Integration:** Uses advanced CSS selectors to bypass Tailwind's `max-width` constraints used by OpenAI.
* **Privacy-First:** Zero external dependencies. No tracking, no data collection, and no network requests.
* **Performance Optimized:** Injects CSS directly into the document head to avoid layout shift (CLS).

## 🛠️ Installation

1. **Install a Userscript Manager:**
* [Tampermonkey](https://www.tampermonkey.net/) (Recommended)
* [Violentmonkey](https://violentmonkey.github.io/)


2. **Create a New Script:**
* Open your extension dashboard and click **"Create a new script"**.


3. **Copy & Paste:**
* Delete the default template and paste the code from `LLM_FullWidth.user.js`.


4. **Save:**
* Press `Ctrl+S` (or `Cmd+S` on Mac) and refresh your ChatGPT/Gemini tabs.



## 📄 Configuration

If you feel 96% is **too wide** for your taste, you can easily adjust the width. Look for the following lines in the code:

```css
max-width: 96% !important;
width: 96% !important;

```

Change `96%` to a fixed value like `1200px` or a different percentage like `80%`.

## 🔒 Security & Privacy

This script is **100% safe**:

* **No `@connect` permissions:** It cannot talk to the internet.
* **No `innerHTML` usage:** Prevents any potential XSS vulnerabilities.
* **Open Source:** You can audit every line of code.

## ⚖️ License

This project is licensed under the **MIT License**. Feel free to modify and redistribute it as you wish.

---

**Would you like me to add a "Known Issues" section or include instructions on how to combine this with your previous "Collapsible Messages" script?**
