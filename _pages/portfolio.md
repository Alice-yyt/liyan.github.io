---
layout: page
title: Portfolio
permalink: /portfolio/
nav: false
nav_order: 5
---

<div class="portfolio">
  <div class="portfolio-piece">
    {% include figure.liquid loading="eager" path="assets/img/painting-still-life.jpg" alt="Still life with flowers and fruit" class="img-fluid rounded z-depth-1" max-width="420px" %}
  </div>

  <div class="pending-card pending-card--slow" role="img" aria-label="A painting that is still loading">
    <svg class="pending-icon" viewBox="0 0 48 48" aria-hidden="true">
      <rect x="6" y="10" width="36" height="28" rx="2" fill="none" stroke="currentColor" stroke-width="1.6"/>
      <circle cx="16" cy="20" r="3" fill="none" stroke="currentColor" stroke-width="1.6"/>
      <path d="M8 34l10-9 7 6 5-4 10 7" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linejoin="round"/>
    </svg>
    <p class="pending-label">Loading…</p>
    <div class="pending-bar" aria-hidden="true"><span></span></div>
  </div>
</div>

<style>
  .portfolio {
    max-width: 420px;
  }
  .portfolio figure {
    margin: 0 0 0.85rem;
  }
  .portfolio img {
    display: block;
    width: 100%;
    max-width: 100%;
    height: auto;
  }
  .pending-card {
    width: 100%;
    aspect-ratio: 768 / 1024;
    border-radius: 0.25rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0.85rem;
    color: color-mix(in srgb, var(--global-text-color) 62%, transparent);
    background: color-mix(in srgb, var(--global-text-color) 7%, var(--global-bg-color));
    border: 1px solid color-mix(in srgb, var(--global-text-color) 14%, transparent);
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
    overflow: hidden;
    position: relative;
  }
  .pending-card--slow::before {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(
      100deg,
      transparent 30%,
      color-mix(in srgb, var(--global-bg-color) 55%, transparent) 50%,
      transparent 70%
    );
    transform: translateX(-100%);
    animation: portfolio-shimmer 2.8s ease-in-out infinite;
  }
  .pending-icon {
    width: 2.4rem;
    height: 2.4rem;
    margin-bottom: 0.55rem;
    position: relative;
    z-index: 1;
  }
  .pending-label {
    margin: 0;
    position: relative;
    z-index: 1;
    font-size: 0.92rem;
  }
  .pending-bar {
    position: relative;
    z-index: 1;
    width: 46%;
    max-width: 11rem;
    height: 3px;
    margin-top: 0.7rem;
    border-radius: 999px;
    background: color-mix(in srgb, var(--global-text-color) 16%, transparent);
    overflow: hidden;
  }
  .pending-bar span {
    display: block;
    height: 100%;
    width: 22%;
    border-radius: inherit;
    background: color-mix(in srgb, var(--global-text-color) 55%, transparent);
    animation: portfolio-creep 3.6s ease-in-out infinite;
  }
  @keyframes portfolio-shimmer {
    0% { transform: translateX(-100%); }
    55%, 100% { transform: translateX(100%); }
  }
  @keyframes portfolio-creep {
    0%, 100% { width: 14%; }
    40% { width: 31%; }
    70% { width: 23%; }
  }
  @media (prefers-reduced-motion: reduce) {
    .pending-card--slow::before,
    .pending-bar span {
      animation: none;
    }
  }
</style>
