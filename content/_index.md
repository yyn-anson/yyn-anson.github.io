---
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "5rem"

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/resume.pdf

  - block: markdown
    content:
      title: Research
      subtitle: ""
      text: |-
        I am an incoming M.S. student in Computer Science at Stanford University and a research trainee at Mila - Quebec AI Institute. My work focuses on reliable machine learning systems for high-stakes and socially consequential settings.

        **Current focus**

        - **Multimodal medical AI:** privacy-preserving MLLM agents for personalized multiple-sclerosis lesion-activity prognosis from clinical narratives and MRI.
        - **Trustworthy and interpretable learning:** evidence-grounded workflows, model failure analysis, and multimodal decision representations.
        - **Computational social science:** political-bias detection, misinformation analysis, and multi-agent LLM systems.
        - **Fair decision systems:** resource allocation under diversity constraints and explainable graph learning.

        At Mila, I work with Professor Tal Arbel on a local retrieval-synthesis-critique system and methods for identifying systematic failure subgroups. My previous research spans fair resource allocation and psychosis prediction at UBC, political-bias detection at McGill, and mobile glucose sensing at SFU.

        [View featured publications](#papers) | [Explore selected projects](/projects/) | [Review research experience](/experience/)
    design:
      columns: "1"

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 1
---
