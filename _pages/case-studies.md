---
layout: page
title: Case Studies
permalink: /case-studies/
---

<style>
/* Case Studies - Dark Theme Consistent with Site */
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

.hero-title {
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
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

.projects-grid {
  display: flex;
  flex-direction: column;
  gap: 40px;
  margin-bottom: 50px;
}

.project-card {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.95), rgba(22, 33, 62, 0.95));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 20px;
  border-left: 6px solid #00d9ff;
  box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3);
  overflow: hidden;
  transition: all 0.3s ease;
  position: relative;
}

.project-card::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  width: 150px;
  height: 150px;
  background: radial-gradient(circle, rgba(0, 217, 255, 0.1) 0%, transparent 70%);
  border-radius: 50%;
  transform: translate(50px, -50px);
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 60px rgba(0, 217, 255, 0.2);
  border-color: rgba(0, 217, 255, 0.6);
}

.project-header {
  padding: 30px;
  position: relative;
  z-index: 2;
}

.project-icon {
  font-size: 3rem;
  display: block;
  margin-bottom: 15px;
}

.project-header h2 {
  margin: 0 0 15px 0;
  color: #ffffff;
  font-size: 2em;
  font-weight: 700;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

.project-badge {
  display: inline-block;
  padding: 8px 20px;
  border-radius: 25px;
  font-size: 0.9rem;
  font-weight: 600;
  color: #000000;
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  box-shadow: 0 4px 15px rgba(0, 217, 255, 0.3);
  margin-top: 10px;
}

.project-description {
  padding: 0 30px;
  font-size: 1.2rem;
  line-height: 1.7;
  color: #e0e0e0;
  position: relative;
  z-index: 2;
}

.project-details {
  padding: 30px;
  position: relative;
  z-index: 2;
}

.detail-section, .impact-section, .metrics-section {
  margin-bottom: 30px;
}

.detail-section h4, .impact-section h4, .metrics-section h4 {
  color: #00d9ff;
  margin-bottom: 15px;
  font-size: 1.3rem;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 10px;
}

.detail-section ul {
  list-style: none;
  padding: 0;
}

.detail-section li {
  padding: 8px 0;
  padding-left: 20px;
  position: relative;
  line-height: 1.6;
  color: #e0e0e0;
}

.detail-section li:before {
  content: "→";
  position: absolute;
  left: 0;
  color: #00d9ff;
  font-weight: bold;
  font-size: 1.2em;
}

.achievements {
  display: grid;
  gap: 15px;
}

.achievement {
  display: flex;
  align-items: flex-start;
  gap: 15px;
  padding: 20px;
  background: linear-gradient(135deg, rgba(0, 217, 255, 0.1) 0%, rgba(26, 26, 46, 0.8) 100%);
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 15px;
  border-left: 4px solid #00d9ff;
  transition: all 0.3s ease;
}

.achievement:hover {
  transform: translateX(5px);
  box-shadow: 0 8px 25px rgba(0, 217, 255, 0.2);
}

.achievement.award {
  border-left-color: #00e6ff;
  background: linear-gradient(135deg, rgba(0, 230, 255, 0.15) 0%, rgba(26, 26, 46, 0.9) 100%);
}

.achievement-icon {
  font-size: 2rem;
  flex-shrink: 0;
}

.achievement strong {
  display: block;
  margin-bottom: 5px;
  color: #ffffff;
  font-size: 1.1em;
}

.achievement p {
  color: #e0e0e0;
  margin: 0;
  line-height: 1.6;
}

.metrics-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
  margin-bottom: 20px;
}

.metric {
  text-align: center;
  padding: 25px;
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  color: #000000;
  border-radius: 15px;
  box-shadow: 0 8px 25px rgba(0, 217, 255, 0.3);
  transition: all 0.3s ease;
}

.metric:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 35px rgba(0, 217, 255, 0.4);
}

.metric-value {
  display: block;
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 8px;
}

.metric-label {
  font-size: 1rem;
  font-weight: 600;
  opacity: 0.9;
}

.additional-impacts {
  background: linear-gradient(135deg, rgba(26, 26, 46, 0.9), rgba(22, 33, 62, 0.9));
  border: 1px solid rgba(0, 217, 255, 0.3);
  border-radius: 12px;
  padding: 20px;
  border-left: 4px solid #00d9ff;
}

.additional-impacts p {
  margin: 8px 0;
  color: #e0e0e0;
  font-size: 1rem;
  line-height: 1.6;
}

.cta-section {
  text-align: center;
  padding: 40px 20px;
  background: linear-gradient(135deg, rgba(0, 217, 255, 0.15) 0%, rgba(26, 26, 46, 0.9) 100%);
  border: 1px solid rgba(0, 217, 255, 0.4);
  border-left: 6px solid #00d9ff;
  border-radius: 20px;
  margin-top: 40px;
  box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3);
  position: relative;
  overflow: hidden;
}

.cta-section::before {
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

.cta-section p {
  font-size: 1.3rem;
  color: #e0e0e0;
  margin-bottom: 25px;
  position: relative;
  z-index: 2;
}

.cta-button {
  display: inline-block;
  padding: 15px 30px;
  background: linear-gradient(135deg, #00d9ff, #0099cc);
  color: #000000;
  text-decoration: none;
  border-radius: 30px;
  font-weight: 600;
  font-size: 1.1em;
  transition: all 0.3s ease;
  box-shadow: 0 6px 25px rgba(0, 217, 255, 0.4);
  position: relative;
  z-index: 2;
}

.cta-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 35px rgba(0, 217, 255, 0.6);
  background: linear-gradient(135deg, #00e6ff, #00b3e6);
  text-decoration: none;
  color: #000000;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-section {
    padding: 30px 15px;
  }
  
  .hero-title {
    font-size: 2.2em;
  }
  
  .hero-subtitle {
    font-size: 1.3em;
  }
  
  .project-header, .project-details, .project-description {
    padding: 20px;
  }
  
  .project-header h2 {
    font-size: 1.6em;
  }
  
  .metrics-grid {
    grid-template-columns: 1fr;
  }
  
  .achievement {
    flex-direction: column;
    text-align: center;
  }
}

/* Smooth Scrolling & Animations */
html {
  scroll-behavior: smooth;
}

.project-card {
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
    <h1 class="hero-title">📚 Case Studies</h1>
    <p class="hero-subtitle">Explore some of the most impactful projects I've worked on throughout my QA career</p>
  </div>
</div>

<div class="projects-grid">
  <div class="project-card">
    <div class="project-header">
      <span class="project-icon">💸</span>
      <h2>Pix – A New Era of Payments</h2>
      <span class="project-badge">Brazil • 2020</span>
    </div>
    <div class="project-description">
      <p>Key QA role in the launch of Pix, Brazil's groundbreaking instant payment system that transformed the financial landscape at the largest bank in Latin America.</p>
    </div>
    <div class="project-details">
      <div class="detail-section">
        <h4>🎯 Challenges</h4>
        <ul>
          <li>Highly critical, real-time system affecting millions of users</li>
          <li>Tight deadlines and regulatory requirements from the Central Bank</li>
          <li>Complex integrations with existing banking infrastructure</li>
        </ul>
      </div>
      
      <div class="detail-section">
        <h4>💡 My Contributions</h4>
        <ul>
          <li>Conducted the <strong>test strategy</strong> for mobile core payment modules</li>
          <li>Implemented <strong>automated regression testing</strong> for Back-end using Java with Rest Assured</li>
          <li>Acted as <strong>focal point</strong> between multiple squads, ensuring communication between engineers and stakeholders</li>
          <li>Coordinated with cross-functional teams to ensure <strong>compliance and stability</strong></li>
        </ul>
      </div>

      <div class="impact-section">
        <h4>🏆 Impact & Recognition</h4>
        <div class="achievements">
          <div class="achievement">
            <span class="achievement-icon">🚀</span>
            <div>
              <strong>Market Impact</strong>
              <p>Pix became one of the fastest-adopted financial technologies in Brazilian history</p>
            </div>
          </div>
          <div class="achievement award">
            <span class="achievement-icon">🏅</span>
            <div>
              <strong>PRAD Recognition Award</strong>
              <p>Prestigious internal recognition for key contributors</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-header">
      <span class="project-icon">🧭</span>
      <h2>Epos Now – Building a Culture of Quality</h2>
      <span class="project-badge">UK • 2022-Present</span>
    </div>
    <div class="project-description">
      <p>Joined as <strong>Senior QA Engineer</strong> and promoted to <strong>Head of QA</strong> at a leading POS systems provider, scaling to over $150M annual revenue.</p>
    </div>
    <div class="project-details">
      <div class="detail-section">
        <h4>⚡ Challenges</h4>
        <ul>
          <li>Legacy code with only E2E tests and 800+ test case regression suite</li>
          <li>Manual testing bottlenecks impacting release cycles</li>
          <li>1 QA for every 8 developers ratio</li>
          <li>Fragmented team with unclear quality ownership</li>
        </ul>
      </div>
      
      <div class="detail-section">
        <h4>🔧 My Contributions</h4>
        <ul>
          <li>Created and rolled out a <strong>QA Handbook</strong> to standardize practices</li>
          <li>Introduced <strong>test automation</strong> with Playwright across legacy migration projects</li>
          <li>Developed strategy based on the <strong>Test Pyramid</strong> methodology</li>
          <li>Championed <strong>shift-left testing</strong> through data-driven workshops</li>
          <li>Mentored QAs and initiated <strong>Path to Engineering</strong> program</li>
          <li>Integrated tests into <strong>CI/CD pipelines</strong> using GitLab CI and Jenkins</li>
        </ul>
      </div>

      <div class="metrics-section">
        <h4>📊 Measurable Impact</h4>
        <div class="metrics-grid">
          <div class="metric">
            <span class="metric-value">40%</span>
            <span class="metric-label">Reduction in Production Bugs</span>
          </div>
          <div class="metric">
            <span class="metric-value">2</span>
            <span class="metric-label">Fully Automated Projects</span>
          </div>
          <div class="metric">
            <span class="metric-value">100%</span>
            <span class="metric-label">Quality Culture Adoption</span>
          </div>
        </div>
        <div class="additional-impacts">
          <p>✅ Improved deployment frequency and confidence</p>
          <p>✅ Fostered strong quality culture with cross-team accountability</p>
          <p>✅ Reduced project bottlenecks during testing phase</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="cta-section">
  <p>Want to know more about these projects or discuss similar challenges?</p>
  <a href="/#contact" class="cta-button">Let's Connect</a>
</div>