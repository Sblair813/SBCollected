---
layout: default
title: Home
---

<style>
  /* Hides the default theme header bar on the homepage */
  .site-header { display: none !important; }
</style>

<!-- 1. ABOUT ME SECTION -->
## Technology Leadership & Product Architecture

I'm a technology leader who has worked as a de facto Product Manager and Solutions Architect, specializing in enterprise supply chain systems, ERP environments, and complex integrations. I bridge the gap between operational reality and software design by owning products, architecting practical solutions, and managing end-to-end delivery of business-critical systems across WMS, TMS, ERP, and fulfillment operations.<img width="468" height="100" alt="image" src="https://github.com/user-attachments/assets/5fd0818e-4bf7-4d94-868a-e1fdd81bad08" />



### Tools & Platforms

**Enterprise Systems:** Microsoft Dynamics 365 • Infor M3 • Körber One (WMS) • Home-Grown / Custom-Built Systems • WMS • WFM • TMS • ERP

**Data & Reporting:** SQL • Power BI • SSRS • HighJump

**Development & Testing:** JavaScript • Visual Studios • SQL • End-to-End System Validation 

**AI & Automation:** Claude (Generative AI) • AI Workflow Automation • Agentic AI

**Product & Delivery:** Jira • Confluence • ServiceNow • xMatters • Agile / Scrum

**Design & Collaboration:** Figma • Lucidchart • Visio • Mural • Process Mapping

---

### Connect

<a href="https://www.linkedin.com/in/susan-b-122067147/" target="_blank" rel="noopener" style="display: inline-flex; align-items: center; background-color: #0077b5; color: #ffffff; font-weight: 600; font-size: 0.875rem; padding: 8px 16px; border-radius: 6px; text-decoration: none; margin-top: 8px;">
  Connect on LinkedIn &rarr;
</a>

<br><br>

---

<!-- 2. ARTICLES SECTION -->
<section class="articles-section" style="margin-bottom: 36px; padding-bottom: 24px; border-bottom: 1px solid #e2e8f0;">

<h2 style="font-size: 1.5rem; font-weight: 600; color: #0f172a; margin-bottom: 20px;">
  Articles
</h2>

<ul style="list-style: none; padding: 0; margin: 0;">
  {% for post in site.posts %}
    <li style="border-bottom: 1px solid #f1f5f9; padding: 12px 0; display: flex; justify-content: space-between; align-items: center;">
      <a href="{{ post.url | relative_url }}" style="font-size: 1rem; font-weight: 500; color: #2563eb; text-decoration: none;">
        {{ post.title | escape }}
      </a>
      <span style="font-size: 0.85rem; color: #64748b;">
        {{ post.date | date: "%b %d, %Y" }}
      </span>
    </li>
  {% else %}
    <li style="color: #64748b; font-style: italic;">No articles published yet.</li>
  {% endfor %}
</ul>

</section>
<!-- 3. TECHNICAL SCRIPTS & ANALYSIS SECTION -->
<section class="scripts-section" style="margin-bottom: 36px; padding-bottom: 24px; border-bottom: 1px solid #e2e8f0;">

<h2 style="font-size: 1.5rem; font-weight: 600; color: #0f172a; margin-bottom: 20px;">
  Technical Scripts & Analysis
</h2>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px;">
  
  <div style="background: #ffffff; border: 1px solid #e2e8f0; border-radius: 8px; padding: 20px;">
    <h3 style="font-size: 1.05rem; font-weight: 600; margin-top: 0; margin-bottom: 8px; color: #0f172a;">
      Order Fulfillment Troubleshooting Script
    </h3>
    <p style="font-size: 0.9rem; color: #475569; margin-bottom: 12px; line-height: 1.5;">
      Python automation to identify order stuck states, validate payload mappings, and resolve integration routing errors across OMS/WMS workflows.
    </p>
    <a href="https://github.com/sblair813/SBCollected/blob/main/scripts/sample_sql_troubleshoot.py" target="_blank" rel="noopener" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">View Code on GitHub &rarr;</a>
  </div>

  <div style="background: #ffffff; border: 1px solid #e2e8f0; border-radius: 8px; padding: 20px;">
    <h3 style="font-size: 1.05rem; font-weight: 600; margin-top: 0; margin-bottom: 8px; color: #0f172a;">
      QC Observation Data Collector
    </h3>
    <p style="font-size: 0.9rem; color: #475569; margin-bottom: 12px; line-height: 1.5;">
      Python utility designed to capture, parse, and categorize warehouse picking and packing audit exceptions during quality control sweeps.
    </p>
    <a href="https://github.com/sblair813/SBCollected/blob/main/scripts/qc_observation.py" target="_blank" rel="noopener" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">View Code on GitHub &rarr;</a>
  </div>

</div>

</section>

<!-- 4. PROJECTS AND PURSUITS SECTION -->
<section class="projects-section" style="margin-bottom: 36px;">

<h2 style="font-size: 1.5rem; font-weight: 600; color: #0f172a; margin-bottom: 20px;">
  Projects and Pursuits
</h2>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px;">
  {% assign count = 0 %}
  {% for project in site.pages %}
    {% if project.path contains 'projects/' and project.name != 'index.md' %}
      {% assign count = count | plus: 1 %}
      <div style="background: #ffffff; border: 1px solid #e2e8f0; border-radius: 8px; padding: 20px;">
        <h3 style="font-size: 1.05rem; font-weight: 600; margin-top: 0; margin-bottom: 8px; color: #0f172a;">
          {{ project.title | escape }}
        </h3>
        {% if project.description %}
          <p style="font-size: 0.9rem; color: #475569; margin-bottom: 12px; line-height: 1.5;">
            {{ project.description }}
          </p>
        {% endif %}
        <a href="{{ project.url | relative_url }}" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">View Project &rarr;</a>
      </div>
    {% endif %}
  {% endfor %}

  {% if count == 0 %}
    <div style="padding: 16px; color: #64748b; font-style: italic;">
      Projects folder contents will appear here once created.
    </div>
  {% endif %}
</div>

</section>

