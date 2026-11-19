---
layout: about
title: about
permalink: /
subtitle: # e.g., <a href='#'>Affiliations</a>. Address. Contacts. Motto. Etc.

profile:
  align: right
  image: profile_pic.png
  image_circular: false # crops the image to make it circular
  more_info: >

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<div style="display: flex; gap: 8px; margin: 12px 0 24px 0; flex-wrap: wrap;">
  <a href="https://github.com/ramneekagn" class="btn btn-sm" role="button" target="_blank" rel="noopener noreferrer">
    <i class="fa-brands fa-github"></i>&nbsp; GitHub
  </a>
  <a href="https://www.linkedin.com/in/ramneek-agnihotri-1b6a8b380/" class="btn btn-sm" role="button" target="_blank" rel="noopener noreferrer">
    <i class="fa-brands fa-linkedin"></i>&nbsp; Linked In
  </a>
</div>


<!-- Write your biography below this line. -->

Masters student in Applied Computer Science at [Ruhr University Bochum](https://informatik.rub.de/) and Research Assistant at [Research Center for Trustworthy Data Science and Security](https://rc-trust.ai/).

You can reach me at: ramneek.agnihotri@edu.rub.de

Research directions: 
- AI Alignment and Safety
- Auditing LLMs through Interpretability methods 
- The foundations of Neural Networks
- Mechanistic Interpretability
- AI Ethics 

What is the nature of intelligence in large language models, and how do they make complex decisions? I want to approach these questions using the tools of interpretability and, with that understanding, build fairness and safety into AI models and prevent concrete harms such as cyberattacks and bias.

Furthermore I want to bridge technical research in interpretability with the practical and social frameworks from AI Ethics. 
As a tool I think mechanistic interpretability is crucial for AI alignment, as I don't believe we should deploy systems whose underlying causal
mechanisms we do not understand. As models become more capable, auditing them exclusively through black box analysis might become insufficient.

Currently I am working on 

<div class="projects">
  <div class="row row-cols-1 row-cols-md-2">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% for project in sorted_projects limit: 2 %}
    {% include projects.liquid %}
  {% endfor %}
  </div>
</div>