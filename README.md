# Hackathon-Project-2025-Cohort
# portfolio project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Josphat Ndungu | Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <h1>Josphat Ndungu</h1>
        <p>Passionate developer specializing in dynamic and responsive interfaces.</p>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><button id="theme-toggle">🌙</button></li>
            </ul>
        </nav>
    </header>
    
    <section id="about">
        <h2>About Me</h2>
        <p>Experienced in HTML, CSS, databases, and front-end frameworks, creating seamless user experiences.</p>
    </section>
    
    <section id="projects">
        <h2>Projects</h2>
        <div id="project-list">
            <!-- Projects will be dynamically loaded here -->
        </div>
    </section>
    
    <section id="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML & CSS</li>
            <li>JavaScript & Frontend Frameworks</li>
            <li>Database Management (MySQL)</li>
            <li>Responsive Design</li>
        </ul>
    </section>
    
    <section id="testimonials">
        <h2>Testimonials</h2>
        <div id="testimonial-list">
            <!-- Testimonials will be dynamically loaded here -->
        </div>
    </section>
    
    <section id="contact">
        <h2>Contact Me</h2>
        <form action="contact.php" method="POST">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Send Message</button>
        </form>
    </section>
    
    <footer>
        <p>&copy; 2025 Josphat Ndungu. All Rights Reserved.</p>
    </footer>
    
    <script>
        // Fetch projects from the database using an API endpoint
        fetch('get_projects.php')
            .then(response => response.json())
            .then(data => {
                let projectList = document.getElementById('project-list');
                data.forEach(project => {
                    let projectDiv = document.createElement('div');
                    projectDiv.classList.add('project');
                    projectDiv.innerHTML = `<h3>${project.title}</h3><p>${project.description}</p>`;
                    projectList.appendChild(projectDiv);
                });
            })
            .catch(error => console.error('Error fetching projects:', error));
        
        // Fetch testimonials from the database
        fetch('get_testimonials.php')
            .then(response => response.json())
            .then(data => {
                let testimonialList = document.getElementById('testimonial-list');
                data.forEach(testimonial => {
                    let testimonialDiv = document.createElement('div');
                    testimonialDiv.classList.add('testimonial');
                    testimonialDiv.innerHTML = `<p>"${testimonial.message}"</p><h4>- ${testimonial.name}</h4>`;
                    testimonialList.appendChild(testimonialDiv);
                });
            })
            .catch(error => console.error('Error fetching testimonials:', error));
        
        // Theme toggle
        document.getElementById('theme-toggle').addEventListener('click', () => {
            document.body.classList.toggle('dark-mode');
        });
    </script>
</body>
</html>

# my portfolio website
file:///C:/Users/HP/Desktop/xampp/htdocs/portfolio/portfolio3.html

# # portfolio project2 with errors
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Josphat Ndungu | Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <h1>Josphat Ndungu</h1>
        <p>Passionate developer specializing in dynamic and responsive interfaces.</p>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><button id="theme-toggle">🌙</button></li>
            </ul>
        </nav>
    </header>
    
    <section id="about">
        <h2>About Me</h2>
        <p>Experienced in HTML, CSS, databases, and front-end frameworks, creating seamless user experiences.</p>
    </section>
    
    <section id="projects">
        <h2>Projects</h2>
        <div id="project-list">
            <!-- Projects will be dynamically loaded here -->
        </div>
    </section>
    
    <section id="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML & CSS</li>
            <li>JavaScript & Frontend Frameworks</li>
            <li>Database Management (MySQL)</li>
            <li>Responsive Design</li>
        </ul>
    </section>
    
    <section id="testimonials">
        <h2>Testimonials</h2>
        <div id="testimonial-list">
            <!-- Testimonials will be dynamically loaded here -->
        </div>
    </section>
    
    <section id="contact">
        <h2>Contact Me</h2>
        <form action="contact.php" method="POST">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Send Message</button>
        </form>
    </section>
    
    <footer>
        <p>&copy; 2025 Josphat Ndungu. All Rights Reserved.</p>
    </footer>
    
    <script>
        // Fetch projects from the database using an API endpoint
        fetch('get_projects.php')
            .then(response => response.json())
            .then(data => {
                let projectList = document.getElementById('project-list');
                data.forEach(project => {
                    let projectDiv = document.createElement('div');
                    projectDiv.classList.add('project');
                    projectDiv.innerHTML = `<h3>${project.title}</h3><p>${project.description}</p>`;
                    projectList.appendChild(projectDiv);
                });
            })
            .catch(error => console.error('Error fetching projects:', error));
        
        // Fetch testimonials from the database
        fetch('get_testimonials.php')
            .then(response => response.json())
            .then(data => {
                let testimonialList = document.getElementById('testimonial-list');
                data.forEach(testimonial => {
                    let testimonialDiv = document.createElement('div');
                    testimonialDiv.classList.add('testimonial');
                    testimonialDiv.innerHTML = `<p>"${testimonial.message}"</p><h4>- ${testimonial.name}</h4>`;
                    testimonialList.appendChild(testimonialDiv);
                });
            })
            .catch(error => console.error('Error fetching testimonials:', error));
        
        // Theme toggle
        document.getElementById('theme-toggle').addEventListener('click', () => {
            document.body.classList.toggle('dark-mode');
        });
    </script>
</body>
</html>

