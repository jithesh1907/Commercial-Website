# Ex02 Commercial Website
## Date:31/08/2026


## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML:
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TechNova Solutions</title>

<link rel="stylesheet" href="style.css">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

</head>
<body>

<header>

<nav>

<h2 class="logo">TechNova</h2>

<ul>

<li><a href="#home">Home</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#about">About</a></li>
<li><a href="#account">Account</a></li>
<li><a href="#contact">Contact</a></li>

</ul>

</nav>

</header>


<!-- HOME -->

<section id="home" class="hero">

<div class="hero-text">

<h1>Innovating Your Digital Future</h1>

<p>
TechNova Solutions delivers innovative software, cloud services,
and AI-powered business solutions to help companies grow.
</p>

<a href="#services" class="btn">Explore Services</a>

</div>

<div class="hero-image">

<img src="img.png" alt="TechNova Solutions">

</div>

</section>



<!-- SERVICES -->

<section id="services">

<h2>Our Services</h2>

<div class="cards">

<div class="card">

<img src="img2.png" alt="Web Development">

<h3>Web Development</h3>

<p>
Responsive websites and modern web applications built for businesses.
</p>

</div>

<div class="card">

<img src="img3.png" alt="Cloud Computing">

<h3>Cloud Solutions</h3>

<p>
Secure cloud infrastructure, migration, and maintenance services.
</p>

</div>

<div class="card">

<img src="img.png" alt="Artificial Intelligence">

<h3>AI Solutions</h3>

<p>
Machine learning, predictive analytics, and intelligent automation.
</p>

</div>

</div>

</section>



<!-- ABOUT -->

<section id="about">

<h2>About Us</h2>

<p>

Founded in 2026, TechNova Solutions specializes in digital
transformation, helping startups and enterprises leverage technology
to improve productivity, customer engagement, and business growth.

</p>

</section>



<!-- ACCOUNT -->

<section id="account">

<h2>User Account</h2>

<div class="account-box">

<form>

<input type="text" placeholder="Username">

<input type="email" placeholder="Email">

<input type="password" placeholder="Password">

<button>Login</button>

</form>

</div>

</section>



<!-- CONTACT -->

<section id="contact">

<h2>Contact Us</h2>

<p>📍 Chennai, India</p>

<p>📞 +91 99437 73848</p>


<p>✉ support@technova.com</p>

</section>



<!-- FOOTER -->

<footer>

<div class="social">

<a href="#">Facebook</a>

<a href="#">Instagram</a>

<a href="#">LinkedIn</a>

<a href="#">Twitter</a>

</div>
<p>Created by: Lakshiya Rajkumar | 212225240076</p>

<p>© 2026 TechNova Solutions. All Rights Reserved.</p>

</footer>

</body>
</html>
```
CSS:
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#f4f7fb;
    color:#333;
}

header{

    background:#a10d90;
    position:sticky;
    top:0;
    z-index:1000;

}

nav{

    width:90%;
    margin:auto;
    height:75px;

    display:flex;
    justify-content:space-between;
    align-items:center;

}

.logo{

    color:white;
    font-size:30px;

}

nav ul{

    display:flex;
    list-style:none;

}

nav ul li{

    margin-left:30px;

}

nav ul li a{

    color:white;
    text-decoration:none;
    font-weight:500;
    transition:.3s;

}

nav ul li a:hover{

    color:#FFD54F;

}

/* HERO */

.hero{

    width:90%;
    margin:auto;
    min-height:90vh;

    display:flex;
    justify-content:space-between;
    align-items:center;

}

.hero-text{

    width:50%;

}

.hero-text h1{

    font-size:55px;
    margin-bottom:20px;
    color:#950da1;

}

.hero-text p{

    font-size:18px;
    line-height:1.8;
    margin-bottom:30px;

}

.btn{

    display:inline-block;

    background:#0d47a1;
    color:white;

    text-decoration:none;

    padding:15px 35px;

    border-radius:40px;

    transition:.3s;

}

.btn:hover{

    background:#1565c0;

    transform:translateY(-5px);

}

.hero-image img{

    width:500px;
    border-radius:15px;
    box-shadow:0 15px 30px rgba(0,0,0,.2);

}

/* Sections */

section{

    padding:80px 10%;

}

section h2{

    text-align:center;
    margin-bottom:40px;
    font-size:40px;
    color:#a10d8d;

}

/* Cards */

.cards{

    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;

}

.card{

    width:320px;

    background:white;

    border-radius:15px;

    overflow:hidden;

    box-shadow:0 10px 20px rgba(0,0,0,.08);

    transition:.3s;

}

.card:hover{

    transform:translateY(-10px);

    box-shadow:0 20px 35px rgba(0,0,0,.15);

}

.card img{

    width:100%;
    height:200px;
    object-fit:cover;

}

.card h3{

    margin:20px;

}

.card p{

    margin:0 20px 20px;

}

/* Account */

.account-box{

    display:flex;
    justify-content:center;

}

form{

    width:350px;

    display:flex;
    flex-direction:column;

    gap:20px;

}

input{

    padding:15px;

    border:1px solid #ccc;

    border-radius:8px;

}

button{

    padding:15px;

    background:#ddb9db;

    color:white;

    border:none;

    border-radius:8px;

    cursor:pointer;

    transition:.3s;

}

button:hover{

    background:#1565c0;

}

/* Contact */

#contact{

    text-align:center;
    background:#e3f2fd;

}

#contact p{

    margin:10px;

}

/* Footer */

footer{

    background:#bd229e;

    color:white;

    text-align:center;

    padding:30px;

}

.social{

    display:flex;

    justify-content:center;

    gap:30px;

    margin-bottom:20px;

}

.social a{

    color:white;

    text-decoration:none;

    transition:.3s;

}

.social a:hover{

    color:#FFD54F;

}

/* Responsive */

@media(max-width:900px){

.hero{

    flex-direction:column-reverse;
    text-align:center;
    padding-top:40px;

}

.hero-text{

    width:100%;

}

.hero-image img{

    width:100%;
    max-width:400px;
    margin-bottom:40px;

}

nav{

    flex-direction:column;
    height:auto;
    padding:20px;

}

nav ul{

    margin-top:20px;
    flex-wrap:wrap;
    justify-content:center;

}

nav ul li{

    margin:10px;

}

}
```


## OUTPUT
<img width="947" height="441" alt="Screenshot 2026-07-29 134316" src="https://github.com/user-attachments/assets/71759656-d3ad-4cc5-975a-5f77927d0c03" />
<img width="949" height="433" alt="Screenshot 2026-07-29 134416" src="https://github.com/user-attachments/assets/1fde74ad-84c2-4281-bd1b-6650933fc7d2" />
<img width="946" height="440" alt="Screenshot 2026-07-29 134442" src="https://github.com/user-attachments/assets/5e39a8fa-8bd9-4711-9cbe-99d90d7c9893" />
<img width="950" height="357" alt="Screenshot 2026-07-29 134512" src="https://github.com/user-attachments/assets/f1ecc312-c87b-4aa7-af2f-279774a3fa5c" />
<img width="942" height="431" alt="Screenshot 2026-07-29 134537" src="https://github.com/user-attachments/assets/e3f9eef7-f74d-4d51-9414-1bcbf74eb4f6" />
<img width="941" height="434" alt="Screenshot 2026-07-29 134559" src="https://github.com/user-attachments/assets/bff14286-0720-4638-b345-12c7a3f95d30" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
