# Band Name Generator 🎸🎤✨

This is a simple web app that creates random band names using adjectives and nouns. It runs without a traditional server, thanks to Netlify Functions. 🎶⚡🌍

Check-out my app [here](https://bandnamestudio.netlify.app/).
---

## 📖 Table of Contents 📚🧭📌

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [Installation & Local Development](#installation--local-development)
5. [Project Structure](#project-structure)
6. [Deployment to Netlify](#deployment-to-netlify)
7. [Environment Variables](#environment-variables)
8. [Usage](#usage)
9. [Contributing](#contributing)
10. [License](#license)
11. [Acknowledgements](#acknowledgements)

---

## Project Overview 🎯📄💡

The **Band Name Generator** is a small app that mixes random words to create cool and funny band names. 🎵🎲✨

It uses:

- 🚀 **Express.js** to run the app logic
- 🖋️ **EJS** to handle what gets shown on the web page
- ☁️ **Netlify Functions** to make it work without a traditional server

You don’t need to manage your own server—it all runs in the cloud and handles traffic automatically. 🛠️🔄⚡

---

## Features 🧰🌟🔧

- 🎲 Generates a band name every time you click a button
- 💻 Simple and clean user interface
- 🔌 Works completely serverless using Netlify
- 🧩 Easy to add your own words for more fun names

---

## Prerequisites 📋💻🔍

To use or work on this app, you’ll need:

- 📦 [Node.js](https://nodejs.org/) (version 14 or newer)
- 🧰 [npm](https://www.npmjs.com/) (comes with Node.js)
- 🛠️ [Netlify CLI](https://docs.netlify.com/cli/get-started/) (to test and deploy locally)

---

## Installation & Local Development 🧑‍💻📂⚙️

1. 📥 **Get the code from GitHub**

   ```bash
   git clone https://github.com/VINAYMADIVAL/Band-Name-Generator.git
   cd Band-Name-Generator
   ```

2. 📦 **Install needed packages**

   ```bash
   npm install
   ```

3. 🧪 **Start the app locally**

   ```bash
   npm start
   # or
   netlify dev
   ```

4. 🌐 **Go to** `http://localhost:8888` in your web browser and try it out! 🎉🔁🎧

---

## Project Structure 🗂️📁🧱

```
my-repo/
├─ netlify.toml             # Settings for Netlify
├─ package.json             # Project info and dependencies
└─ netlify/
   └─ functions/
      └─ server/
         ├─ index.js        # Express app setup
         ├─ server.js       # Connects Express to Netlify
         ├─ views/          # Web page templates
         │   ├─ index.ejs
         │   └─ partials/
         │       ├─ header.ejs
         │       └─ footer.ejs
         └─ public/         # CSS and images
             └─ styles/
                 └─ main.css
```

---

## Deployment to Netlify 🚀🔧🌐

1. 🔗 **Connect your GitHub repo** to Netlify
2. ⚙️ **Check your **``** file**:
   ```toml
   [build]
     functions = "netlify/functions"
     command   = "echo 'nothing to build'"

   [[redirects]]
     from   = "/*"
     to     = "/.netlify/functions/server"
     status = 200
   ```
3. 🚀 **Push your code** to GitHub
4. 🔄 Netlify will build and host the app automatically

---

## Environment Variables ⚠️🔒🧬

⚠️ You don’t need any special settings for this project to work. If you add more advanced features later, you might use them. 🔐📄🛡️

---

## Usage 🧪📲🎶

- 🖱️ Click the **Generate Band Name** button
- 📢 See the name appear below the form
- 📤 Use the name however you like—just for fun or for your next band! 🕺🎸📯

---

## Contributing 🤝🛠️📈

Want to help improve this app? Here’s how:

1. 🍴 Fork this repo on GitHub
2. 🌿 Make a new branch for your changes
3. 💾 Save your work with a clear commit message
4. 📤 Push your branch to your GitHub
5. 📬 Create a Pull Request so we can review it

📌 Please write clean code and test what you add. 🔍✅💡

---

## License 📄⚖️🔓

📄 This project currently doesn't have any License. You can reuse it or change it for your own projects. 📘🔏✅

---

## Acknowledgements 🙏🎉👏

- 🙏 Thanks to the guidance of tutor Dr.Angela Yu from Udemy
- 💡 Inspired by all the fun band name generators out there 🎼💭💫

