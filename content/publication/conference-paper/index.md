---
title: 'GlucoSense: Non-Invasive Glucose Monitoring using Mobile Devices'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Neha Sharma
  - Mariam Bebawy
  - admin
  - Mohamed Hefeeda

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2025-11-04T00:00:00Z'
doi: 'https://doi.org/10.1145/3680207.3723472'

# Schedule page publish date (NOT publication's date).
publishDate: '2025-11-04T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *The 31st Annual International Conference on Mobile Computing and Networking*
publication_short: In *ACM MOBICOM ’25*

abstract: |
  Regular glucose monitoring is crucial for diabetic patients to
  avoid the risk of health complications such as stroke, kidney
  failure, heart disease, and even death. Most current devices
  for measuring glucose are costly and painful. We propose
  GlucoSense, a non-invasive glucose sensing solution on mo-
  bile devices. GlucoSense builds on the fact that glucose is an
  optically active molecule, which interacts with various wave-
  lengths. We first conduct spectral analysis to demonstrate
  the feasibility of measuring glucose in the visible and near-
  infrared range (400–1000 nm), which is the range available
  on mobile devices. We also identify the relative importance
  of various spectral bands in this range. We further propose
  multiple practical designs for obtaining the required spectral
  bands for measuring glucose. We then design GlucoSense
  exploiting the sensing capabilities of modern smartphones
  combined with machine learning models. We conduct an
  ethics-approved user study with a diverse set of participants
  in terms of age, sex, ethnicity, and body mass index (BMI). We
  compare GlucoSense against a widely-used, FDA-approved
  glucose measuring device. Our results show that 80.4% of Glu-
  coSense predictions are within Zone A (clinically accurate),
  and the remaining 19.3% are in Zone B (clinically accept-
  able) of the Clarke Error Grid (CEG). In addition, 99.7% of
  the predictions are within the None and Slight risk zones
  of the Surveillance Error Grid (SEG), indicating their high
  accuracy. Both CEG and SEG are standard metrics for assess-
  ing glucose-measuring devices. These results were obtained
  by GlucoSense running on unmodified phones in realistic
  environments with diverse illuminations.

# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
  # - Large Language Models
  - Blood Glucose
  - Mobile Health
  - Hyperspectral Imaging

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
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  caption: ''
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

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
