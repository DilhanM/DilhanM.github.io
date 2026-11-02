---
layout: about
title: About
permalink: /
subtitle: Department of Chemistry; University of Liverpool

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  /* Centre the group name and subtitle at the top of the page. */
  .post-header .post-title,
  .post-header .desc {
    text-align: center;
  }

  /* Justify the bio text only (not the news or publication lists). */
  article > .clearfix p,
  #why-2 ~ p {
    text-align: justify;
  }

  /* Photo floats right of the intro on desktop; full width on phones. */
  article figure {
    float: right;
    width: 40%;
    margin: 0.3rem 0 1rem 1.5rem;
  }
  @media (max-width: 575.98px) {
    article figure {
      float: none;
      width: 100%;
      margin: 0 0 1rem;
    }
  }
</style>

<script>
  // Move the "Why √2?" section below the news and publications lists, just above the social icons.
  document.addEventListener("DOMContentLoaded", () => {
    const heading = document.getElementById("why-2");
    const social = document.querySelector("article > .social");
    if (!heading || !social) return;
    const section = [heading];
    for (let el = heading.nextElementSibling; el; el = el.nextElementSibling) section.push(el);
    section.forEach((el) => social.before(el));
  });
</script>

{% include figure.liquid path="assets/img/liverpool.jpg" class="img-fluid rounded z-depth-1" alt="A snapshot of Liverpool's media wall with Radio City Tower in the background, as seen on the walk from Liverpool Lime Street towards the Department of Chemistry" %}

We are a newly established quantum computational chemistry group at the University of Liverpool. We design and implement quantum computing algorithms for chemistry and quantum machine learning.

An overview of our research aims, methods and recent highlights can be found on the [Research](/research/) page, and a full list of our publications on the [Publications](/publications/) page. You can meet the team on the [People](/people/) page, and if you are interested in working with us, see [Join Us](/join/).

**Research interests:** Theoretical and Computational Chemistry &middot; Quantum Machine Learning &middot; Tensor Network Methods (DMRG) &middot; Quantum Computing.

#### Why √2?

_A note from Dilhan._

As a new DPhil student, I inherited a large Fortran code for time-dependent DMRG simulations. These were the pre-LLM days, and the world was in lockdown. Naturally, this meant long nights of coffee and code.

√2 is an important number in quantum mechanics; it appears [everywhere](https://www.youtube.com/shorts/UmuMgA_RxnU). It turned out that the code I inherited had a bug where this number was not used consistently. After several hundred print statements, I finally traced it. It was one of the first times I felt the joy of solving a scientific problem myself, and that memory has stayed with me. As I build my own research group, it feels apt to remember why we do research in the first place.

For me, it is to find stray √2s.
