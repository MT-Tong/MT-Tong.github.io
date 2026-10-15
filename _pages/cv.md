---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
.cv-download-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7em;
  margin-bottom: 1.2em;
}

.cv-download-button {
  display: inline-flex;
  align-items: center;
  gap: 0.4em;
  padding: 0.5em 0.8em;
  border: 1px solid currentColor;
  border-radius: 4px;
  color: inherit;
  font-weight: 600;
  text-decoration: none;
}

.cv-download-button::before {
  content: "↓";
  font-weight: 700;
}

.cv-download-button:hover {
  opacity: 0.8;
  text-decoration: none;
}

.cv-preview-controls {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.6em;
  margin-bottom: 0.8em;
}

.cv-preview-label {
  font-weight: 600;
}

.cv-preview-button {
  padding: 0.4em 0.75em;
  border: 1px solid currentColor;
  border-radius: 4px;
  background: transparent;
  color: inherit;
  font: inherit;
  cursor: pointer;
}

.cv-preview-button.is-active {
  background: #333;
  color: #fff;
}

html[data-theme="dark"] .cv-preview-button.is-active {
  background: #fff;
  color: #111;
}

.cv-pdf-viewer {
  display: block;
  width: 100%;
  height: 1100px;
  border: 1px solid #d3d3d3;
}

html[data-theme="dark"] .cv-pdf-viewer {
  border-color: #666;
}

.cv-preview-fallback {
  margin-top: 0.7em;
  font-size: 0.9em;
}

@media (max-width: 768px) {
  .cv-pdf-viewer {
    height: 800px;
  }
}
</style>

<div class="cv-download-buttons" aria-label="Download CV">
  <a
    class="cv-download-button"
    href="{{ base_path }}/files/CV.pdf"
    download="Meilin_Tong_CV_short.pdf"
  >
    Download CV (short)
  </a>

  <a
    class="cv-download-button"
    href="{{ base_path }}/files/CV_long.pdf"
    download="Meilin_Tong_CV_long.pdf"
  >
    Download CV (long)
  </a>
</div>

<div class="cv-preview-controls" aria-label="Choose CV preview">
  <span class="cv-preview-label">Preview:</span>

  <button
    type="button"
    class="cv-preview-button is-active"
    data-cv-file="{{ base_path }}/files/CV.pdf"
    data-cv-title="Short version of Meilin Tong's CV"
    aria-controls="cv-pdf-viewer"
    aria-pressed="true"
  >
    Short version
  </button>

  <button
    type="button"
    class="cv-preview-button"
    data-cv-file="{{ base_path }}/files/CV_long.pdf"
    data-cv-title="Long version of Meilin Tong's CV"
    aria-controls="cv-pdf-viewer"
    aria-pressed="false"
  >
    Long version
  </button>
</div>

<iframe
  id="cv-pdf-viewer"
  class="cv-pdf-viewer"
  src="{{ base_path }}/files/CV.pdf"
  title="Short version of Meilin Tong's CV"
>
</iframe>

<p class="cv-preview-fallback">
  If the preview does not appear, 
  <a
    id="cv-preview-link"
    href="{{ base_path }}/files/CV.pdf"
    target="_blank"
    rel="noopener noreferrer"
  >open the selected CV in a new tab</a>.
</p>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const viewer = document.getElementById("cv-pdf-viewer");
  const previewLink = document.getElementById("cv-preview-link");
  const buttons = document.querySelectorAll(".cv-preview-button");

  buttons.forEach(function (button) {
    button.addEventListener("click", function () {
      const selectedFile = button.getAttribute("data-cv-file");
      const selectedTitle = button.getAttribute("data-cv-title");

      viewer.setAttribute("src", selectedFile);
      viewer.setAttribute("title", selectedTitle);
      previewLink.setAttribute("href", selectedFile);

      buttons.forEach(function (otherButton) {
        const isSelected = otherButton === button;

        otherButton.classList.toggle("is-active", isSelected);
        otherButton.setAttribute(
          "aria-pressed",
          isSelected ? "true" : "false"
        );
      });
    });
  });
});
</script>
