<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sahana P | Creative Portfolio</title>
<meta name="description" content="Sahana P Portfolio | B.Com Computer Applications Student | Web Development & Technology">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;scroll-behavior:smooth;}
body{background:#fdf8fc;color:#2d2d2d;overflow-x:hidden;}
#matrix{position:fixed;top:0;left:0;width:100%;height:100%;z-index:-10;opacity:.06;}
nav{position:fixed;top:0;left:0;width:100%;padding:18px 50px;display:flex;justify-content:space-between;align-items:center;background:rgba(255,255,255,.85);backdrop-filter:blur(18px);border-bottom:1px solid #f0e6f5;z-index:1000;}
.logo{font-size:24px;font-weight:700;background:linear-gradient(90deg,#ec4899,#8b5cf6);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
nav ul{display:flex;list-style:none;gap:28px;}
nav ul li a{text-decoration:none;color:#555;font-size:15px;font-weight:500;transition:.3s;position:relative;}
nav ul li a:hover{color:#ec4899;}
nav ul li a::after{content:'';position:absolute;bottom:-6px;left:0;width:0;height:2px;background:linear-gradient(90deg,#ec4899,#8b5cf6);transition:.3s;}
nav ul li a:hover::after{width:100%;}
.menu-btn{display:none;font-size:30px;cursor:pointer;color:#ec4899;z-index:1001;transition:.3s;}
.menu-btn:hover{transform:scale(1.1);}
.nav-backdrop{position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,.4);backdrop-filter:blur(4px);opacity:0;visibility:hidden;transition:.4s;z-index:998;}
.nav-backdrop.active{opacity:1;visibility:visible;}
.hero{height:100vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:20px;background:linear-gradient(135deg,rgba(236,72,153,.08),rgba(139,92,246,.08));}
.hero h1{font-size:4.5rem;font-weight:700;margin-bottom:10px;color:#2d2d2d;}
.hero h1 span{background:linear-gradient(90deg,#ec4899,#8b5cf6);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.typing{font-size:1.3rem;color:#8b5cf6;margin-bottom:25px;font-weight:500;}
.hero p{max-width:800px;line-height:1.9;color:#666;}
.hero-btn{margin-top:35px;padding:15px 35px;border-radius:50px;text-decoration:none;color:white;font-weight:600;background:linear-gradient(90deg,#ec4899,#8b5cf6);transition:.3s;display:inline-block;box-shadow:0 8px 20px rgba(236,72,153,.25);}
.hero-btn:hover{transform:translateY(-4px);box-shadow:0 12px 30px rgba(236,72,153,.35);}
section{padding:110px 60px;}
section h2{text-align:center;margin-bottom:50px;font-size:2.2rem;background:linear-gradient(90deg,#ec4899,#8b5cf6);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:25px;}
.card{background:rgba(255,255,255,.7);border:1px solid rgba(236,72,153,.1);padding:25px;border-radius:20px;transition:.4s;backdrop-filter:blur(10px);box-shadow:0 4px 15px rgba(236,72,153,.08);}
.card:hover{transform:translateY(-10px);border-color:#ec4899;box-shadow:0 10px 30px rgba(236,72,153,.15);}
.card h3{margin-bottom:10px;color:#ec4899;}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:20px;}
.stat-box{background:#fff;padding:25px;border-radius:18px;text-align:center;border:1px solid #f0e6f5;box-shadow:0 4px 15px rgba(236,72,153,.05);}
.stat-box h3{font-size:2rem;color:#ec4899;}
.stat-box p{color:#777;margin-top:10px;}
.service-tag{display:inline-block;padding:5px 12px;border-radius:20px;background:rgba(236,72,153,.1);border:1px solid #ec4899;color:#ec4899;font-size:12px;margin-bottom:15px;font-weight:500;}

.contact-box{max-width:700px;margin:auto;}
.contact-cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px;margin-bottom:30px;}
.contact-card{background:rgba(255,255,255,.8);border:1px solid rgba(236,72,153,.1);backdrop-filter:blur(15px);padding:20px;border-radius:18px;text-align:center;transition:.4s;text-decoration:none;color:#333;box-shadow:0 4px 15px rgba(236,72,153,.05);}
.contact-card:hover{transform:translateY(-8px);border-color:#ec4899;box-shadow:0 10px 25px rgba(236,72,153,.2);}
.contact-card h3{color:#ec4899;margin-bottom:10px;}
.contact-card p{color:#666;font-size:14px;word-break:break-word;}
.contact input,.contact textarea{width:100%;padding:15px;margin:10px 0;background:#fff;border:1px solid #f0e6f5;color:#333;border-radius:12px;outline:none;}
.contact input:focus,.contact textarea:focus{border-color:#ec4899;box-shadow:0 0 0 3px rgba(236,72,153,.1);}
.btn{width:100%;padding:15px;border:none;border-radius:50px;font-weight:600;cursor:pointer;background:linear-gradient(90deg,#ec4899,#8b5cf6);color:white;box-shadow:0 8px 20px rgba(236,72,153,.25);}
.btn:hover{opacity:.9;transform:translateY(-2px);}
.whatsapp-float{position:fixed;bottom:25px;right:25px;width:60px;height:60px;background:#25D366;color:white;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:28px;text-decoration:none;box-shadow:0 0 20px rgba(37,211,102,.5);z-index:9999;}
footer{padding:40px;text-align:center;border-top:1px solid #f0e6f5;color:#888;display:flex;flex-direction:column;align-items:center;justify-content:center;width:100%;margin:0 auto;background:#fff;}
.hidden{opacity:0;transform:translateY(50px);transition:.7s;}
.show{opacity:1;transform:translateY(0);}
.timeline{position:relative;max-width:900px;margin:auto;}
.timeline::after{content:'';position:absolute;width:4px;background:linear-gradient(#ec4899,#8b5cf6);top:0;bottom:0;left:50%;margin-left:-2px;border-radius:10px;}
.timeline-item{padding:10px 40px;position:relative;width:50%;}
.timeline-item::after{content:'';position:absolute;width:22px;height:22px;right:-11px;background:#ec4899;border:4px solid #8b5cf6;top:25px;border-radius:50%;z-index:1;box-shadow:0 0 20px rgba(236,72,153,.5);}
.left{left:0;}
.right{left:50%;}
.right::after{left:-11px;}
.timeline-content{padding:25px;background:rgba(255,255,255,.8);border:1px solid rgba(236,72,153,.1);border-radius:18px;backdrop-filter:blur(12px);transition:.4s;box-shadow:0 4px 15px rgba(236,72,153,.05);}
.timeline-content:hover{transform:translateY(-8px);box-shadow:0 10px 25px rgba(236,72,153,.15);}
.timeline-content h3{color:#ec4899;margin-bottom:10px;}
.skill-bar{width:100%;height:12px;background:#f0e6f5;border-radius:20px;overflow:hidden;margin:15px 0;}
.skill-fill{height:100%;background:linear-gradient(90deg,#ec4899,#8b5cf6);border-radius:20px;display:block;animation:fillBar 2s ease;}
@keyframes fillBar{from{width:0;}}
.cursor-glow{position:fixed;width:250px;height:250px;background:radial-gradient(circle,rgba(236,72,153,.12),transparent 70%);pointer-events:none;border-radius:50%;transform:translate(-50%,-50%);z-index:-1;}

/* MOBILE FIXES */
@media(max-width:1024px){
.menu-btn{display:block;}
nav{padding:15px 20px;}
nav ul{position:fixed;top:0;right:-320px;width:320px;height:100vh;background:rgba(255,255,255,.98);backdrop-filter:blur(20px);flex-direction:column;text-align:left;padding:100px 30px 40px;border-left:1px solid #f0e6f5;transition:right.4s cubic-bezier(0.4, 0, 0.2, 1);z-index:999;gap:5px;display:flex;}
nav ul.active{right:0;}
nav ul li{margin:0;width:100%;}
nav ul li a{display:block;padding:16px 20px;font-size:16px;border-radius:12px;border:1px solid transparent;}
nav ul li a:hover{background:rgba(236,72,153,.08);border-color:rgba(236,72,153,.2);color:#ec4899;}
nav ul li a::after{display:none;}
body.menu-open{overflow:hidden;}
}
@media(max-width:768px){
.timeline::after{left:20px;}
.timeline-item{width:100%;padding-left:60px;padding-right:15px;}
.left,.right{left:0;}
.timeline-item::after{left:9px;}
.hero h1{font-size:3rem;}
section{padding:80px 20px;}
nav ul{width:280px;right:-280px;}
}
@media(max-width:480px){
nav ul{width:100%;right:-100%;}
}
</style>
</head>
<body>
<canvas id="matrix"></canvas>
<div class="nav-backdrop" onclick="toggleMenu()"></div>
<nav>
<div class="logo">SAHANA P</div>
<div class="menu-btn" onclick="toggleMenu()">☰</div>
<ul id="navLinks">
<li><a href="#home" onclick="closeMenu()">🏠 Home</a></li>
<li><a href="#about" onclick="closeMenu()">👩‍💻 About</a></li>
<li><a href="#skills" onclick="closeMenu()">⚡ Skills</a></li>
<li><a href="#projects" onclick="closeMenu()">💼 Projects</a></li>
<li><a href="#education" onclick="closeMenu()">🎓 Education</a></li>
<li><a href="#timeline" onclick="closeMenu()">📈 Timeline</a></li>
<li><a href="#services" onclick="closeMenu()">🛠️ Services</a></li>
<li><a href="#contact" onclick="closeMenu()">📧 Contact</a></li>
</ul>
</nav>

<section class="hero" id="home">
<h1>Hi, I'm <span>Sahana</span></h1>
<div class="typing" id="typing"></div>
<p>B.Com Computer Applications Student at SASTRA University. Passionate about modern web technologies, creative design, automation and building elegant digital experiences.</p>
<a href="#contact" class="hero-btn">Let's Connect</a>
<br><br>
<a href="https://www.instagram.com/sahanapannerselvam?igsh=YXE1NjdkcHEzZ2c=" target="_blank" class="hero-btn" style="background:linear-gradient(90deg,#E1306C,#F77737);">View Instagram Profile</a>
</section>

<section id="about" class="hidden"><h2>About Me</h2><div class="card"><p style="line-height:1.9;color:#555;"> I am currently pursuing B.Com Computer Applications at SASTRA University, Thanjavur. My interests include web development, creative design, technology, automation and digital solutions. I enjoy building modern and aesthetic websites while continuously improving my technical skills through hands-on projects.</p></div></section>

<section id="skills" class="hidden"><h2>Skills</h2>
<div class="card"><h3>HTML & CSS</h3><div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div><p>90%</p></div>
<div class="card"><h3>JavaScript</h3><div class="skill-bar"><div class="skill-fill" style="width:75%"></div></div><p>75%</p></div>
<div class="card"><h3>C++ Programming</h3><div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div><p>80%</p></div>
<div class="card"><h3>Computer Applications</h3><div class="skill-bar"><div class="skill-fill" style="width:85%"></div></div><p>85%</p></div>
</section>

<section class="hidden"><h2>Overview</h2><div class="stats">
<div class="stat-box"><h3>2025</h3><p>Portfolio Started</p></div>
<div class="stat-box"><h3>10+</h3><p>Projects Planned</p></div>
<div class="stat-box"><h3>24/7</h3><p>Learning Mode</p></div>
<div class="stat-box"><h3>∞</h3><p>Growth Mindset</p></div>
</div></section>

<section id="projects" class="hidden"><h2>Projects</h2><div class="grid">
<div class="card"><h3>Personal Portfolio</h3><p>Professional portfolio website hosted using GitHub Pages with custom domain integration.</p></div>
<div class="card"><h3>Web Development Journey</h3><p>Collection of HTML, CSS and JavaScript practice projects.</p></div>
<div class="card"><h3>Future web Projects</h3><p>Exploring scalable software and digital business solutions.</p></div>
</div></section>

<section id="education" class="hidden"><h2>Education</h2><div class="card"><h3>B.Com Computer Applications</h3><p style="margin-top:10px;color:#555;">SASTRA Deemed University<br>Thanjavur, Tamil Nadu</p></div></section>

<section id="timeline" class="hidden"><h2>My Journey</h2><div class="timeline">
<div class="timeline-item left"><div class="timeline-content"><h3>🎂 2008</h3><p>Born on 3/4/2008. The beginning of a journey driven by creativity, learning and ambition.</p></div></div>
<div class="timeline-item right"><div class="timeline-content"><h3>📚 2023</h3><p>Completed SSLC with 65%.</p></div></div>
<div class="timeline-item left"><div class="timeline-content"><h3>🏆 2025</h3><p>Completed Higher Secondary Education (HSC) with 85%.</p></div></div>
<div class="timeline-item right"><div class="timeline-content"><h3>🎓 2026 - Present</h3><p>Currently pursuing B.Com (Computer Applications) at SASTRA Deemed University, Thanjavur. Focused on technology, business applications and web development.</p></div></div>
<div class="timeline-item left"><div class="timeline-content"><h3>🚀 Future Vision</h3><p>Aspiring to become a skilled technology professional, web developer and entrepreneur while creating innovative digital solutions.</p></div></div>
</div></section>

<section id="services" class="hidden"><h2>Services</h2><div class="grid">
<div class="card"><span class="service-tag">Available</span><h3>🌐 Website Creation</h3><p>Professional websites for students and businesses.</p></div>
<div class="card"><span class="service-tag">Available</span><h3>🎓 Student Portfolio Websites</h3><p>Personal portfolio websites for students to showcase skills, education, achievements and projects.</p></div>
<div class="card"><span class="service-tag">Available</span><h3>📚 College Project Websites</h3><p>Custom websites and front-end project development for academic presentations and submissions.</p></div>
<div class="card"><span class="service-tag">Available</span><h3>🏢 Small Business Websites</h3><p>Business websites with service details, contact forms, WhatsApp integration and branding.</p></div>
<div class="card"><span class="service-tag">Available</span><h3>🚀 Landing Pages</h3><p>High-converting landing pages for products, events, promotions and marketing campaigns.</p></div>
<div class="card"><span class="service-tag">Available</span><h3>🎬 Photo & Video Editing</h3><p>Professional photo enhancement, social media creatives and video editing services.</p></div>
</div>
<div style="text-align:center;margin-top:40px;"><a href="https://wa.me/916374955703" target="_blank" class="hero-btn">Request a Service</a></div></section>

<section id="contact" class="hidden contact"><h2>Contact</h2><div class="contact-box">
<div class="contact-cards">
<a href="mailto:Sahanaspace9@gmail.com" class="contact-card"><h3>📧 Email</h3><p>Sahanaspace9@gmail.com</p></a>
<a href="https://www.instagram.com/sahanapannerselvam?igsh=YXE1NjdkcHEzZ2c=" target="_blank" class="contact-card"><h3>📷 Instagram</h3><p>@sahanapannerselvam</p></a>
<a href="https://wa.me/916374955703" target="_blank" class="contact-card"><h3>📱 WhatsApp</h3><p>+91 63749 55703</p></a>
</div>
<form action="https://formspree.io/f/mnjeqjvk" method="POST">
<input type="text" name="name" placeholder="Your name " required>
<input type="email" name="email" placeholder="Your Email" required>
<textarea name="message" rows="5" placeholder="Your Message" required></textarea>
<button class="btn">Send Message</button>
</form>
</div></section>

<footer style="text-align:center;width:100%;"><div>
<h3 style="color:#ec4899;">SAHANA P</h3><br>
<p>B.Com Computer Applications</p><p>SASTRA University</p><br>
<p>© 2026 All Rights Reserved</p>
</div></footer>

<a href="https://wa.me/916374955703" target="_blank" class="whatsapp-float">💬</a>
<div class="cursor-glow"></div>

<script>
/* TYPING EFFECT */
const words=["Web Developer","Creative Designer","Tech Enthusiast","Future Software Builder"];
let i=0;let j=0;
function type(){const typing=document.getElementById("typing");if(j<words[i].length){typing.innerHTML+=words[i].charAt(j);j++;setTimeout(type,80);}else{setTimeout(()=>{typing.innerHTML="";j=0;i=(i+1)%words.length;type();},1500);}}
type();

/* SCROLL ANIMATION */
const observer=new IntersectionObserver(entries=>{entries.forEach(entry=>{if(entry.isIntersecting){entry.target.classList.add("show");}});});
document.querySelectorAll(".hidden").forEach(el=>observer.observe(el));

/* MATRIX EFFECT */
const canvas=document.getElementById("matrix");const ctx=canvas.getContext("2d");
function resizeCanvas(){canvas.width=window.innerWidth;canvas.height=window.innerHeight;}
resizeCanvas();
const letters="ABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890{}[]<>#$%&";const fontSize=14;let columns=canvas.width/fontSize;let drops=[];
function initDrops(){columns=Math.floor(canvas.width/fontSize);drops=[];for(let x=0;x<columns;x++){drops[x]=1;}}
initDrops();
function draw(){ctx.fillStyle="rgba(253,248,252,0.08)";ctx.fillRect(0,0,canvas.width,canvas.height);ctx.fillStyle="#ec4899";ctx.font=fontSize+"px monospace";for(let i=0;i<drops.length;i++){const text=letters.charAt(Math.floor(Math.random()*letters.length));ctx.fillText(text,i*fontSize,drops[i]*fontSize);if(drops[i]*fontSize>canvas.height&&Math.random()>0.975){drops[i]=0;}drops[i]++;}}
setInterval(draw,35);
window.addEventListener("resize",()=>{resizeCanvas();initDrops();});

/* MENU */
function toggleMenu(){const nav=document.getElementById("navLinks");const btn=document.querySelector(".menu-btn");const backdrop=document.querySelector(".nav-backdrop");const body=document.body;nav.classList.toggle("active");backdrop.classList.toggle("active");body.classList.toggle("menu-open");btn.innerHTML=nav.classList.contains("active")?"✕":"☰";}
function closeMenu(){const nav=document.getElementById("navLinks");const btn=document.querySelector(".menu-btn");const backdrop=document.querySelector(".nav-backdrop");const body=document.body;nav.classList.remove("active");backdrop.classList.remove("active");body.classList.remove("menu-open");btn.innerHTML="☰";}

const glow=document.querySelector(".cursor-glow");
document.addEventListener("mousemove",(e)=>{glow.style.left=e.clientX+"px";glow.style.top=e.clientY+"px";});
</script>
</body>
</html>
