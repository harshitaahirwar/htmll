![Typing](https://readme-typing-svg.herokuapp.com?color=blue&lines=Welcome+to+my+project;Frontend+Developer;QA+Engineer)
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=your-username&show_icons=true)
![HTML](https://img.shields.io/badge/HTML-orange?logo=html5)
![CSS](https://img.shields.io/badge/CSS-blue?logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-yellow?logo=javascript)

# 🚀 My Portfolio

![Typing](https://readme-typing-svg.herokuapp.com?lines=Welcome+to+my+portfolio)

## 🔗 Live Demo
[Click Here](https://your-site.com)

<details>
<summary>📂 Project Details</summary>

- Built with HTML, CSS, JS
- Responsive design
- API integration

</details>





<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <h1>Harshita Portfolio</h1>
  <button id="themeToggle">🌙</button>
</header>

<section class="hero">
  <h2 id="typing"></h2>
</section>

<section class="projects">
  <button onclick="filterProjects('all')">All</button>
  <button onclick="filterProjects('qa')">QA</button>
  <button onclick="filterProjects('frontend')">Frontend</button>

  <div class="project qa">Automation Testing Project</div>
  <div class="project frontend">Portfolio Website</div>
</section>

<section class="contact">
  <form>
    <input type="text" placeholder="Your Name">
    <input type="email" placeholder="Your Email">
    <button type="submit">Send</button>
  </form>
</section>

<script src="script.js"></script>
</body>
</html>





// Typing effect
const text = "QA Engineer | Frontend Developer";
let i = 0;

function type() {
  if (i < text.length) {
    document.getElementById("typing").innerHTML += text.charAt(i);
    i++;
    setTimeout(type, 100);
  }
}
type();

// Dark mode toggle
document.getElementById("themeToggle").onclick = () => {
  document.body.classList.toggle("dark");
};

// Project filter
function filterProjects(type) {
  let projects = document.querySelectorAll(".project");
  projects.forEach(p => {
    if (type === "all" || p.classList.contains(type)) {
      p.style.display = "block";
    } else {
      p.style.display = "none";
    }
  });
}
## 📊 Stats
![Stats](https://github-readme-stats.vercel.app/api?username=your-username)
