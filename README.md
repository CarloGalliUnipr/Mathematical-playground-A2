# A.2 — The Mathematical Playground

A self-contained interactive laboratory for **Computational Morphology, Module A.2 — Mathematical Foundations**.

## What's included

- **Experiment 1 — Functions & graphs:** sliders for `a` and `b`, linear and quadratic functions, interactive graph, two automatically checked conceptual questions.
- **Experiment 2 — Growth & decay:** exponential population model, positive/negative rate, adjustable initial population, linear/logarithmic vertical scale, doubling time and half-life, two self-checks.
- **Experiment 3 — Spatial gradients & images:** concentration profile, adjustable initial concentration and characteristic length, synthetic 8 × 12 intensity matrix, pixel inspector, two self-checks.

Students need **no software installation, login, or programming experience**. All graphics and controls are implemented in plain HTML, CSS, and JavaScript with no outside libraries or CDN resources.

## Preview locally

Open `index.html` in a modern browser. There is no server or build step.

## Publish on GitHub Pages (web interface)

1. Create a new **public** GitHub repository, such as `a2-mathematical-playground`.
2. Upload the contents of this folder (especially `index.html`) to the **root** of the repository, then commit.
3. Go to **Settings → Pages** in the repository.
4. Under **Build and deployment**, choose **Deploy from a branch**; select `main` and `/(root)`; save.
5. The site should be available at `https://YOUR-USERNAME.github.io/a2-mathematical-playground/` once GitHub completes deployment. Find the exact site URL in the Pages settings.
6. Post this URL in the course platform or link it from the chapter A.2 page.

Alternatively, add `index.html` to a pre-existing Pages repository. If the site is a **project site**, the path depends on the repository name.

## Assessment and privacy

- Self-checks give **automatic feedback** and can be retried until correct.
- Completion of each of the six checks is stored **locally in the student's browser**, when browser storage is available. Students can reset this.
- **No grades or responses are submitted to the instructor.** GitHub Pages is static hosting, not a learning-management backend; this file is intended for formative assessment, not an auditable gradebook.
- The lab has no analytics, trackers, form submissions, API calls, or remote resources.
- If a graded record is required later, use the learning platform's own quiz/SCORM capabilities or a secure backend instead of relying on client-side data.

## Teaching scope

This lab complements the A.2 student notes and does **not** include the old confusing “Assignment A1” label. Its experiments are independent, explanatory, and deliberately avoid solving differential equations, numerical integration, or reaction–diffusion models, which belong to later chapters.

### Mathematical conventions

- `N(t) = N₀ exp(rt)`, with time in days and `r` in inverse days.
- `c(x) = c₀ exp(−x/ℓ)`, with position and `ℓ` measured in millimeters.
- The image matrix represents **synthetic concentration-correlated intensities**, not empirical microscopy. Small row-to-row modulation is included to make the heatmap look like a 2D dataset; it is not a mechanistic model.
- Exponential functions are unrestricted idealizations; they need not remain biologically valid indefinitely.

## Editing

All user-facing text, styles, calculations and questions are in `index.html`. Search for the `checks` array to edit the six concept questions. No package installation or bundler is required.
