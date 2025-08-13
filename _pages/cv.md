---
layout: page
title: Curriculum Vitae
permalink: /cv/
---

<style>
/* Dark Theme Optimized */
.cv-header {
  text-align: center;
  margin-bottom: 40px;
  padding: 30px 20px;
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  border-radius: 15px;
  border-left: 6px solid #00d9ff;
  box-shadow: 0 8px 32px rgba(0, 217, 255, 0.2);
}

.cv-header h1 {
  color: #ffffff;
  margin-bottom: 10px;
  font-size: 2.2em;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

.cv-title {
  color: #00d9ff;
  font-size: 1.3em;
  font-weight: 500;
  margin-bottom: 20px;
}

.download-btn {
  display: inline-block;
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  color: white !important;
  padding: 12px 24px;
  text-decoration: none;
  border-radius: 25px;
  font-weight: 600;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0, 217, 255, 0.4);
  border: 1px solid rgba(0, 217, 255, 0.3);
}

.download-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 25px rgba(0, 217, 255, 0.6);
  text-decoration: none;
  color: white !important;
  background: linear-gradient(135deg, #00e6ff, #00b3e6);
}

/* Navigation Menu */
.cv-nav {
  background: rgba(26, 26, 46, 0.95);
  border: 2px solid rgba(0, 217, 255, 0.3);
  border-radius: 12px;
  padding: 20px;
  margin: 30px 0;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(10px);
}

.cv-nav h3 {
  color: #ffffff;
  margin-bottom: 15px;
  font-size: 1.1em;
}

.nav-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 10px;
}

.nav-grid a {
  color: #b3b3b3;
  text-decoration: none;
  padding: 8px 15px;
  border-radius: 8px;
  transition: all 0.3s ease;
  border-left: 3px solid transparent;
}

.nav-grid a:hover {
  background: rgba(0, 217, 255, 0.1);
  border-left-color: #00d9ff;
  color: #00d9ff;
  text-decoration: none;
}

/* Section Headers */
.section-header {
  display: flex;
  align-items: center;
  margin: 40px 0 25px 0;
  padding-bottom: 10px;
  border-bottom: 2px solid rgba(0, 217, 255, 0.3);
}

.section-header h2 {
  color: #ffffff;
  margin: 0;
  font-size: 1.8em;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

/* Summary */
.summary-box {
  background: linear-gradient(135deg, rgba(0, 217, 255, 0.1) 0%, rgba(26, 26, 46, 0.8) 100%);
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-left: 5px solid #00d9ff;
  border-radius: 12px;
  padding: 25px;
  margin: 20px 0;
  font-size: 1.1em;
  line-height: 1.7;
  color: #e0e0e0;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
}

/* Skills Grid */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 15px;
  margin: 20px 0;
}

.skill-item {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.9), rgba(22, 33, 62, 0.9));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 10px;
  padding: 15px;
  transition: all 0.3s ease;
  border-left: 4px solid #00d9ff;
  color: #ffffff;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
}

.skill-item:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(0, 217, 255, 0.2);
  border-left-color: #00e6ff;
}

/* Timeline */
.timeline {
  position: relative;
  margin: 40px 0;
  padding-left: 50px;
  border-left: 3px solid rgba(0, 217, 255, 0.3);
}

.timeline::before {
  content: "";
  position: absolute;
  left: -2px;
  top: 0;
  bottom: 0;
  width: 3px;
  background: linear-gradient(180deg, #00d9ff 0%, #0099cc 50%, #006699 100%);
  border-radius: 2px;
  box-shadow: 0 0 10px rgba(0, 217, 255, 0.5);
}

.timeline-item {
  margin-bottom: 40px;
  position: relative;
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.95), rgba(22, 33, 62, 0.95));
  border-radius: 12px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
  padding: 24px;
  margin-left: -20px;
  transition: all 0.3s ease;
  border-left: 4px solid #00d9ff;
  border: 1px solid rgba(0, 217, 255, 0.2);
}

.timeline-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 40px rgba(0, 217, 255, 0.2);
  border-color: rgba(0, 217, 255, 0.4);
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -32px;
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  border: 4px solid #1a1a2e;
  border-radius: 50%;
  width: 20px;
  height: 20px;
  top: 20px;
  box-shadow: 0 0 15px rgba(0, 217, 255, 0.6);
  z-index: 2;
}

.timeline-item h4 {
  margin: 0 0 8px 0;
  color: #ffffff;
  font-size: 1.3em;
  font-weight: 600;
  line-height: 1.3;
}

.timeline-item .company {
  font-size: 1.1em;
  color: #00d9ff;
  font-weight: 500;
  margin-bottom: 6px;
  display: block;
}

.timeline-item .period {
  font-size: 0.9em;
  color: #b3b3b3;
  font-weight: 500;
  background: rgba(0, 217, 255, 0.2);
  padding: 4px 12px;
  border-radius: 20px;
  display: inline-block;
  margin-bottom: 12px;
  border: 1px solid rgba(0, 217, 255, 0.3);
}

.timeline-item .description {
  color: #e0e0e0;
  line-height: 1.6;
  margin-top: 10px;
}

.timeline-item:first-child::after {
  content: "Current";
  position: absolute;
  top: -10px;
  right: 15px;
  background: linear-gradient(135deg, #00ff88, #00cc6a);
  color: #000000;
  padding: 4px 10px;
  border-radius: 12px;
  font-size: 0.75em;
  font-weight: 600;
  box-shadow: 0 2px 10px rgba(0, 255, 136, 0.4);
}

/* Education & Certifications */
.info-card {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.95), rgba(22, 33, 62, 0.95));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 12px;
  padding: 20px;
  margin: 15px 0;
  border-left: 4px solid #00d9ff;
  transition: all 0.3s ease;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
}

.info-card:hover {
  box-shadow: 0 8px 30px rgba(0, 217, 255, 0.2);
  transform: translateY(-2px);
}

.info-card h4 {
  color: #ffffff;
  margin: 0 0 8px 0;
}

.info-card .meta {
  color: #b3b3b3;
  font-size: 0.9em;
}

/* Languages */
.languages-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 15px;
  margin: 20px 0;
}

.language-item {
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  color: #000000;
  padding: 20px;
  border-radius: 12px;
  text-align: center;
  font-weight: 500;
  box-shadow: 0 6px 25px rgba(0, 217, 255, 0.3);
  transition: all 0.3s ease;
}

.language-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 35px rgba(0, 217, 255, 0.4);
}

.language-item .level {
  font-size: 0.9em;
  opacity: 0.8;
  margin-top: 5px;
  font-weight: 600;
}

/* Responsive*/
@media (max-width: 768px) {
  .cv-header {
    padding: 20px 15px;
  }
  
  .cv-header h1 {
    font-size: 1.8em;
  }
  
  .timeline {
    padding-left: 25px;
    margin: 20px 0;
  }
  
  .timeline-item {
    margin-left: -10px;
    padding: 20px 16px;
    margin-bottom: 25px;
  }
  
  .timeline-item::before {
    left: -22px;
    width: 16px;
    height: 16px;
    top: 18px;
  }
  
  .nav-grid {
    grid-template-columns: 1fr;
  }
}

/* Animations */
html {
  scroll-behavior: smooth;
}

.timeline-item {
  animation: slideInLeft 0.6s ease-out;
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>

<div class="cv-header">
  <h1>Carlos Chaves</h1>
  <div class="cv-title">Head of Quality & Senior QA Engineer</div>
  <!-- <a href="/assets/Carlos_Chaves_CV.pdf" class="download-btn" target="_blank">📄 Download PDF</a> -->
</div>

<div class="cv-nav">
  <h3>📌 Navigation</h3>
  <div class="nav-grid">
    <a href="#professional-summary">💼 Professional Summary</a>
    <a href="#core-skills">🛠 Core Skills</a>
    <a href="#professional-experience">📈 Professional Experience</a>
    <a href="#education">🎓 Education</a>
    <a href="#certifications">📜 Certifications</a>
    <a href="#languages">🌍 Languages</a>
  </div>
</div>

---

<div class="section-header">
  <h2 id="professional-summary">💼 Professional Summary</h2>
</div>

<div class="summary-box">
Results-driven QA professional with more than 15 years of experience in software quality assurance, test strategy implementation, and fostering a culture of continuous improvement. Expertise in leading teams, optimising testing processes, and integrating automated testing into CI/CD pipelines. Passionate about advocating for quality at all stages of development, mentoring teams, and leveraging data-driven insights to drive efficiency.
</div>

---

<div class="section-header">
  <h2 id="core-skills">🛠 Core Skills</h2>
</div>

<div class="skills-grid">
  <div class="skill-item">✅ Test Strategy & Process Optimisation</div>
  <div class="skill-item">⬅️ Shift-Left Testing & CI/CD Integration</div>
  <div class="skill-item">🤖 Test Automation (Selenium, Cypress, Playwright)</div>
  <div class="skill-item">⚡ Performance Testing</div>
  <div class="skill-item">🔄 Agile & DevOps Quality Practices</div>
  <div class="skill-item">👨‍💼 Technical Leadership & Mentoring</div>
  <div class="skill-item">⚠️ Risk Assessment & Defect Management</div>
  <div class="skill-item">🤝 Stakeholder Communication & Collaboration</div>
  <div class="skill-item">🧪 Test Frameworks: BDD, TDD, ATDD</div>
</div>

---

<div class="section-header">
  <h2 id="professional-experience">📈 Professional Experience</h2>
</div>

<div class="timeline">
  <div class="timeline-item">
    <h4>Head of Quality</h4>
    <span class="company">Epos Now</span>
    <span class="period">Dec 2023 – Present</span>
    <div class="description">
      Led the transition to a quality-first approach with Shift-Left Testing, mentored 8+ QA team members, defined KPIs, and implemented data-driven QA strategies.
    </div>
  </div>

  <div class="timeline-item">
    <h4>Senior QA Engineer</h4>
    <span class="company">Epos Now</span>
    <span class="period">Dec 2022 – Dec 2023</span>
    <div class="description">
      Implemented automated test strategies in CI/CD pipelines, migrated legacy systems to React with Playwright automation, and optimised regression suites.
    </div>
  </div>

  <div class="timeline-item">
    <h4>Senior QA Engineer</h4>
    <span class="company">Fidel API</span>
    <span class="period">Jun 2021 – Nov 2022</span>
    <div class="description">
      Automated API testing with Cypress, introduced shift-left practices, and performed performance/security testing.
    </div>
  </div>

  <div class="timeline-item">
    <h4>Senior QA Engineer</h4>
    <span class="company">Itaú Bank</span>
    <span class="period">Mar 2020 – Jul 2021</span>
    <div class="description">
      Key QA role in PIX launch, led E2E testing, automated API/UI tests, and coordinated strategies across 5 squads.
    </div>
  </div>

  <div class="timeline-item">
    <h4>QA Lead</h4>
    <span class="company">Enjoei</span>
    <span class="period">Jul 2018 – Mar 2020</span>
    <div class="description">
      Built mobile automation framework with Appium & Cucumber, integrated tests into Docker/CD pipelines, and led QA hiring and mentoring.
    </div>
  </div>

  <div class="timeline-item">
    <h4>QA Engineer</h4>
    <span class="company">Software Quality Consulting</span>
    <span class="period">2008 – 2018</span>
    <div class="description">
      Worked across major clients like BTG Pactual, PagSeguro, and RedBull, leading automation with Selenium & BDD.
    </div>
  </div>
</div>

---

<div class="section-header">
  <h2 id="education">🎓 Education</h2>
</div>

<div class="info-card">
  <h4>Bachelor of Computer Information Systems</h4>
  <div class="meta">Universidade Presbiteriana Mackenzie • Dec 2014</div>
</div>

---

<div class="section-header">
  <h2 id="certifications">📜 Certifications</h2>
</div>

<div class="info-card">
  <h4>ISTQB - Foundation Level Certification</h4>
</div>

<div class="info-card">
  <h4>Test Quality in Agile Methodologies</h4>
  <div class="meta">Kanban and Scrum • Knowledge21</div>
</div>

<div class="info-card">
  <h4>Advanced Test Management</h4>
  <div class="meta">ISTQB syllabus</div>
</div>

---

<div class="section-header">
  <h2 id="languages">🌍 Languages</h2>
</div>

<div class="languages-grid">
  <div class="language-item">
    <div>Portuguese</div>
    <div class="level">Native</div>
  </div>
  <div class="language-item">
    <div>English</div>
    <div class="level">Fluent</div>
  </div>
</div>

---