# Lines Of Code Counter

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,100:00B4DB&height=220&section=header&text=Lines%20Of%20Code%20Counter&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Measure%20Analyze%20And%20Visualize%20Your%20Codebase&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-4.1.0-00B4DB?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-93.9K-0F2027?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FFD700?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-cli%20%7C%20web%20%7C%20vscode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

</div>

---

## 📊 The Ultimate Code Metrics Tool

How big is your project, really? While lines of code (LOC) is not a perfect measure of complexity, it remains one of the most universally understood metrics in software engineering. Whether you are a solo developer tracking your progress, a team lead estimating project scope, or a researcher analyzing open-source repositories, having an accurate and fast LOC counter is essential.

**Lines Of Code Counter** is a blazing-fast, highly accurate, and beautifully designed tool that supports over 150 programming languages. Unlike basic `wc -l` scripts that count blank lines and comments, this tool is powered by advanced lexical analyzers. It intelligently distinguishes between actual source code, comments, and empty lines, giving you a true picture of your codebase's size.

This repository provides a complete ecosystem: a powerful CLI for automation, a stunning web dashboard for visual analysis, and a VS Code extension for real-time stats. It can process millions of lines of code in seconds, making it the perfect tool for analyzing massive monorepos or open-source projects with decades of history.

<img width="680" height="453" alt="input1" src="https://github.com/user-attachments/assets/891c1a1d-2a8b-48ed-a29d-68a1ae92e05b" />


---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🚀 **Blazing Fast** | Written in Rust, it processes millions of lines in milliseconds |
| 🌐 **150+ Languages** | Supports Python, JavaScript, Rust, Go, C++, and everything in between |
| 🧠 **Smart Parsing** | Accurately separates comments, blanks, and actual source code |
| 📊 **Beautiful Dashboard** | Interactive charts showing language distribution and file sizes |
| 🎨 **Git Integration** | Track how your LOC changes over time with commit history analysis |
| 🛠️ **CI/CD Ready** | JSON and CSV output formats for seamless pipeline integration |
| 💻 **VS Code Extension** | See real-time LOC stats right in your editor's status bar |
| 📦 **Zero Config** | Just point it at a folder and it works out of the box |

---

## 🛠️ How To Use The Tool

Instead of a traditional installation guide, here is how you can use the Lines Of Code Counter in your daily workflow.

### 💻 For The Command Line Power User
You can run the tool directly from your terminal without any complex setup. It integrates perfectly with your shell scripts. Simply navigate to your project root and run the counter. It will output a beautifully formatted table directly in your terminal, showing you exactly how many lines of code you have written versus how many are comments.

### 📊 For The Visual Thinker
If you prefer graphs and charts, the built-in web dashboard is for you. Once you run the analysis, the tool generates a local HTML file. Open it in your browser, and you will be greeted by a stunning, interactive sunburst chart. You can click on different slices to drill down into specific folders and see exactly which language dominates your project.

### 💻 For The VS Code Enthusiast
Forget switching between terminal and editor. The VS Code extension brings the power of the counter directly to your status bar. As you type, it updates in real-time. You can instantly see the total LOC, the number of files you have modified, and the percentage of comments in your current file. It is the perfect way to stay aware of your progress without breaking your flow.

---

<div align="center">

### 🔗 Ready to measure your code?

[![Get Tool](https://img.shields.io/badge/📊_GET_TOOL-0F2027?style=for-the-badge&logoColor=white)](https://share.google/CnF0iygqBBFxQbr2Q)

</div>

---

## 🧠 Under The Hood: How The Counter Works

Naively counting lines in a file is easy, but accurately identifying what is code and what is a comment is surprisingly difficult. Different languages have different comment syntaxes (e.g., `//`, `#`, `/* */`, `<!-- -->`).

This tool uses a technique called **Tokenization**. It reads the file and breaks it down into tokens (keywords, identifiers, symbols). By using a state machine that understands the grammar of the specific language, it can determine whether a line is inside a string literal, a multi-line comment, or actual executable code.

For performance, the tool uses the **Rayon** library in Rust to parallelize file reading. It spawns multiple threads to process different files simultaneously, utilizing all the cores on your CPU. This is why it can analyze a massive Linux kernel repository in just a few seconds, while other tools take minutes.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-00B4DB?style=for-the-badge&logoColor=white)](https://share.google/CnF0iygqBBFxQbr2Q)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We are always adding support for new languages and improving our tokenizers. If you have found a bug in a specific language parser, or want to add a new feature to the web dashboard, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-language`).
3. **Commit** your changes (`git commit -m 'Add new language support'`).
4. **Push** to the branch (`git push origin feature/new-language`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your project stats, ask for help with CI/CD integration, and discuss the latest trends in software metrics.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@loc-counter.dev.

---

<div align="center">

### ⭐ If this tool helps you measure your project, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FFD700?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/lines-of-code-counter)

---

### 🚀 Start counting your lines today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-007ACC?style=for-the-badge&logoColor=white)](https://share.google/CnF0iygqBBFxQbr2Q)

<sub>Crafted with precision and ❤️ by the Lines Of Code Counter community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:00B4DB,100:0F2027&height=120&section=footer)

</div>
