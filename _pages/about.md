---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  p.bio a { color: inherit !important; text-decoration: underline dotted #9aa0a6 !important; text-underline-offset: 3px; }
  p.bio a:hover { text-decoration: underline solid currentColor !important; }
  ul.cv-list { list-style: none; margin-left: 0; padding-left: 0; }
  ul.cv-list li { display: flex; justify-content: space-between; gap: 1.5em; }
  ul.cv-list .cv-years { white-space: nowrap; color: #666; }
</style>

I am a final-year PhD student working at the [Robotics Systems Lab](https://www.acin.tuwien.ac.at/en/robotic-systems-lab/), TU Wien, under the supervision of [Prof. Christian Ott](https://www.acin.tuwien.ac.at/en/staff/cott/). My research focuses on combining **optimization-based control** with **reinforcement learning** to enable safe physical interaction of underactuated **aerial manipulators** in uncertain environments.  Previously, I was a research engineer in [Prof. Antonio Franchi](https://people.utwente.nl/a.franchi)'s group at the University of Twente, working on model predictive control for aerial-robotic systems. I completed a MSc in Aerospace Engineering from the Delft University of Technology, with a specialization in control and simulation. 
{: .bio}

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

Education
======
<ul class="cv-list">
  <li><span>Ph.D in Electrical Engineering from Vienna University of Technology, Austria</span><span class="cv-years">2022 – Present</span></li>
  <li><span>M.Sc in Aerospace Engineering from Delft University of Technology, The Netherlands</span><span class="cv-years">2018 – 2020</span></li>
  <li><span>B.Tech in Electrical Engineering from National Institute of Technology, Silchar, India</span><span class="cv-years">2012 – 2016</span></li>
</ul>

Experience
======
-  PhD Researcher at Vienna University of Technology, Austria (2022 - Present)
-  Research Engineer at University of Twente, The Netherlands (2020 - 2022)
-  Research Internship at German Aerospace Center (DLR), Germany (2019)
-  Project Engineer at Indian Institute of Science, India (2017-2018)
-  Project Engineer at Indian Institute of Technology, Bombay, India (2016)
