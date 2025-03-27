<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile Intro</title>
    <style>
        /* CSS Styles */
        .github-intro {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 2rem;
            background-color: #0d1117;
            color: #c9d1d9;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .github-intro::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, #58a6ff, #8b949e, #58a6ff);
        }
        
        .intro-header {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
        }
        
        .avatar {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 3px solid #58a6ff;
            margin-right: 1.5rem;
            object-fit: cover;
        }
        
        .name {
            font-size: 2rem;
            margin: 0;
            color: #58a6ff;
        }
        
        .title {
            font-size: 1.2rem;
            margin: 0.5rem 0;
            color: #8b949e;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 0.5rem;
        }
        
        .social-link {
            color: #58a6ff;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .social-link:hover {
            color: #79c0ff;
            text-decoration: underline;
        }
        
        .intro-content {
            line-height: 1.6;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin: 1.5rem 0;
        }
        
        .tech-item {
            background-color: #161b22;
            color: #58a6ff;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: transform 0.3s, background-color 0.3s;
        }
        
        .tech-item:hover {
            transform: translateY(-3px);
            background-color: #1f2937;
        }
        
        .stats {
            display: flex;
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-number {
            font-size: 1.5rem;
            font-weight: bold;
            color: #58a6ff;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: #8b949e;
        }
        
        .typing-effect {
            min-height: 1.5em;
            border-right: 2px solid #58a6ff;
            animation: blink 1s step-end infinite;
        }
        
        @keyframes blink {
            from, to { border-color: transparent; }
            50% { border-color: #58a6ff; }
        }
        
        .quote {
            font-style: italic;
            margin: 1.5rem 0;
            padding: 1rem;
            background-color: #161b22;
            border-left: 3px solid #58a6ff;
        }
    </style>
</head>
<body>
    <div class="github-intro">
        <div class="intro-header">
            
            <div>
                <h1 class="name" id="username">Ashraful Islam Akash</h1>
                <p class="title" id="user-title">Developer</p>
                <div class="social-links">
                    <a href="https://github.com/Ashraful-akash467" class="social-link" target="_blank">GitHub</a>
                    <a href="https://www.facebook.com/ashraful.akash.151322" class="social-link" target="_blank">Facebook</a>
                    <a href="https://www.linkedin.com/in/ashraful-islam-akash-387906253/" class="social-link" target="_blank">LinkedIn</a>
                    <a href="https://twitter.com/yourusername" class="social-link" target="_blank">Twitter</a>
                    <a href="mailto:ashrafulakash467@gmail.com" class="social-link" target="_blank">Email</a>
                </div>
            </div>
        </div>
        
        <div class="intro-content">
            <p>Hello there! 👋 I'm <span id="dynamic-name">Ashraful Islam Akash</span>, a passionate <span class="typing-effect" id="typing-text"></span></p>
            
            <div class="quote" id="random-quote">
                "The only way to do great work is to love what you do."
            </div>
            
            <p>I specialize in building modern web applications with cutting-edge technologies.</p>
            
            <h3>🛠️ Tech Stack</h3>
            <div class="tech-stack" id="tech-stack">
                <!-- Will be populated by JavaScript -->
            </div>
            
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number" id="repo-count">0</div>
                    <div class="stat-label">Repositories</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number" id="star-count">0</div>
                    <div class="stat-label">Stars</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number" id="follower-count">0</div>
                    <div class="stat-label">Followers</div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // JavaScript for interactive elements
        document.addEventListener('DOMContentLoaded', function() {
            // Typing effect
            const typingText = document.getElementById('typing-text');
            const professions = ['Developer', 'Designer', 'Creator', 'Problem Solver', 'Tech Enthusiast'];
            let professionIndex = 0;
            let charIndex = 0;
            let isDeleting = false;
            
            function type() {
                const currentProfession = professions[professionIndex];
                
                if (isDeleting) {
                    typingText.textContent = currentProfession.substring(0, charIndex - 1);
                    charIndex--;
                } else {
                    typingText.textContent = currentProfession.substring(0, charIndex + 1);
                    charIndex++;
                }
                
                if (!isDeleting && charIndex === currentProfession.length) {
                    isDeleting = true;
                    setTimeout(type, 1500);
                } else if (isDeleting && charIndex === 0) {
                    isDeleting = false;
                    professionIndex = (professionIndex + 1) % professions.length;
                    setTimeout(type, 500);
                } else {
                    setTimeout(type, isDeleting ? 50 : 150);
                }
            }
            
            // Start typing effect after a short delay
            setTimeout(type, 1000);
            
            // Tech stack items
            const techStack = [
                'Python', 'CPP', 'C Programing', 'Java', 
                'HTML5', 'CSS', 'JavaScript', 'Git', 
                'Docker', 'Problem Solver', 'SQL', 'MongoDB'
            ];
            
            const techStackContainer = document.getElementById('tech-stack');
            techStack.forEach(tech => {
                const techItem = document.createElement('span');
                techItem.className = 'tech-item';
                techItem.textContent = tech;
                techStackContainer.appendChild(techItem);
            });
            
            // Animated counters
            function animateCounter(elementId, target, duration = 2000) {
                const element = document.getElementById(elementId);
                const start = 0;
                const increment = target / (duration / 16);
                let current = start;
                
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= target) {
                        clearInterval(timer);
                        current = target;
                    }
                    element.textContent = Math.floor(current);
                }, 16);
            }
            
            // Simulate some stats (replace with actual API calls to GitHub)
            animateCounter('repo-count', 8);
            animateCounter('star-count', );
            animateCounter('follower-count', );
            
            // Random quotes
            const quotes = [
                "The only way to do great work is to love what you do. - Steve Jobs",
                "First, solve the problem. Then, write the code. - John Johnson",
                "Any fool can write code that a computer can understand. Good programmers write code that humans can understand. - Martin Fowler",
                "Code is like humor. When you have to explain it, it's bad. - Cory House",
                "Make it work, make it right, make it fast. - Kent Beck"
            ];
            
            const quoteElement = document.getElementById('random-quote');
            quoteElement.textContent = quotes[Math.floor(Math.random() * quotes.length)];
            
            // You could replace this with actual GitHub API calls to get real data
            /*
            fetch('https://api.github.com/users/yourusername')
                .then(response => response.json())
                .then(data => {
                    document.getElementById('username').textContent = data.name || 'Your Name';
                    document.getElementById('profile-avatar').src = data.avatar_url;
                    document.getElementById('repo-count').textContent = data.public_repos;
                    // Add more data as needed
                });
            */
        });
    </script>
</body>
</html>
