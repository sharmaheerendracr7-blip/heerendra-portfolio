<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Heerendra Sharma | Front-End Developer</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>

:root{
    --bg:#ffffff;
    --text:#111;
    --card:#f3f3f3;
}

body.dark{
    --bg:#0f172a;
    --text:#f1f5f9;
    --card:#1e293b;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:var(--bg);
    color:var(--text);
    transition:0.3s;
}

header{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
    animation:fadeIn 1.2s ease-in-out;
}

header h1{
    font-size:3rem;
    font-weight:700;
}

header h2{
    margin:10px 0;
    color:gray;
}

.btn{
    margin-top:15px;
    padding:12px 25px;
    background:#111;
    color:#fff;
    text-decoration:none;
    border-radius:30px;
    transition:0.3s;
    display:inline-block;
}

.btn:hover{
    opacity:0.8;
}

.toggle{
    position:fixed;
    top:20px;
    right:20px;
    cursor:pointer;
    font-size:14px;
    padding:8px 15px;
    background:#111;
    color:#fff;
    border-radius:20px;
}

section{
    padding:70px 10%;
}

.section-title{
    text-align:center;
    margin-bottom:40px;
    font-size:2rem;
}

.skills, .projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    background:var(--card);
    padding:20px;
    border-radius:10px;
    transition:0.3s;
    opacity:0;
    transform:translateY(20px);
}

.card.show{
    opacity:1;
    transform:translateY(0);
}

footer{
    text-align:center;
    padding:30px;
    background:#111;
    color:#fff;
}

@keyframes fadeIn{
    from{opacity:0;}
    to{opacity:1;}
}

</style>
</head>
<body>

<div class="toggle" onclick="toggleMode()">Dark Mode</div>

<header>
    <h1>Heerendra Sharma</h1>
    <h2>Front-End Web Developer</h2>
    <p>Building responsive, high-performance and user-centric web experiences.</p>
    <a href="#projects" class="btn">View Projects</a>
    <a href="Heerendra_Sharma_ATS_Resume_Final.pdf" class="btn" download>Download Resume</a>
</header>

<section>
    <h2 class="section-title">Technical Skills</h2>
    <div class="skills">
        <div class="card"><h3>Languages</h3><p>HTML5, CSS3, JavaScript</p></div>
        <div class="card"><h3>Concepts</h3><p>Responsive Design, Flexbox, CSS Grid</p></div>
        <div class="card"><h3>Tools</h3><p>Git, GitHub, VS Code</p></div>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Projects</h2>
    <div class="projects">
        <div class="card"><h3>Portfolio Website</h3><p>Fully responsive personal portfolio.</p></div>
        <div class="card"><h3>E-Commerce Web App</h3><p>Dynamic cart & product filtering.</p></div>
        <div class="card"><h3>Task Management App</h3><p>CRUD + Local Storage integration.</p></div>
        <div class="card"><h3>Weather App</h3><p>API integration using Fetch API.</p></div>
        <div class="card"><h3>Landing Page Optimization</h3><p>Conversion-focused UI design.</p></div>
    </div>
</section>

<section>
    <h2 class="section-title">Contact</h2>
    <p style="text-align:center;">
        Jaipur, Rajasthan <br>
        +91 8905643678 <br>
        Sharmaheerendracr7@gmail.com <br>
        linkedin.com/in/heerendra-sharma-0407143a6
    </p>
</section>

<footer>
    © 2026 Heerendra Sharma | All Rights Reserved
</footer>

<script>

function toggleMode(){
    document.body.classList.toggle("dark");
}

const cards = document.querySelectorAll(".card");

window.addEventListener("scroll", ()=>{
    cards.forEach(card=>{
        const cardTop = card.getBoundingClientRect().top;
        if(cardTop < window.innerHeight - 50){
            card.classList.add("show");
        }
    });
});

</script>

</body>
</html> 