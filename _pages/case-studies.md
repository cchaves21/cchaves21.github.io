---
layout: page
title: Case Studies
permalink: /case-studies/
---

<style>
.hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 4rem 2rem;
  margin: -2rem -2rem 3rem -2rem;
  text-align: center;
  border-radius: 0 0 2rem 2rem;
}

.hero-title {
  font-size: 3rem;
  margin-bottom: 1rem;
  font-weight: 700;
}

.hero-subtitle {
  font-size: 1.2rem;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto;
}

.projects-grid {
  display: flex;
  flex-direction: column;
  gap: 3rem;
  margin-bottom: 3rem;
}

.project-card {
  background: white;
  border-radius: 1.5rem;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 2px solid #f0f0f0;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
}

.project-header {
  padding: 2rem;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
  position: relative;
}

.project-icon {
  font-size: 3rem;
  display: block;
  margin-bottom: 1rem;
}

.project-header h2 {
  margin: 0 0 1rem 0;
  color: #2d3748;
  font-size: 1.8rem;
  font-weight: 700;
}

.project-badge {
  position: absolute;
  top: 2rem;
  right: 2rem;
  padding: 0.5rem 1rem;
  border-radius: 2rem;
  font-size: 0.9rem;
  font-weight: 600;
  color: white;
}

.project-badge.brazil {
  background: linear-gradient(135deg, #00b09b, #96c93d);
}

.project-badge.uk {
  background: linear-gradient(135deg, #667eea, #764ba2);
}

.project-description {
  padding: 0 2rem;
  font-size: 1.1rem;
  line-height: 1.7;
  color: #4a5568;
}

.project-details {
  padding: 2rem;
}

.detail-section, .impact-section, .metrics-section {
  margin-bottom: 2rem;
}

.detail-section h4, .impact-section h4, .metrics-section h4 {
  color: #2d3748;
  margin-bottom: 1rem;
  font-size: 1.2rem;
  font-weight: 600;
}

.detail-section ul {
  list-style: none;
  padding: 0;
}

.detail-section li {
  padding: 0.5rem 0;
  padding-left: 1.5rem;
  position: relative;
  line-height: 1.6;
}

.detail-section li:before {
  content: "→";
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
}

.achievements {
  display: grid;
  gap: 1rem;
}

.achievement {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  padding: 1rem;
  background: #f7fafc;
  border-radius: 1rem;
  border-left: 4px solid #667eea;
}

.achievement.award {
  background: linear-gradient(135deg, #fef5e7, #fed7aa);
  border-left-color: #f6ad55;
}

.achievement-icon {
  font-size: 1.5rem;
  flex-shrink: 0;
}

.achievement strong {
  display: block;
  margin-bottom: 0.25rem;
  color: #2d3748;
}

.metrics-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1rem;
  margin-bottom: 1rem;
}

.metric {
  text-align: center;
  padding: 1.5rem;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  border-radius: 1rem;
  box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
}

.metric-value {
  display: block;
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
}

.metric-label {
  font-size: 0.9rem;
  opacity: 0.9;
}

.additional-impacts p {
  margin: 0.5rem 0;
  color: #4a5568;
  font-size: 0.95rem;
}

.cta-section {
  text-align: center;
  padding: 3rem 2rem;
  background: linear-gradient(135deg, #f7fafc, #edf2f7);
  border-radius: 1.5rem;
  margin-top: 2rem;
}

.cta-section p {
  font-size: 1.2rem;
  color: #4a5568;
  margin-bottom: 1.5rem;
}

.cta-button {
  display: inline-block;
  padding: 1rem 2rem;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  text-decoration: none;
  border-radius: 2rem;
  font-weight: 600;
  transition: all 0.3s ease;
  box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(102, 126, 234, 0.4);
  text-decoration: none;
  color: white;
}

@media (max-width: 768px) {
  .hero-section {
    padding: 2rem 1rem;
    margin: -1rem -1rem 2rem -1rem;
  }
  
  .hero-title {
    font-size: 2rem;
  }
  
  .project-header {
    padding: 1.5rem;
  }
  
  .project-badge {
    position: static;
    margin-top: 1rem;
    display: inline-block;
  }
  
  .project-details {
    padding: 1.5rem;
  }
  
  .metrics-grid {
    grid-template-columns: 1fr;
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
  <div class="project-card featured">
    <div class="project-header">
      <span class="project-icon">💸</span>
      <h2>Pix – A New Era of Payments</h2>
      <span class="project-badge brazil">Brazil • 2020</span>
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

  <div class="project-card featured">
    <div class="project-header">
      <span class="project-icon">🧭</span>
      <h2>Epos Now – Building a Culture of Quality</h2>
      <span class="project-badge uk">UK • 2022-Present</span>
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
  <a href="/contact/" class="cta-button">Let's Connect</a>
</div>