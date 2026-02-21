# heerendra-portfolio
Personal Portfolio Website
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Heerendra Sharma | Front-End Developer</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#ffffff;
    color:#111;
    line-height:1.6;
}

header{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

header h1{
    font-size:3rem;
    font-weight:700;
}

header h2{
    font-weight:400;
    margin:10px 0;
    color:#555;
}

header p{
    max-width:600px;
    margin:15px auto;
    color:#666;
}

.btn{
    display:inline-block;
    margin-top:20px;
    padding:12px 25px;
    background:#111;
    color:#fff;
    text-decoration:none;
    border-radius:30px;
    transition:0.3s;
}

.btn:hover{
    background:#444;
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
    background:#f5f5f5;
    padding:20px;
    border-radius:10px;
    transition:0.3s;
}

.card:hover{
    transform:translateY(-5px);
}

footer{
    text-align:center;
    padding:30px;
    background:#111;
    color:#fff;
}

@media(max-width:768px){
    header h1{
        font-size:2.2rem;
    }
}

</style>
</head>
<body>

<header>
    <h1>Heerendra Sharma</h1>
    <h2>Front-End Web Developer</h2>
    <p>Building responsive, high-performance and user-centric web experiences using modern web technologies.</p>
    <a href="#projects" class="btn">View Projects</a>
</header>

<section id="about">
    <h2 class="section-title">About Me</h2>
    <p style="text-align:center; max-width:800px; margin:auto;">
        Motivated Front-End Developer with strong foundations in HTML, CSS and JavaScript.
        Passionate about building responsive, scalable and performance-optimized web applications.
        Seeking an entry-level opportunity to contribute to impactful projects and grow professionally.
    </p>
</section>

<section id="skills">
    <h2 class="section-title">Technical Skills</h2>
    <div class="skills">
        <div class="card">
            <h3>Languages</h3>
            <p>HTML5, CSS3, JavaScript</p>
        </div>
        <div class="card">
            <h3>Concepts</h3>
            <p>Responsive Design, Flexbox, CSS Grid, Media Queries</p>
        </div>
        <div class="card">
            <h3>Tools</h3>
            <p>Git, GitHub, VS Code, Chrome DevTools</p>
        </div>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Projects</h2>
    <div class="projects">
        <div class="card">
            <h3>Advanced Responsive Portfolio</h3>
            <p>Mobile-first portfolio website with smooth UI and performance optimization.</p>
        </div>
        <div class="card">
            <h3>E-Commerce Web App</h3>
            <p>Product listing, filtering and dynamic cart functionality using JavaScript.</p>
        </div>
        <div class="card">
            <h3>Task Management App</h3>
            <p>CRUD-based To-Do application with Local Storage integration.</p>
        </div>
        <div class="card">
            <h3>Weather App</h3>
            <p>Integrated weather API using Fetch API to display real-time data.</p>
        </div>
        <div class="card">
            <h3>Landing Page Optimization</h3>
            <p>Conversion-focused responsive landing page with improved accessibility.</p>
        </div>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Contact</h2>
    <p style="text-align:center;">
        📍 Jaipur, Rajasthan <br>
        📞 +91 8905643678 <br>
        📧 Sharmaheerendracr7@gmail.com <br>
        🔗 linkedin.com/in/heerendra-sharma-0407143a6
    </p>
</section>

<footer>
    © 2026 Heerendra Sharma | All Rights Reserved
</footer>

</body>
</html>
