---
title: 'MADS: Ensemble LLM-based Multi-Agent Debate System for Political Bias Detection'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Benjamin C. M. Fung
- Elena Obukhova
- D. Mouheb
- C. Huang
- S. Huang

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2025-10-07T00:00:00Z'
# doi: 'https://doi.org/10.1145/3680207.3723472'

# Schedule page publish date (NOT publication's date).
publishDate: '2025-10-07T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: "Submitted to *DSAA 2026*"
publication_short: "Submitted to *DSAA 2026*"

abstract: |2-
  In the contemporary digital information ecosystem, algorithmic curation and social media amplification have transformed news consumption, creating echo chambers that reinforce partisan narratives and making it increasingly difficult for readers to identify biased reporting. Political bias detection presents fundamental challenges: news articles interweave facts, opinions, and selective framing across thousands of words, where subtle omissions and word choices can be as influential as explicit statements. Traditional supervised approaches require costly expert annotations that struggle to keep pace with the volume and evolution of online content. We introduce an unsupervised framework leveraging multi-agent debate among large language models to detect political bias without training data. By orchestrating structured deliberation among three diverse LLMs, our approach enables models to challenge each other's interpretations through evidence-based argumentation, exposing biases that individual models miss while providing interpretable reasoning chains. Across comprehensive evaluations on 3 separate datasets (totalling over 7,000 articles) from major U.S. media outlets, our framework achieves competitive performance with unsupervised methods on expert-annotated datasets while outperforming established supervised baselines from prior work. We also contribute a benchmark of 473,989 articles collected during the 2024 U.S. election period. This work demonstrates that multi-agent deliberation can transform political bias detection from an annotation-dependent task to an unsupervised reasoning problem, providing transparent, evidence-grounded classifications essential for media literacy in democratic discourse.

# Summary. An optional shortened abstract.
summary: 

tags:
- Political Bias Detection
- Large Language Models
- Model Ensemble
- Unsupervised Learning

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'MADS'
  # caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
