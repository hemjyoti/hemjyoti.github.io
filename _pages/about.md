---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi there! I am a final-year PhD student working at the [Robotics Systems Lab](https://www.acin.tuwien.ac.at/en/robotic-systems-lab/), under the supervision of [Prof. Christian Ott](https://www.acin.tuwien.ac.at/en/staff/cott/). My research focuses on the control of underactuated aerial robots, in particular suspended aerial manipulators, for agile maneuvers and safe physical interaction with unknown environments. I combine optimization-based, task-prioritized whole-body control and passivity-based methods with residual reinforcement learning, and validate them in real-world experiments.  Previously, I worked with [Prof. Antonio Franchi](https://homepages.laas.fr/afranchi/robotics/?q=front_page) as a research engineer on aerial manipulation. I completed a MSc in Aerospace Engineering from the Delft University of Technology, with a specialization in control and simulation. 

Selected Publications
======

{% include base_path %}
{% include pub-styles.html %}
{% assign selected_pubs = site.publications | where: "selected", true | sort: "date" | reverse %}
<div class="pubs pubs-selected">
{% for p in selected_pubs %}
{% include pub-card.html %}
{% endfor %}
<p style="margin-top:1em;"><a href="{{ base_path }}/publications/" style="color:#b509ac;text-decoration:none;font-weight:700;">See the full list of publications &rarr;</a></p>
</div>

<script>
document.querySelectorAll('.pubs-selected').forEach(function (root) {
  root.addEventListener('click', function (e) {
    var tog = e.target.closest('[data-toggle]');
    if (tog) {
      var pub = tog.closest('.pub');
      var panel = pub.querySelector('[data-panel="' + tog.dataset.toggle + '"]');
      var open = !panel.classList.contains('open');
      pub.querySelectorAll('.pub-extra').forEach(function (p) { p.classList.remove('open'); });
      pub.querySelectorAll('[data-toggle]').forEach(function (b) { b.setAttribute('aria-expanded', 'false'); });
      if (open) { panel.classList.add('open'); tog.setAttribute('aria-expanded', 'true'); }
    }
    if (e.target.classList.contains('more')) { e.target.previousElementSibling.hidden = false; e.target.remove(); }
    if (e.target.classList.contains('copy')) {
      var txt = e.target.nextElementSibling.textContent;
      navigator.clipboard.writeText(txt).then(function () { e.target.textContent = 'Copied'; setTimeout(function () { e.target.textContent = 'Copy'; }, 1500); });
    }
  });
});
</script>

Experience
======
-  **PhD Researcher** at Vienna University of Technology, Austria (2022 - Present)
-  **Research Engineer** at University of Twente, The Netherlands (2020 - 2022)
-  **Research Internship** at German Aerospace Center (DLR), Germany (2019)
-  **Project Engineer** at Indian Institute of Science, India (2017-2018)
-  **Project Engineer** at Indian Institute of Technology, Bombay, India (2016)



Education
======
- **PhD in Aerial Robotics and Control** from Vienna University of Technology, Austria (2022 - Present)
- **Master of Science in Aerospace Engineering** from Delft University of Technology, The Netherlands (2018 - 2020)
- **Bachelor of Science in Electrical Engineering** from National Institute of Technology, Silchar, India (2012 - 2016)
