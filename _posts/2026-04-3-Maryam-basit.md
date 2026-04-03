---
title: "CE journey"
date: 2026-04-3
categories: [Blogging, Programming]
tags: [pf, programming, engineering]
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="styles.css">
</head>

<body>

<header>
  <h1>Maryam Basit</h1>
  <p>Computer Engineering Student | Growth Through Challenges 🚀</p>
</header>

<nav>
  <a href="#journey">Journey</a>
  <a href="#projects">Projects</a>
  <a href="#skills">Skills</a>
  <a href="#posts">Posts</a>
  <a href="#contact">Contact</a>
</nav>

<section id="journey">
<h2>✨ My Journey</h2>
<div class="card">
<p>I started my journey from a pre-engineering background where coding was completely new. I faced confusion, errors, and difficulty in understanding syntax. Writing code on paper during exams was even more challenging.</p>
<p>But with consistency, practice, and patience, I improved my problem-solving skills and gained confidence.</p>
</div>
</section>

<section id="projects">
<h2>💻 Projects</h2>
<div class="grid">
<div class="card"><h3>Student Result System</h3><p>C# OOP-based project.</p></div>
<div class="card"><h3>Profit & Loss Calculator</h3><p>Business logic implementation.</p></div>
<div class="card"><h3>File Upload Page</h3><p>HTML GitHub upload system.</p></div>
</div>
</section>

<section id="skills">
<h2>🚀 Skills</h2>
<div class="card">
<p>C#</p>
<div class="progress"><div class="progress-bar" style="width:80%"></div></div>
<p>HTML</p>
<div class="progress"><div class="progress-bar" style="width:70%"></div></div>
<p>SQL</p>
<div class="progress"><div class="progress-bar" style="width:60%"></div></div>
</div>
</section>

<section id="posts">
<h2>📝 My Posts</h2>
<div class="card">
<input type="text" id="postTitle" placeholder="Post Title" style="width:100%;padding:10px;margin-bottom:10px;border-radius:10px;border:none;">
<textarea id="postContent" placeholder="Write your post here..." style="width:100%;padding:10px;border-radius:10px;border:none;"></textarea>
<br><br>
<button onclick="addPost()">Add Post</button>
</div>

<div id="postContainer"></div>
</section>

<section id="contact">
<h2>📩 Contact</h2>
<div class="card">
<p>Email: your-email@example.com</p>
</div>
</section>

<footer>
<p>© 2026 Maryam Basit | Keep Growing 💙</p>
</footer>

<script>
function addPost() {
  let title = document.getElementById('postTitle').value;
  let content = document.getElementById('postContent').value;

  if(title === '' || content === '') {
    alert('Please fill both fields');
    return;
  }

  let postDiv = document.createElement('div');
  postDiv.className = 'card';
  postDiv.innerHTML = `<h3>${title}</h3><p>${content}</p>`;

  document.getElementById('postContainer').prepend(postDiv);

  document.getElementById('postTitle').value = '';
  document.getElementById('postContent').value = '';
}
</script>

</body>
</html>


