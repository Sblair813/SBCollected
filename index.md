---
layout: default
title: Home
---

<style>
  /* Hides the default theme header bar on the homepage */
  .site-header { display: none !important; }
</style>

<!-- 1. ABOUT ME SECTION -->
<section style="margin-bottom: 32px;">
  <h2 style="font-size: 1.5rem; font-weight: 600; color: #0f172a; margin-bottom: 8px;">
    Technology Leadership & Product Architecture
  </h2>

  <p style="font-size: 1rem; color: #475569; line-height: 1.6; margin-bottom: 16px;">
    Demonstrating enterprise IT Product Management, Supply Chain integration architectures, and automated Knowledge Governance frameworks.
  </p>

  <details style="background: #ffffff; border: 1px solid #e2e8f0; border-radius: 8px; padding: 16px 20px; cursor: pointer;">
    <summary style="font-size: 0.9rem; font-weight: 600; color: #2563eb; user-select: none;">
      View Tools, Platforms & Technical Core Competencies &rarr;
    </summary>
    
    <div style="margin-top: 16px; font-size: 0.9rem; color: #334155; line-height: 1.6;">
      <p style="margin-bottom: 10px;">
        <strong>Enterprise Systems:</strong> Microsoft Dynamics 365 • Infor M3 • Körber One (WMS) • Home-Grown and Custom-Built Systems • WMS • WFM • TMS • ERP
      </p>
      <p style="margin-bottom: 10px;">
        <strong>Data & Reporting:</strong> SQL • Power BI • SSRS • HighJump
      </p>
      <p style="margin-bottom: 10px;">
        <strong>Development & Testing:</strong> JavaScript • Visual Studio • SQL • End-to-End System Validation
      </p>
      <p style="margin-bottom: 10px;">
        <strong>AI & Automation:</strong> Claude (Generative AI) • AI Workflow Automation • Agentic AI
      </p>
      <p style="margin-bottom: 10px;">
        <strong>Product & Delivery:</strong> Jira • Confluence • ServiceNow • xMatters • Agile / Scrum
      </p>
      <p style="margin-bottom: 0;">
        <strong>Design & Collaboration:</strong> Figma • Lucidchart • Visio • Mural • Process Mapping
      </p>
    </div>
  </details>
</section>

<hr style="border: 0; border-top: 1px solid #e2e8f0; margin-bottom: 32px;" />

---
<!-- 2. CONNECT SECTION -->
<section class="connect-section" style="margin-bottom: 32px;">

  <h2 style="font-size: 1.25rem; font-weight: 600; color: #0f172a; margin-bottom: 12px;">
    Connect
  </h2>

  <a href="https://www.linkedin.com/in/susan-b-122067147/" target="_blank" rel="noopener" style="display: inline-flex; align-items: center; background-color: #0077b5; color: #ffffff; font-weight: 600; font-size: 0.875rem; padding: 10px 18px; border-radius: 6px; text-decoration: none; transition: background-color 0.2s ease;">
    Connect on LinkedIn &rarr;
  </a>

</section>

<hr style="border: 0; border-top: 1px solid #e2e8f0; margin-bottom: 32px;" />

<!-- 3. ARTICLES SECTION -->
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
<!-- 4. TECHNICAL SCRIPTS & ANALYSIS SECTION -->
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

<!-- 5. KNOWLEDGE MANAGEMENT -->
<section class="km-section" style="margin-bottom: 36px;">

<h2 style="font-size: 1.5rem; font-weight: 600; color: #0f172a; margin-bottom: 20px;">
  Knowledge Management
</h2>

<div style="background: #ffffff; border: 1px solid #e2e8f0; border-radius: 8px; padding: 24px;">
  <h3 style="font-size: 1.15rem; font-weight: 600; margin-top: 0; margin-bottom: 10px; color: #0f172a;">
    Enterprise Knowledge Management Framework
  </h3>
  <p style="font-size: 0.95rem; color: #475569; margin-bottom: 16px; line-height: 1.6;">
    A production-grade 4-pillar Information Architecture model featuring YAML front-matter metadata schemas, controlled taxonomy dictionaries, semantic system ontologies, and automated lifecycle governance policies.
  </p>
  
  <div style="display: flex; gap: 16px; flex-wrap: wrap;">
    <a href="/SBCollected/KM/Governance/GOVERNANCE.html" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">Governance & Policies &rarr;</a>
    <a href="/SBCollected/KM/Taxonomy/TAXONOMY.html" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">Taxonomy & Metadata &rarr;</a>
    <a href="/SBCollected/KM/Ontology/SYSTEM_ONTOLOGY.html" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">System Ontology &rarr;</a>
  </div>
</div>

</section>


<!-- 6. PROJECTS AND PURSUITS SECTION -->
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
        <a href="{{ project.path | replace: '.md', '' | relative_url }}" style="font-size: 0.875rem; font-weight: 600; color: #2563eb; text-decoration: none;">View Project &rarr;</a>
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

