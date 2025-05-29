<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cosmic Explorer GitHub Theme</title>
    <style>
        :root {
            --space-dark: #0a0e17;
            --nebula-purple: #6a00ff;
            --cyber-blue: #00e5ff;
            --matrix-green: #00ff9d;
            --starlight: #ffffff;
            --warp-speed: #ff00e5;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--space-dark);
            color: var(--starlight);
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(106, 0, 255, 0.1) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(0, 229, 255, 0.1) 0%, transparent 20%),
                linear-gradient(to bottom, transparent, var(--space-dark));
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .star {
            position: absolute;
            background-color: white;
            border-radius: 50%;
            animation: twinkle var(--duration, 5s) infinite ease-in-out;
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 0.2; }
            50% { opacity: 1; }
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        header {
            text-align: center;
            padding: 3rem 0;
            position: relative;
            border-bottom: 1px solid rgba(0, 229, 255, 0.3);
            margin-bottom: 3rem;
        }
        
        .hologram {
            width: 150px;
            height: 150px;
            background: linear-gradient(135deg, var(--cyber-blue), var(--nebula-purple));
            border-radius: 50%;
            margin: 0 auto 1.5rem;
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 30px var(--cyber-blue);
            animation: rotate 15s linear infinite;
        }
        
        .hologram::before {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, transparent 30%, rgba(0, 229, 255, 0.3) 100%);
            animation: pulse 4s infinite alternate;
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        @keyframes pulse {
            0% { transform: scale(0.8); opacity: 0.3; }
            100% { transform: scale(1.2); opacity: 0.6; }
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            background: linear-gradient(90deg, var(--cyber-blue), var(--matrix-green));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-transform: uppercase;
            letter-spacing: 3px;
            position: relative;
            display: inline-block;
        }
        
        h1::after {
            content: "";
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, var(--cyber-blue), var(--matrix-green));
            border-radius: 3px;
        }
        
        .tagline {
            font-size: 1.2rem;
            color: var(--cyber-blue);
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.6;
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }
        
        .card {
            background: rgba(10, 15, 30, 0.7);
            border: 1px solid rgba(0, 229, 255, 0.2);
            border-radius: 10px;
            padding: 2rem;
            backdrop-filter: blur(10px);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0, 229, 255, 0.2);
            border-color: var(--cyber-blue);
        }
        
        .card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: linear-gradient(to bottom, var(--cyber-blue), var(--matrix-green));
        }
        
        .card h2 {
            color: var(--matrix-green);
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
        }
        
        .card h2 i {
            margin-right: 10px;
            color: var(--cyber-blue);
        }
        
        .stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
            margin-top: 2rem;
        }
        
        .stat {
            background: rgba(0, 0, 0, 0.3);
            padding: 1rem;
            border-radius: 5px;
            text-align: center;
        }
        
        .stat-value {
            font-size: 2rem;
            font-weight: bold;
            color: var(--cyber-blue);
            margin-bottom: 0.5rem;
        }
        
        .stat-label {
            color: var(--starlight);
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .repo-list {
            list-style: none;
        }
        
        .repo-item {
            padding: 1rem 0;
            border-bottom: 1px solid rgba(0, 229, 255, 0.1);
        }
        
        .repo-item:last-child {
            border-bottom: none;
        }
        
        .repo-title {
            color: var(--cyber-blue);
            display: block;
            margin-bottom: 0.5rem;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }
        
        .repo-title:hover {
            color: var(--matrix-green);
        }
        
        .repo-desc {
            font-size: 0.9rem;
            opacity: 0.9;
            margin-bottom: 0.5rem;
        }
        
        .repo-meta {
            display: flex;
            gap: 1rem;
            font-size: 0.8rem;
            color: var(--matrix-green);
        }
        
        .terminal {
            background: rgba(0, 0, 0, 0.7);
            border-radius: 5px;
            padding: 1.5rem;
            font-family: 'Courier New', monospace;
            font-size: 0.9rem;
            line-height: 1.6;
            position: relative;
            overflow: hidden;
        }
        
        .terminal-header {
            display: flex;
            align-items: center;
            margin-bottom: 1rem;
        }
        
        .terminal-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            margin-right: 5px;
        }
        
        .terminal-dot.red { background: #ff5f56; }
        .terminal-dot.yellow { background: #ffbd2e; }
        .terminal-dot.green { background: #27c93f; }
        
        .terminal-content {
            color: var(--matrix-green);
        }
        
        .terminal-content .command {
            color: var(--cyber-blue);
        }
        
        .terminal-content .output {
            display: block;
            margin-top: 0.5rem;
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            margin-top: 1.5rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
            color: var(--starlight);
            transition: color 0.3s ease;
            padding: 0.5rem;
            border-radius: 5px;
        }
        
        .contact-item:hover {
            background: rgba(0, 229, 255, 0.1);
            color: var(--cyber-blue);
        }
        
        .contact-icon {
            font-size: 1.5rem;
            color: var(--matrix-green);
        }
        
        footer {
            text-align: center;
            padding: 3rem 0 2rem;
            margin-top: 3rem;
            border-top: 1px solid rgba(0, 229, 255, 0.3);
            color: var(--cyber-blue);
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Animated stars background -->
    <div class="stars" id="stars"></div>
    
    <div class="container">
        <header>
            <div class="hologram"></div>
            <h1>Cosmic Explorer</h1>
            <p class="tagline">Navigating the quantum realm of code and creating digital constellations in the GitHub universe</p>
        </header>
        
        <div class="grid">
            <!-- Stats Card -->
            <div class="card">
                <h2><i class="fas fa-chart-network"></i> Galactic Stats</h2>
                <div class="stats">
                    <div class="stat">
                        <div class="stat-value">42</div>
                        <div class="stat-label">Repositories</div>
                    </div>
                    <div class="stat">
                        <div class="stat-value">12</div>
                        <div class="stat-label">Projects</div>
                    </div>
                    <div class="stat">
                        <div class="stat-value">1.2K</div>
                        <div class="stat-label">Commits</div>
                    </div>
                    <div class="stat">
                        <div class="stat-value">89</div>
                        <div class="stat-label">Stars</div>
                    </div>
                </div>
            </div>
            
            <!-- Repositories Card -->
            <div class="card">
                <h2><i class="fas fa-starship"></i> Stellar Projects</h2>
                <ul class="repo-list">
                    <li class="repo-item">
                        <a href="#" class="repo-title">quantum-computing-framework</a>
                        <p class="repo-desc">A framework for simulating quantum algorithms in a distributed environment</p>
                        <div class="repo-meta">
                            <span>★ 24</span>
                            <span>JavaScript</span>
                        </div>
                    </li>
                    <li class="repo-item">
                        <a href="#" class="repo-title">neural-stellar-navigation</a>
                        <p class="repo-desc">AI-powered space navigation system using neural networks</p>
                        <div class="repo-meta">
                            <span>★ 36</span>
                            <span>Python</span>
                        </div>
                    </li>
                    <li class="repo-item">
                        <a href="#" class="repo-title">cyberpunk-ui-framework</a>
                        <p class="repo-desc">A futuristic UI component library for web applications</p>
                        <div class="repo-meta">
                            <span>★ 18</span>
                            <span>TypeScript</span>
                        </div>
                    </li>
                </ul>
            </div>
            
            <!-- Terminal Card -->
            <div class="card">
                <h2><i class="fas fa-terminal"></i> Command Center</h2>
                <div class="terminal">
                    <div class="terminal-header">
                        <div class="terminal-dot red"></div>
                        <div class="terminal-dot yellow"></div>
                        <div class="terminal-dot green"></div>
                    </div>
                    <div class="terminal-content">
                        <span class="command">$ git status</span>
                        <span class="output">On branch main: Quantum Computing Module</span>
                        <br>
                        <span class="command">$ git commit -am "Warp drive optimization"</span>
                        <span class="output">[main 0f3d7a2] Warp drive optimization</span>
                        <span class="output">3 files changed, 42 insertions(+)</span>
                        <br>
                        <span class="command">$ git push origin main</span>
                        <span class="output">Enumerating objects: 7, done.</span>
                        <span class="output">Delta compression using up to 8 cores</span>
                        <span class="output">Compressing objects: 100% (5/5), done.</span>
                        <span class="output">Writing objects: 100% (5/5), 1.42 KiB | 1.42 MiB/s, done.</span>
                    </div>
                </div>
            </div>
            
            <!-- Contact Card -->
            <div class="card">
                <h2><i class="fas fa-satellite"></i> Transmissions</h2>
                <p>Connect through the interstellar network:</p>
                <div class="contact-grid">
                    <a href="#" class="contact-item">
                        <i class="fas fa-envelope contact-icon"></i>
                        <span>Email</span>
                    </a>
                    <a href="#" class="contact-item">
                        <i class="fab fa-github contact-icon"></i>
                        <span>GitHub</span>
                    </a>
                    <a href="#" class="contact-item">
                        <i class="fab fa-linkedin contact-icon"></i>
                        <span>LinkedIn</span>
                    </a>
                    <a href="#" class="contact-item">
                        <i class="fab fa-twitter contact-icon"></i>
                        <span>Twitter</span>
                    </a>
                </div>
            </div>
        </div>
        
        <footer>
            <p>Warping through the digital cosmos at light speed • Established 2023</p>
            <p>Current location: GitHub Sector 7G • Transmission status: Active</p>
        </footer>
    </div>
    
    <script>
        // Create animated stars
        function createStars() {
            const starsContainer = document.getElementById('stars');
            const starsCount = 200;
            
            for (let i = 0; i < starsCount; i++) {
                const star = document.createElement('div');
                star.classList.add('star');
                
                // Random position
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                
                // Random size
                const size = Math.random() * 3;
                
                // Random animation duration
                const duration = 2 + Math.random() * 8;
                
                star.style.left = `${posX}%`;
                star.style.top = `${posY}%`;
                star.style.width = `${size}px`;
                star.style.height = `${size}px`;
                star.style.setProperty('--duration', `${duration}s`);
                star.style.animationDelay = `${Math.random() * 5}s`;
                
                starsContainer.appendChild(star);
            }
        }
        
        document.addEventListener('DOMContentLoaded', createStars);
        
        // Create matrix-like falling code effect
        function createMatrixEffect() {
            const matrixContainer = document.createElement('div');
            matrixContainer.style.position = 'fixed';
            matrixContainer.style.top = '0';
            matrixContainer.style.left = '0';
            matrixContainer.style.width = '100%';
            matrixContainer.style.height = '100%';
            matrixContainer.style.pointerEvents = 'none';
            matrixContainer.style.zIndex = '-1';
            matrixContainer.style.overflow = 'hidden';
            document.body.appendChild(matrixContainer);
            
            const characters = '01';
            const fontSize = 14;
            const columns = Math.floor(window.innerWidth / fontSize);
            
            for (let i = 0; i < columns; i++) {
                const column = document.createElement('div');
                column.style.position = 'absolute';
                column.style.top = '-100px';
                column.style.left = `${i * fontSize}px`;
                column.style.width = `${fontSize}px`;
                column.style.fontFamily = 'monospace';
                column.style.fontSize = `${fontSize}px`;
                column.style.color = 'rgba(0, 255, 157, 0.8)';
                column.style.textShadow = '0 0 5px rgba(0, 255, 157, 0.5)';
                column.style.writingMode = 'vertical-rl';
                column.style.textOrientation = 'mixed';
                matrixContainer.appendChild(column);
                
                animateColumn(column);
            }
            
            function animateColumn(column) {
                let content = '';
                const length = 20 + Math.floor(Math.random() * 20);
                const speed = 50 + Math.random() * 150;
                
                for (let i = 0; i < length; i++) {
                    content += characters.charAt(Math.floor(Math.random() * characters.length));
                }
                
                column.textContent = content;
                column.style.top = '-100px';
                
                setTimeout(() => {
                    column.style.transition = `top ${speed / 1000}s linear`;
                    column.style.top = `${window.innerHeight}px`;
                }, 100);
                
                setTimeout(() => {
                    animateColumn(column);
                }, speed + 2000);
            }
        }
        
        // Uncomment to enable Matrix effect (can be performance intensive)
        // createMatrixEffect();
    </script>
    
    <!-- Font Awesome for icons -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
