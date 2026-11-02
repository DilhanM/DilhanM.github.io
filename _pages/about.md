---
layout: about
title: About
permalink: /
subtitle: Department of Chemistry; University of Liverpool

profile:
  align: right
  image: liverpool.jpg
  image_circular: false # crops the image to make it circular

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
  /* Justify the bio text only (not the news or publication lists). */
  article > .clearfix p,
  #why-2 ~ p {
    text-align: justify;
  }

  /* Larger photo than the theme's default 30% width (desktop only; phones already show it full width). */
  @media (min-width: 576px) {
    article > .profile {
      width: 40%;
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

We are a newly established quantum computational chemistry group at the University of Liverpool. We design and implement quantum computing algorithms for chemistry and quantum machine learning.

An overview of our research aims, methods and recent highlights can be found on the [Research](/research/) page, and a full list of our publications on the [Publications](/publications/) page. You can meet the team on the [People](/people/) page, and if you are interested in working with us, see [Join Us](/join/).

**Research interests:** Theoretical and Computational Chemistry &middot; Quantum Machine Learning &middot; Tensor Network Methods (DMRG) &middot; Quantum Computing.

#### Why √2?

_A note from Dilhan._

As a new DPhil student, I inherited a large Fortran code for time-dependent DMRG simulations. These were the pre-LLM days, and the world was in lockdown. Naturally, this meant long nights of coffee and code.

√2 is an important number in quantum mechanics; it appears [everywhere](https://www.youtube.com/shorts/UmuMgA_RxnU). It turned out that the code I inherited had a bug where this number was not used consistently. After several hundred print statements, I finally traced it. It was one of the first times I felt the joy of solving a scientific problem myself, and that memory has stayed with me. As I start my own research group, it feels apt to remember why I do research in the first place.

For me, it is to find stray √2s.
