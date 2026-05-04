# 暨南大学经济学院研究生毕业论文格式与写作规范自查工具

Jinan University School of Economics Graduate Thesis Format and Writing Self-Check Tool

## Overview

This project is a GitHub Pages-ready static web tool for graduate students in the College of Economics, Jinan University, to self-check thesis writing and formatting requirements. It supports a manual checklist, local DOCX / PDF / TEX preliminary checks, Markdown self-check report export, and a Chinese / English interface.

The project is fully static. It does not require a backend server, database, Node.js build pipeline, or complex deployment workflow.

This tool is a self-check aid and reference tool only. It is not an official Jinan University or college review system. The automatic check uses rule-based detection and risk prompts, so results should be understood cautiously as “possibly missing,” “suggested manual confirmation,” or “preliminary judgment.” It cannot replace formal college review, official university documents, or supervisor guidance.

## Project Structure

- `index.html`: New default page for GitHub Pages.
- `index_old.html`: Preserved legacy page. Only a return link to the new page has been added.
- `resources/`: Directory for reference PDF materials.
- `resources/thesis_writing_and_defense_notes.pdf`: PDF notes on thesis writing, defense preparation, and data search experience. Thanks to Pei Tiancheng for providing the related materials.
- `jnu_logo.png`: Jinan University logo shown near the footer.
- `.nojekyll`: GitHub Pages static deployment marker.
- `README.md`: Project documentation.

## Features

- Manual thesis format checklist with “Passed / Needs revision / N/A / Unchecked” states.
- Local browser parsing for DOCX / PDF / TEX files.
- Direct LaTeX source paste-in for rule-based checks.
- Risk prompts for structure, abstract, keywords, chapters, figures, tables, equations, citations, and references.
- Search, status filtering, risk-level filtering, and revision notes.
- Markdown self-check report export, including automatic check summary and manual checklist status.
- `localStorage` saves only manual checklist states and notes; uploaded thesis content is not saved to `localStorage` and is not uploaded to any server.
- Chinese / English interface switching, with the selected language remembered in the browser.

## Thanks

The content of this tool mainly draws on thesis writing and format-checking materials accumulated by previous senior students. Special thanks go to Pei Tiancheng, Lin Xingguang, and others for their systematic work on related checklists, writing experience, and reference materials, which provided an important foundation for this tool.

Sincere thanks are also extended to Professor Ouyang for guidance and support in graduate thesis writing standards and academic training.

On the basis of these materials, Yang Jie integrated and structured the relevant content, implemented it as a web-based tool, and is responsible for the tool design, feature development, and ongoing maintenance.

## Scope and Disclaimer

This tool is mainly intended as a self-check aid for graduate thesis writing and formatting in the College of Economics, Jinan University. Requirements may differ across colleges or programs, so please follow your college’s official requirements, the latest university documents, and your supervisor’s advice.

This tool is not an official university or college review system and does not claim to replace college review, supervisor feedback, or official documents. Automatic checks cannot cover every formatting, content, or layout issue. Details such as margins, page numbers, fonts, headers, footers, figure/table placement, and reference formatting still require manual verification.

## Deployment to GitHub Pages

1. Create or open a GitHub repository.
2. Upload `index.html`, `index_old.html`, `README.md`, `jnu_logo.png`, `resources/`, and `.nojekyll` to the repository root.
3. Go to repository `Settings` -> `Pages`.
4. Set Source to `Deploy from a branch`.
5. Select branch `main` and folder `/root`.
6. Save the settings and wait for GitHub Pages to finish deployment.

If the logo is not displayed, confirm that `jnu_logo.png` is in the repository root together with `index.html`. If the reference material link does not open, confirm that `resources/thesis_writing_and_defense_notes.pdf` has been uploaded to the `resources/` directory.

## Local Use

Open `index.html` directly in a browser. If the browser or network environment blocks CDN scripts, DOCX / PDF automatic parsing may be unavailable and the page will show a warning. The manual checklist, LaTeX text check, and report export can still be used.

## Author

Author / Maintainer: 杨杰（Jie Yang）  
Email: jieyang020618@gmail.com  
Copyright: © 2026 杨杰 Jie Yang. All rights reserved.

No open-source license is declared for this project. Without the author’s permission, copying, modification, redistribution, or commercial use is not permitted.
