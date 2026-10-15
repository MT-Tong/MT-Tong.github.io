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
.cv-preview-controls {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.6em;
  margin-bottom: 1em;
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

.cv-preview-button:hover {
  opacity: 0.8;
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

@media (max-width: 768px) {
  .cv-pdf-viewer {
    height: 800px;
  }
}
</style>

<div class="cv-preview-controls" aria-label="Choose CV version">
  <span class="cv-preview-label">CV version:</span>

  <button
    type="button"
    class="cv-preview-button is-active"
    data-cv-file="{{ base_path }}/files/CV.pdf"
    data-cv-title="Short version of Meilin Tong's CV"
    aria-controls="cv-pdf-viewer"
    aria-pressed="true"
  >
    Short
  </button>

  <button
    type="button"
    class="cv-preview-button"
    data-cv-file="{{ base_path }}/files/CV_long.pdf"
    data-cv-title="Long version of Meilin Tong's CV"
    aria-controls="cv-pdf-viewer"
    aria-pressed="false"
  >
    Long
  </button>
</div>

<iframe
  id="cv-pdf-viewer"
  class="cv-pdf-viewer"
  src="{{ base_path }}/files/CV.pdf"
  title="Short version of Meilin Tong's CV"
>
</iframe>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const viewer = document.getElementById("cv-pdf-viewer");
  const buttons = document.querySelectorAll(".cv-preview-button");

  buttons.forEach(function (button) {
    button.addEventListener("click", function () {
      const selectedFile = button.getAttribute("data-cv-file");
      const selectedTitle = button.getAttribute("data-cv-title");

      viewer.setAttribute("src", selectedFile);
      viewer.setAttribute("title", selectedTitle);

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
