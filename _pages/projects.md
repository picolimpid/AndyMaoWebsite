---
layout: page
title: Projects
permalink: /projects/
nav: true
nav_order: 3
horizontal: false
---

<style>
  .project-link, .project-link:hover { text-decoration: none; color: inherit; }
  .project-card {
    display: flex; align-items: center; gap: 32px;
    border: 1px solid var(--global-divider-color); border-radius: 8px;
    background-color: var(--global-bg-color);
    transition: transform 0.15s, box-shadow 0.15s;
  }
  .project-link:hover .project-card { transform: translateY(-2px); }
  .project-thumb { flex: 0 0 200px; width: 200px; }
  .project-thumb img { width: 100%; aspect-ratio: 5 / 3; object-fit: cover; border-radius: 5px; display: block; }
  .project-body { flex: 1; min-width: 0; }
  .project-body .card-title { font-size: 1.25rem; color: var(--global-text-color); }
  .project-link:hover .card-title { color: var(--global-theme-color); }
  .project-body .card-text { font-size: 1rem; color: var(--global-text-color); margin-bottom: 0; }
  @media (max-width: 640px) {
    .project-card { flex-direction: column; align-items: stretch; gap: 16px; }
    .project-thumb { flex: none; width: 100%; }
  }
</style>

<!-- pages/projects.md -->

<div class="projects">
  <h2 class="category mb-4">Research Projects</h2>
  <div class="container">
    <div class="row mb-4">
      <div class="col-12 mb-4">
        <a href="https://github.com/picolimpid/HyDE-Fine-Tuning-for-Efficient-Query-Retrieval" target="_blank" class="d-block project-link">
          <div class="project-card p-4 shadow-sm">
            <div class="project-thumb">
              <img src="{{ '/assets/img/projects/hyde.svg' | relative_url }}" alt="HyDE Fine-Tuning for Efficient Query Retrieval">
            </div>
            <div class="project-body">
              <h5 class="card-title mb-3">HyDE Fine-Tuning for Efficient Query Retrieval</h5>
              <p class="card-text">Distills HyDE-style retrieval (LLM-generated hypothetical documents with mean-pooled embeddings) into a one-shot query encoder, so no LLM call is needed at retrieval time. Evaluated on 2WikiMultihopQA with FAISS dense retrieval, with the largest Recall@K gains on symmetric encoders such as Contriever and BGE.</p>
            </div>
          </div>
        </a>
      </div>

      <div class="col-12 mb-4">
        <a href="https://github.com/picolimpid/Dream-steam" target="_blank" class="d-block project-link">
          <div class="project-card p-4 shadow-sm">
            <div class="project-thumb">
              <img src="{{ '/assets/img/projects/steam.svg' | relative_url }}" alt="Was This Review Helpful? How Review Characteristics Shape Perceived Helpfulness on Steam">
            </div>
            <div class="project-body">
              <h5 class="card-title mb-3">Was This Review Helpful? How Review Characteristics Shape Perceived Helpfulness on Steam</h5>
              <p class="card-text">Uses a stratified propensity score design and repeated vote snapshots to study whether a reviewer who keeps playing after writing a review receives different helpful-vote counts, separately for positive and negative reviews.</p>
            </div>
          </div>
        </a>
      </div>

      <div class="col-12 mb-4">
        <a href="https://github.com/picolimpid/PRISM" target="_blank" class="d-block project-link">
          <div class="project-card p-4 shadow-sm">
            <div class="project-thumb">
              <img src="{{ '/assets/img/projects/prism.svg' | relative_url }}" alt="PRISM: Characterizing User Behavior on Bluesky">
            </div>
            <div class="project-body">
              <h5 class="card-title mb-3">PRISM: Characterizing User Behavior on Bluesky</h5>
              <p class="card-text">Builds user-level behavioral and linguistic feature matrices from Bluesky timelines (posting frequency, repost and reply ratios, interaction timing, readability, sentiment) and clusters users to characterize distinct patterns of online engagement.</p>
            </div>
          </div>
        </a>
      </div>

      <div class="col-12 mb-4">
        <a href="https://github.com/picolimpid/social-biases-T2I-models" target="_blank" class="d-block project-link">
          <div class="project-card p-4 shadow-sm">
            <div class="project-thumb">
              <img src="{{ '/assets/img/projects/t2i.svg' | relative_url }}" alt="Social Biases in Text-to-Image Models">
            </div>
            <div class="project-body">
              <h5 class="card-title mb-3">Social Biases in Text-to-Image Models</h5>
              <p class="card-text">Investigates demographic, occupational, and cultural biases in AI-generated images by testing diverse prompts and collecting feedback, and proposes strategies for fairer and more inclusive generated visuals.</p>
            </div>
          </div>
        </a>
      </div>
    </div>
  </div>
</div>
