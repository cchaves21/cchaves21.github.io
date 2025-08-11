---
layout: page
title: Carlos Chaves
---

<style>
.hero-section {
  text-align: center;
  margin-bottom: 50px;
  padding: 40px 20px;
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  border-radius: 20px;
  border-left: 6px solid #00d9ff;
  box-shadow: 0 12px 40px rgba(0, 217, 255, 0.2);
  position: relative;
  overflow: hidden;
  .social-links {
    flex-direction: column;
    align-items: center;
  }
}

.hero-section::before {
  content: "";
  position: absolute;
  top: -50%;
  right: -50%;
  width: 100%;
  height: 200%;
  background: radial-gradient(circle, rgba(0, 217, 255, 0.1) 0%, transparent 70%);
  animation: float 6s ease-in-out infinite;
}

@keyframes float {
  0%, 100% { transform: translateY(0px) rotate(0deg); }
  50% { transform: translateY(-20px) rotate(5deg); }
}

.hero-content {
  position: relative;
  z-index: 2;
}

.hero-section h1 {
  color: #ffffff;
  margin-bottom: 15px;
  font-size: 2.8em;
  font-weight: 700;
  text-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
}

.hero-subtitle {
  color: #00d9ff;
  font-size: 1.5em;
  font-weight: 500;
  margin-bottom: 20px;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

.hero-description {
  color: #e0e0e0;
  font-size: 1.2em;
  line-height: 1.6;
  margin-bottom: 30px;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

.cta-buttons {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
}

.cta-btn {
  display: inline-block;
  padding: 15px 30px;
  text-decoration: none;
  border-radius: 30px;
  font-weight: 600;
  font-size: 1.1em;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.cta-btn.primary {
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  color: #000000 !important;
  box-shadow: 0 6px 25px rgba(0, 217, 255, 0.4);
}

.cta-btn.secondary {
  background: transparent;
  color: #00d9ff !important;
  border: 2px solid #00d9ff;
  box-shadow: 0 4px 20px rgba(0, 217, 255, 0.2);
}

.cta-btn:hover {
  transform: translateY(-3px);
  text-decoration: none;
}

.cta-btn.primary:hover {
  box-shadow: 0 8px 35px rgba(0, 217, 255, 0.6);
  background: linear-gradient(135deg, #00e6ff, #00b3e6);
}

.cta-btn.secondary:hover {
  background: rgba(0, 217, 255, 0.1);
  box-shadow: 0 6px 30px rgba(0, 217, 255, 0.4);
}

/* Navigation Menu */
.main-nav {
  background: rgba(26, 26, 46, 0.95);
  border: 2px solid rgba(0, 217, 255, 0.3);
  border-radius: 15px;
  padding: 25px;
  margin: 40px 0;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(15px);
}

.main-nav h3 {
  color: #ffffff;
  margin-bottom: 20px;
  font-size: 1.3em;
  text-align: center;
}

.nav-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 15px;
}

.nav-item {
  color: #b3b3b3;
  text-decoration: none;
  padding: 12px 20px;
  border-radius: 10px;
  transition: all 0.3s ease;
  border-left: 4px solid transparent;
  text-align: center;
  font-weight: 500;
}

.nav-item:hover {
  background: rgba(0, 217, 255, 0.1);
  border-left-color: #00d9ff;
  color: #00d9ff;
  text-decoration: none;
  transform: translateX(5px);
}

/* Section Headers */
.section-header {
  display: flex;
  align-items: center;
  margin: 50px 0 30px 0;
  padding-bottom: 15px;
  border-bottom: 3px solid rgba(0, 217, 255, 0.3);
  position: relative;
}

.section-header::after {
  content: "";
  position: absolute;
  bottom: -3px;
  left: 0;
  width: 60px;
  height: 3px;
  background: linear-gradient(90deg, #00d9ff, #0099cc);
  border-radius: 2px;
}

.section-header h2 {
  color: #ffffff;
  margin: 0;
  font-size: 2em;
  font-weight: 600;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

/* About Section */
.about-content {
  background: linear-gradient(135deg, rgba(0, 217, 255, 0.1) 0%, rgba(26, 26, 46, 0.8) 100%);
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-left: 5px solid #00d9ff;
  border-radius: 15px;
  padding: 30px;
  margin: 25px 0;
  font-size: 1.1em;
  line-height: 1.8;
  color: #e0e0e0;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
}

/* Tech Stack */
.tech-stack {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin: 30px 0;
}

.tech-category {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.9), rgba(22, 33, 62, 0.9));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 12px;
  padding: 25px;
  transition: all 0.3s ease;
  border-left: 4px solid #00d9ff;
  box-shadow: 0 6px 25px rgba(0, 0, 0, 0.3);
}

.tech-category:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 35px rgba(0, 217, 255, 0.2);
  border-color: rgba(0, 217, 255, 0.5);
}

.tech-category h4 {
  color: #00d9ff;
  margin: 0 0 15px 0;
  font-size: 1.2em;
  font-weight: 600;
}

.tech-category .tech-items {
  color: #e0e0e0;
  line-height: 1.6;
}

/* Articles Section */
.articles-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 25px;
  margin: 30px 0;
}

.article-card {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.95), rgba(22, 33, 62, 0.95));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 15px;
  padding: 30px;
  transition: all 0.3s ease;
  border-left: 5px solid #00d9ff;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
  position: relative;
  overflow: hidden;
}

.article-card::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  width: 100px;
  height: 100px;
  background: radial-gradient(circle, rgba(0, 217, 255, 0.1) 0%, transparent 70%);
  border-radius: 50%;
  transform: translate(30px, -30px);
}

.article-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 50px rgba(0, 217, 255, 0.2);
  border-color: rgba(0, 217, 255, 0.6);
}

.article-card h4 {
  color: #ffffff;
  margin: 0 0 15px 0;
  font-size: 1.3em;
  font-weight: 600;
  line-height: 1.4;
  position: relative;
  z-index: 2;
}

.article-card .article-meta {
  color: #b3b3b3;
  font-size: 0.9em;
  margin-bottom: 15px;
}

.article-card .article-excerpt {
  color: #e0e0e0;
  line-height: 1.6;
  font-size: 1em;
}

.read-more {
  display: inline-block;
  color: #00d9ff;
  text-decoration: none;
  font-weight: 500;
  margin-top: 15px;
  transition: all 0.3s ease;
}

.read-more:hover {
  color: #00e6ff;
  text-decoration: none;
  transform: translateX(5px);
}

.read-more::after {
  content: " →";
  transition: transform 0.3s ease;
}

.read-more:hover::after {
  transform: translateX(3px);
}

/* Career Highlights Section */
.highlights-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 25px;
  margin: 30px 0;
}

.highlight-item {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.95), rgba(22, 33, 62, 0.95));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 15px;
  padding: 25px;
  transition: all 0.3s ease;
  border-left: 5px solid #00d9ff;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
  display: flex;
  align-items: flex-start;
  gap: 20px;
}

.highlight-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 50px rgba(0, 217, 255, 0.2);
  border-color: rgba(0, 217, 255, 0.6);
}

.highlight-icon {
  font-size: 2.5em;
  flex-shrink: 0;
  width: 60px;
  text-align: center;
}

.highlight-content h4 {
  color: #ffffff;
  margin: 0 0 10px 0;
  font-size: 1.2em;
  font-weight: 600;
}

.highlight-content p {
  color: #e0e0e0;
  line-height: 1.6;
  margin: 0;
}

.action-buttons {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 40px;
  flex-wrap: wrap;
}

/* Philosophy Section */
.philosophy-content {
  background: linear-gradient(135deg, rgba(0, 217, 255, 0.15) 0%, rgba(26, 26, 46, 0.9) 100%);
  border: 1px solid rgba(0, 217, 255, 0.4);
  border-left: 6px solid #00d9ff;
  border-radius: 15px;
  padding: 35px;
  margin: 25px 0;
  font-size: 1.2em;
  line-height: 1.8;
  color: #e0e0e0;
  box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3);
  text-align: center;
  position: relative;
  overflow: hidden;
}

.philosophy-content::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(0, 217, 255, 0.05) 0%, transparent 70%);
  animation: pulse 4s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 0.5; }
  50% { transform: scale(1.1); opacity: 0.8; }
}

.philosophy-content strong {
  color: #00d9ff;
  font-weight: 600;
}

.philosophy-highlight {
  display: block;
  font-size: 1.4em;
  font-weight: 700;
  color: #00d9ff;
  text-shadow: 0 2px 8px rgba(0, 217, 255, 0.5);
  margin-top: 20px;
  position: relative;
  z-index: 2;
}
.contact-info {
  text-align: center;
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.9), rgba(22, 33, 62, 0.9));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 15px;
  padding: 40px;
  margin: 30px 0;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
}

.contact-info h3 {
  color: #ffffff;
  margin-bottom: 20px;
  font-size: 1.5em;
}

.contact-info p {
  color: #e0e0e0;
  font-size: 1.1em;
  margin-bottom: 25px;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.social-link {
  display: inline-block;
  color: #00d9ff;
  text-decoration: none;
  font-weight: 500;
  padding: 10px 20px;
  border: 2px solid #00d9ff;
  border-radius: 25px;
  transition: all 0.3s ease;
}

.social-link:hover {
  background: rgba(0, 217, 255, 0.1);
  color: #00e6ff;
  text-decoration: none;
  transform: translateY(-2px);
  box-shadow: 0 5px 20px rgba(0, 217, 255, 0.3);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-section h1 {
    font-size: 2.2em;
  }
  
  .hero-subtitle {
    font-size: 1.3em;
  }
  
  .cta-buttons {
    flex-direction: column;
    align-items: center;
  }
  
  .nav-grid {
    grid-template-columns: 1fr;
  }
  
  .tech-stack {
    grid-template-columns: 1fr;
  }
  
  .articles-grid {
    grid-template-columns: 1fr;
  }
  
  .highlights-grid {
    grid-template-columns: 1fr;
  }
  
  .highlight-item {
    flex-direction: column;
    text-align: center;
  }
  
  .action-buttons {
    flex-direction: column;
    align-items: center;
  }
}

/* Smooth Scrolling & Animations */
html {
  scroll-behavior: smooth;
}

.section-content {
  animation: fadeInUp 0.6s ease-out;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<div class="hero-section">
  <div class="hero-content">
    <h1>Carlos Chaves</h1>
    <div class="hero-subtitle">Head of Quality & Senior QA Engineer</div>
    <div class="hero-description">
      Results-driven QA professional with 15+ years of experience in software quality assurance, test strategy implementation, and fostering continuous improvement cultures. Passionate about quality advocacy, team mentoring, and data-driven efficiency.
    </div>
    <div class="cta-buttons">
      <a href="/cv/" class="cta-btn primary">View My CV</a>
      <a href="#contact" class="cta-btn secondary">Get In Touch</a>
    </div>
  </div>
</div>

<div class="main-nav">
  <h3>🧭 Quick Navigation</h3>
  <div class="nav-grid">
    <a href="#about" class="nav-item">👨‍💼 About Me</a>
    <a href="#career-highlights" class="nav-item">🏆 Career Highlights</a>
    <a href="#what-drives-me" class="nav-item">💡 What Drives Me</a>
    <a href="#tech-stack" class="nav-item">⚙️ Tech Stack</a>
    <a href="#articles" class="nav-item">📝 Articles</a>
    <a href="#contact" class="nav-item">📞 Contact</a>
    <a href="/cv/" class="nav-item">📄 Full CV</a>
  </div>
</div>

---

<div class="section-header">
  <h2 id="about">👨‍💼 About Me</h2>
</div>

<div class="section-content">
  <div class="about-content">
    I'm Carlos Chaves, a QA professional with over 15 years of experience in software quality, automation, and technical leadership. I started my journey in São Paulo, Brazil, working at a consultancy focused on integrated business solutions. What began as an internship quickly turned into a lifelong passion for testing and quality engineering.
    <br><br>
    Over the years, I've worked across multiple industries, from finance to retail tech. Always with a focus on improving product quality and team maturity through smart processes and tooling.
    <br><br>
    Currently, I serve as <strong>Head of QA</strong> in a British company that has scaled revenue to $150M+ in the last year, where I lead strategic quality initiatives and support the growth of QA as an engineering discipline.
  </div>
</div>

---

<div class="section-header">
  <h2 id="career-highlights">🏆 Career Highlights</h2>
</div>

<div class="section-content">
  <div class="highlights-grid">
    <div class="highlight-item">
      <div class="highlight-icon">🔁</div>
      <div class="highlight-content">
        <h4>Shift-Left Testing Implementation</h4>
        <p>Introduced shift-left testing and continuous integration practices across multiple organizations</p>
      </div>
    </div>

    <div class="highlight-item">
      <div class="highlight-icon">🧪</div>
      <div class="highlight-content">
        <h4>Automated Test Frameworks</h4>
        <p>Designed and implemented automated test frameworks across multiple platforms</p>
      </div>
    </div>

    <div class="highlight-item">
      <div class="highlight-icon">📘</div>
      <div class="highlight-content">
        <h4>QA Handbook Creation</h4>
        <p>Authored the company-wide QA Handbook to define standards and best practices</p>
      </div>
    </div>

    <div class="highlight-item">
      <div class="highlight-icon">🚀</div>
      <div class="highlight-content">
        <h4>Path to Engineering Program</h4>
        <p>Created and led the Path to Engineering program, helping internal talent grow into engineering roles</p>
      </div>
    </div>

    <div class="highlight-item">
      <div class="highlight-icon">🏆</div>
      <div class="highlight-content">
        <h4>PRAD Recognition Award</h4>
        <p>Received recognition from the largest bank in Latin America for QA leadership during the launch of PIX, a real-time payment system that revolutionized the Brazilian financial market</p>
      </div>
    </div>

    <div class="highlight-item">
      <div class="highlight-icon">🤝</div>
      <div class="highlight-content">
        <h4>Mentoring & Collaboration</h4>
        <p>Passionate about mentoring, documentation, and cross-functional collaboration</p>
      </div>
    </div>
  </div>

  <div class="action-buttons">
    <a href="/case-studies" class="cta-btn primary">📂 View Case Studies</a>
    <a href="/tech-stack" class="cta-btn secondary">🛠 Tech Stack</a>
  </div>
</div>

---

<div class="section-header">
  <h2 id="what-drives-me">💡 What Drives Me</h2>
</div>

<div class="section-content">
  <div class="philosophy-content">
    I believe quality is not just about finding bugs, it's about <strong>building confidence</strong> in what we deliver, <strong>enabling developers</strong>, and <strong>championing user experience</strong>.
    <br><br>
    <span class="philosophy-highlight">Good QA is proactive, not reactive.</span>
  </div>
</div>

---

<div class="section-header">
  <h2 id="tech-stack">⚙️ Tech Stack</h2>
</div>

<div class="section-content">
  <div class="tech-stack">
    <div class="tech-category">
      <h4>🤖 Test Automation Tools</h4>
      <div class="tech-items">
        Appium, Selenium, Cypress, Playwright
      </div>
    </div>

    <div class="tech-category">
      <h4>💻 Languages & Scripting</h4>
      <div class="tech-items">
        Java, JavaScript
      </div>
    </div>

    <div class="tech-category">
      <h4>🧪 Test Frameworks</h4>
      <div class="tech-items">
        Cucumber, JUnit
      </div>
    </div>

    <div class="tech-category">
      <h4>🔄 CI/CD & Infrastructure</h4>
      <div class="tech-items">
        Jenkins, GitHub Actions, GitLab CI
      </div>
    </div>

    <div class="tech-category">
      <h4>🤝 Collaboration & Documentation</h4>
      <div class="tech-items">
        Jira, Xray
      </div>
    </div>

    <div class="tech-category">
      <h4>☁️ Cloud</h4>
      <div class="tech-items">
        AWS
      </div>
    </div>
  </div>
</div>

---

<div class="section-header">
  <h2 id="articles">📝 Published Articles</h2>
</div>

<div class="section-content">
  <div class="articles-grid">
    <div class="article-card">
      <h4>Shift-Left Testing: It's Not Just About Involving QA Early</h4>
      <div class="article-meta">Quality Engineering • Testing Strategy</div>
      <div class="article-excerpt">
        Exploring the true essence of shift-left testing beyond the common misconception of simply involving QA earlier in the development cycle. Discover how to build quality into every stage of your software development process.
      </div>
      <a href="https://medium.com/@kchaves001/shift-left-testing-its-not-just-about-involving-qa-early-ad80ed4db714" class="read-more" target="_blank" 
      rel="noopener noreferrer">Read Article</a>
    </div>

    <div class="article-card">
      <h4>The Evolution of Leadership: From Command to Care</h4>
      <div class="article-meta">Leadership • Team Management</div>
      <div class="article-excerpt">
        A reflection on modern leadership in tech teams, examining how the shift from traditional command-and-control to empathetic, servant leadership creates more effective and motivated teams.
      </div>
      <a href="https://medium.com/@kchaves001/the-evolution-of-leadership-from-command-to-care-ae47d152e54e" class="read-more" target="_blank" 
      rel="noopener noreferrer">Read Article</a>
    </div>

    <div class="article-card">
      <h4>The Test Pyramid: Insights from 15 Years of Experience</h4>
      <div class="article-meta">Test Architecture • Automation Strategy</div>
      <div class="article-excerpt">
        Real-world insights and lessons learned from implementing test pyramid strategies across different organizations, technologies, and team structures over 15 years in software quality assurance.
      </div>
      <a href="https://medium.com/@kchaves001/the-test-pyramid-insights-from-15-years-of-experience-4adbdaf300f5" class="read-more" target="_blank" 
      rel="noopener noreferrer">Read Article</a>
    </div>
  </div>
</div>

---

<div class="section-header">
  <h2 id="contact">📞 Let's Connect</h2>
</div>

<div class="section-content">
  <div class="contact-info">
    <h3>Ready to collaborate?</h3>
    <p>I'm always open to discussing quality engineering, sharing experiences, or exploring new opportunities. Let's connect and see how we can work together to build better software.</p>
    
    <div class="social-links">
      <a href="https://www.linkedin.com/in/carlos-chaves-3b616924" class="social-link">LinkedIn</a>
      <a href="https://github.com/cchaves21" class="social-link">GitHub</a>
      <a href="mailto:carlosrschaves@gmail.com" class="social-link">Email</a>
      <a href="/cv/" class="social-link">My CV</a>
    </div>
  </div>
</div>

---