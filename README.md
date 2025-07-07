<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Augusto Luzzi - Software Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
            padding: 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            background: linear-gradient(120deg, #6C63FF, #61DAFB);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .language-toggle {
            margin: 20px 0;
            display: flex;
            justify-content: center;
            gap: 10px;
        }
        
        .lang-btn {
            padding: 8px 20px;
            border: 2px solid #6C63FF;
            background: transparent;
            color: #6C63FF;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        
        .lang-btn.active {
            background: #6C63FF;
            color: white;
        }
        
        .lang-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(108, 99, 255, 0.3);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
        }
        
        .social-link {
            padding: 10px 20px;
            background: #238636;
            color: white;
            text-decoration: none;
            border-radius: 6px;
            transition: all 0.3s ease;
        }
        
        .social-link:hover {
            background: #2ea043;
            transform: translateY(-2px);
        }
        
        .code-block {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
            margin: 20px 0;
            font-family: 'Consolas', 'Monaco', monospace;
            overflow-x: auto;
        }
        
        .section {
            margin: 40px 0;
        }
        
        .tech-stack {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .tech-category {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
        }
        
        .tech-category h3 {
            color: #6C63FF;
            margin-bottom: 15px;
        }
        
        .tech-badge {
            display: inline-block;
            padding: 5px 10px;
            margin: 5px;
            background: #30363d;
            border-radius: 4px;
            font-size: 0.9em;
        }
        
        .quote {
            font-size: 1.2em;
            font-style: italic;
            text-align: center;
            margin: 30px 0;
            padding: 20px;
            border-left: 4px solid #6C63FF;
            background: #161b22;
        }
        
        .highlights {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }
        
        .highlight-item {
            background: #161b22;
            padding: 15px;
            border-radius: 8px;
            border-left: 3px solid #6C63FF;
        }
        
        .stats {
            text-align: center;
            margin: 40px 0;
        }
        
        .stats img {
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .section {
            animation: fadeIn 0.6s ease-out;
        }
        
        /* Typing animation */
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink {
            50% { border-color: transparent }
        }
        
        .typing-text {
            overflow: hidden;
            border-right: 3px solid #6C63FF;
            white-space: nowrap;
            animation: typing 3.5s steps(40, end), blink .75s step-end infinite;
            margin: 0 auto;
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            h1 { font-size: 2em; }
            .tech-stack { grid-template-columns: 1fr; }
            .highlights { grid-template-columns: 1fr; }
        }
        
        .footer {
            text-align: center;
            margin-top: 60px;
            padding-top: 30px;
            border-top: 1px solid #30363d;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Augusto Luzzi</h1>
            <p class="subtitle" data-en="Full-Stack Engineer | Data Enthusiast" data-pt="Engenheiro Full-Stack | Entusiasta de Dados">Full-Stack Engineer | Data Enthusiast</p>
            
            <div class="language-toggle">
                <button class="lang-btn active" onclick="setLanguage('en')">🇺🇸 English</button>
                <button class="lang-btn" onclick="setLanguage('pt')">🇧🇷 Português</button>
            </div>
            
            <div class="social-links">
                <a href="https://www.linkedin.com/in/augusto-luzzi/" class="social-link">LinkedIn</a>
                <a href="https://github.com/augrumph" class="social-link">GitHub</a>
                <a href="mailto:seu-email@example.com" class="social-link">Email</a>
            </div>
        </div>
        
        <div class="section">
            <h2 data-en="🎯 TL;DR" data-pt="🎯 Resumo">🎯 TL;DR</h2>
            <div class="code-block">
<pre><code>const augusto = {
  <span data-en='role: "Software Engineer @ Grupo Marista"' data-pt='cargo: "Engenheiro de Software @ Grupo Marista"'>role: "Software Engineer @ Grupo Marista"</span>,
  <span data-en='location: "Curitiba, PR 🇧🇷"' data-pt='localização: "Curitiba, PR 🇧🇷"'>location: "Curitiba, PR 🇧🇷"</span>,
  <span data-en='experience: "2+ years"' data-pt='experiência: "2+ anos"'>experience: "2+ years"</span>,
  <span data-en='mindset: "Startup-oriented 🚀"' data-pt='mentalidade: "Orientado a startups 🚀"'>mindset: "Startup-oriented 🚀"</span>,
  <span data-en='superpower: "Connecting engineering with data insights 📊"' data-pt='superpoder: "Conectar engenharia com insights de dados 📊"'>superpower: "Connecting engineering with data insights 📊"</span>,
  <span data-en='currentlyLearning: "Cloud-native architectures"' data-pt='estudandoAtualmente: "Arquiteturas cloud-native"'>currentlyLearning: "Cloud-native architectures"</span>,
  <span data-en='lookingFor: "Opportunities to combine full-stack dev with data innovation"' data-pt='procurando: "Oportunidades para combinar dev full-stack com inovação em dados"'>lookingFor: "Opportunities to combine full-stack dev with data innovation"</span>
};</code></pre>
            </div>
        </div>
        
        <div class="section">
            <h2 data-en="💫 About Me" data-pt="💫 Sobre Mim">💫 About Me</h2>
            <div class="quote">
                <p data-en='"While most devs deliver code, I deliver intelligence."' data-pt='"Enquanto a maioria dos devs entrega código, eu entrego inteligência."'>"While most devs deliver code, I deliver intelligence."</p>
            </div>
            <p data-en="Started my journey in Data Science at BRF, where I discovered my superpower: connecting engineering and data analysis. Today, I build web and mobile applications that don't just work — they generate insights that impact thousands of users." 
               data-pt="Comecei minha jornada em Data Science na BRF, onde descobri meu superpoder: conectar engenharia e análise de dados. Hoje, desenvolvo aplicações web e mobile que não apenas funcionam — elas geram insights que impactam milhares de usuários.">
                Started my journey in Data Science at BRF, where I discovered my superpower: connecting engineering and data analysis. Today, I build web and mobile applications that don't just work — they generate insights that impact thousands of users.
            </p>
        </div>
        
        <div class="section">
            <h2 data-en="🏆 Highlights" data-pt="🏆 Destaques">🏆 Highlights</h2>
            <div class="highlights">
                <div class="highlight-item">
                    <strong>🥇</strong> <span data-en="Winner - HIPUC Health Innovation Hackathon" data-pt="Vencedor - Hackathon HIPUC de Inovação em Saúde">Winner - HIPUC Health Innovation Hackathon</span>
                </div>
                <div class="highlight-item">
                    <strong>👔</strong> <span data-en="VP - Software Engineering Academic Center (2 years)" data-pt="VP - Centro Acadêmico de Engenharia de Software (2 anos)">VP - Software Engineering Academic Center (2 years)</span>
                </div>
                <div class="highlight-item">
                    <strong>🚀</strong> <span data-en="Active Member - PUCPR-SPINE Entrepreneurship Hub" data-pt="Membro Ativo - Núcleo de Empreendedorismo PUCPR-SPINE">Active Member - PUCPR-SPINE Entrepreneurship Hub</span>
                </div>
                <div class="highlight-item">
                    <strong>📊</strong> <span data-en="Data Background - Transforming metrics into business decisions" data-pt="Background em Dados - Transformando métricas em decisões de negócio">Data Background - Transforming metrics into business decisions</span>
                </div>
            </div>
        </div>
        
        <div class="section">
            <h2>🛠️ Tech Stack</h2>
            <div class="tech-stack">
                <div class="tech-category">
                    <h3>Frontend</h3>
                    <span class="tech-badge">React.js</span>
                    <span class="tech-badge">TypeScript</span>
                    <span class="tech-badge">JavaScript</span>
                    <span class="tech-badge">HTML5</span>
                    <span class="tech-badge">CSS3</span>
                </div>
                <div class="tech-category">
                    <h3>Backend</h3>
                    <span class="tech-badge">Java</span>
                    <span class="tech-badge">Spring Boot</span>
                    <span class="tech-badge">Node.js</span>
                    <span class="tech-badge">Python</span>
                </div>
                <div class="tech-category">
                    <h3>Data & Analytics</h3>
                    <span class="tech-badge">MySQL</span>
                    <span class="tech-badge">SQL Server</span>
                    <span class="tech-badge">Power BI</span>
                </div>
                <div class="tech-category">
                    <h3>Cloud & DevOps</h3>
                    <span class="tech-badge">Azure</span>
                    <span class="tech-badge">Azure DevOps</span>
                    <span class="tech-badge">Git</span>
                </div>
            </div>
        </div>
        
        <div class="footer">
            <p data-en="Open to opportunities where I can combine full-stack development with my passion for data and innovation" 
               data-pt="Aberto a oportunidades onde posso combinar desenvolvimento full-stack com minha paixão por dados e inovação">
                Open to opportunities where I can combine full-stack development with my passion for data and innovation
            </p>
            <p style="margin-top: 20px; opacity: 0.7;">Made with 💜 by Augusto Luzzi</p>
        </div>
    </div>
    
    <script>
        function setLanguage(lang) {
            // Update button states
            document.querySelectorAll('.lang-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            event.target.classList.add('active');
            
            // Update all elements with language data
            document.querySelectorAll('[data-en][data-pt]').forEach(element => {
                element.textContent = element.getAttribute(`data-${lang}`);
            });
            
            // Save preference
            localStorage.setItem('preferredLanguage', lang);
        }
        
        // Load saved language preference
        document.addEventListener('DOMContentLoaded', function() {
            const savedLang = localStorage.getItem('preferredLanguage') || 'en';
            if (savedLang === 'pt') {
                document.querySelectorAll('.lang-btn')[1].click();
            }
        });
        
        // Add smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
