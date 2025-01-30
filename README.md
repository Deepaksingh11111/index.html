<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
</head>
<body>
    <header>
        <div class="profile">
            <h1>Deepak Singh</h1>
            <img src="C:\Users\DELL\OneDrive\Desktop\portfolio\deepaksinghmahalwar.jpg" alt="My Photo" class="profile-pic">
            <p>Web Developer | Designer | Creator</p>
            <h2>For more information click on the sections given below.</h2>
        </div>
    </header>
    
    <nav>
        <ul>
            <li><a href="#" class="toggle-section" data-target="about">About Me</a></li>
            <li><a href="#" class="toggle-section" data-target="education">Education</a></li>
            <li><a href="#" class="toggle-section" data-target="projects">Projects</a></li>
            <li><a href="#" class="toggle-section" data-target="skills">Skills</a></li>
            <li><a href="#" class="toggle-section" data-target="contact">Contact</a></li>
        </ul>
    </nav>
    
    <section id="about" class="toggle-content">
        <h2>About Me</h2>
        <p>My name is Deepak Singh. I am passionate about web development and design, always eager to learn new technologies and improve my skills. Welcome to my portfolio!</p>
    </section>
    
    <section id="education" class="toggle-content">
        <h2>Education</h2>
        <table border="1" style="width:100%; text-align:center;">
            <tr>
                <th>Qualification</th>
                <th>Board</th>
                <th>Percentage</th>
            </tr>
            <tr>
                <td>12th</td>
                <td>CBSE</td>
                <td>63.2%</td>
            </tr>
            <tr>
                <td>10th</td>
                <td>CBSE</td>
                <td>77.8%</td>
            </tr>
        </table>
    </section>
    
    <section id="projects" class="toggle-content">
        <h2>Projects</h2>
        <ul>
            <li><strong>Chat GPT Model:</strong> Developed a Chat GPT model using Python with the help of Bolt IoT trainings with IIT Kanpur in AI to enable AI-driven conversational interactions.</li>
            <li><strong>Calculator:</strong> A simple calculator built using HTML, CSS, and JavaScript to perform basic arithmetic operations.</li>
            <li><strong>Calculator in C:</strong> Created a calculator program in C to perform arithmetic operations efficiently.</li>
        </ul>
    </section>
    
    <section id="skills" class="toggle-content">
        <h2>Skills</h2>
        <ul class="skills-list">
            <li>HTML</li>
            <li>JavaScript</li>
            <li>CSS</li>
            <li>C</li>
        </ul>
    </section>

    <section id="contact" class="toggle-content">
        <h2>Contact Info</h2>
        <p><strong>Phone:</strong> +91 6398267378</p>
        <p><strong>Instagram:</strong> <a href="https://www.instagram.com/deepaksinghmahalwar/profilecard/?igsh=bnQyeTg1YTE3bHJ4" target="_blank">@deepaksinghmahalwar</a></p>
        <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/deepak-singh-04b645333?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">@DeepakSingh</a></p>
        <p><strong>Moj:</strong> <a href="https://mojapp.in/@chaudharysahab1?referrer=UbGBmWS-tD7515" target="_blank">@chaudharysahab1</a></p>
        <p><strong>Email:</strong> deepaksinghmahalwar.2021@gmail.com</p>
    </section>

    <footer>
        <p>&copy; 2025 Deepak Singh. All rights reserved.</p>
    </footer>

    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(120deg, #a1c4fd, #c2e9fb);
        }

        .profile {
            margin-top: 50px;
        }

        /* Resized image to passport size */
        .profile-pic {
            width: 120px;  /* Passport size */
            height: 120px; /* Keep it square */
            border-radius: 10px; /* Slightly rounded edges */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .skills-list {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .skills-list li {
            font-size: 1.2em;
            font-weight: bold;
            color: #333;
            background: #fff;
            padding: 10px 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .toggle-content {
            display: none;
            margin-top: 30px;
        }

        .toggle-content.show {
            display: block;
        }

        .toggle-section {
            font-size: 1.2em;
            cursor: pointer;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 5px;
            color: #333;
            background-color: #f0f0f0;
            margin: 10px 0;
            display: inline-block;
        }

        .toggle-section:hover {
            background-color: #ddd;
        }

        .active {
            background-color: #a1c4fd;
            color: white;
        }

        nav ul {
            padding: 0;
            list-style: none;
            text-align: center;
        }

        nav ul li {
            display: inline-block;
            margin: 0 20px;
        }

        nav ul li a {
            text-decoration: none;
            padding: 10px;
            font-size: 1.2em;
            transition: background-color 0.3s ease;
        }

        nav ul li a:hover {
            background-color: #ddd;
        }
    </style>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const sections = document.querySelectorAll('.toggle-content');
            const links = document.querySelectorAll('.toggle-section');

            links.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const targetSection = document.getElementById(this.getAttribute('data-target'));
                    targetSection.classList.toggle('show');
                    this.classList.toggle('active');
                });
            });

            sections.forEach(section => {
                section.classList.remove('show');
            });
        });
    </script>
</body>
</html> 
