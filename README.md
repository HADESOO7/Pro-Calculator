<div align="center">

  <h1>🧮 Pro Scientific Calculator</h1>
  
  <p>
    A high-performance, web-based scientific calculator featuring a <br>
    <strong>mobile-first dark mode UI</strong>, <strong>history tracking</strong>, and <strong>advanced trigonometric functions</strong>.
  </p>

  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
    <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
  </p>

  <h4>
    <a href="https://[YOUR-USERNAME].github.io/[YOUR-REPO-NAME]/">View Live Demo 🚀</a>
    <span> · </span>
    <a href="https://github.com/[YOUR-USERNAME]/[YOUR-REPO-NAME]/issues">Report Bug 🪲</a>
  </h4>
</div>

<br />

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#interface-preview">Interface Preview</a></li>
    <li><a href="#key-features">Key Features</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#technologies-used">Technologies Used</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

---

## 📱 About The Project

This project is a fully functional scientific calculator designed to replicate the premium experience of native mobile applications. Built entirely with vanilla web technologies, it emphasizes **user experience (UX)** through a distraction-free dark mode interface, tactile button feedback, and fluid animations.

Unlike standard web calculators, this application manages state to allow for complex chained calculations, history retrieval, and error handling without page reloads.

## 📸 Interface Preview

<div align="center"> 
  <img src="screenshots/[screenshot1.png]" alt="Calculator Main View" width="300" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="screenshots/[screenshot2.png]" alt="History Drawer View" width="300" />
</div>

> *The interface features a Glassmorphism-inspired history drawer and neon-accented controls optimized for OLED screens.*

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **Advanced Math** | Full support for Trigonometry (`sin`, `cos`, `tan`), Logarithms (`log`, `ln`), Roots (`√`), and Exponents (`^`). |
| **RAD / DEG Toggle** | Instantly switch calculation logic between Radians and Degrees with a visual indicator. |
| **Smart History** | A slide-up drawer stores past calculations. Clicking a history item re-inserts the result for new calculations. |
| **Error Handling** | Intelligent syntax parsing prevents app crashes on invalid inputs (e.g., division by zero). |
| **Responsive Design** | The layout adapts to simulated mobile dimensions with touch-friendly targets (48px+). |

## 🛠️ Technologies Used

* **Core:** Semantic HTML5
* **Styling:** CSS3 (Variables, Flexbox, Grid, Glassmorphism effects)
* **Logic:** Vanilla JavaScript (ES6+, DOM Manipulation, Event Handling)

## 🚀 Getting Started

To run this project locally on your machine, follow these simple steps.

### Prerequisites
* A modern web browser (Chrome, Firefox, Safari, Edge).

### Installation

1.  **Clone the repository**
    ```sh
    git clone [https://github.com/](https://github.com/)[YOUR-USERNAME]/[YOUR-REPO-NAME].git
    ```
2.  **Navigate to the project directory**
    ```sh
    cd [YOUR-REPO-NAME]
    ```
3.  **Open the file**
    Double-click `index.html` to launch the application in your default browser.

## 🧠 Code Highlight

  Sneak peak of the code. 

<div class="calculator">
    
    <div class="mode-indicator" id="modeBtn" onclick="toggleMode()">DEG</div>
    <div class="history-icon" onclick="toggleHistory()">🕒</div>

    <div class="display">
        <div id="expression"></div>
        <div id="result">0</div>
    </div>

    <div class="history-drawer" id="historyDrawer">
        <div class="drawer-header">
            <h3>History</h3>
            <button class="close-btn" onclick="toggleHistory()">✕</button>
        </div>
        <div class="history-list" id="historyList">
            </div>
        <button class="clear-btn" onclick="clearHistory()">Clear All History</button>
    </div>
