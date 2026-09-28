---
layout: about
title: about
permalink: /
subtitle: liyanyang3-c AT my DOT cityu DOT edu DOT hk

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  link: https://ant.isi.edu/~songxiao/
  more_info: >
    <p>Taken with my friend Xiao in Wuhan.</p>
    <p>Can't wait for her to find this. :)</p>

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
  .profile {
    width: 220px;
    max-width: 100%;
  }
  .profile a.profile-link {
    display: block;
    cursor: pointer;
  }
  .profile .more-info {
    font-family: inherit;
    font-size: 0.85rem;
    line-height: 1.4;
    margin-top: 0.45rem;
  }
  .profile .more-info p {
    display: block;
    margin: 0;
  }
  .profile .more-info p + p {
    margin-top: 0.2rem;
  }
  @media (hover: hover) {
    .profile {
      position: relative;
    }
    .profile .more-info {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      margin: 0;
      padding: 0.45rem 0.55rem;
      background: rgba(255, 255, 255, 0.94);
      color: #1a1a1a;
      border-radius: 0 0 0.25rem 0.25rem;
      opacity: 0;
      transition: opacity 0.2s ease;
      pointer-events: none;
    }
    .profile:hover .more-info,
    .profile:focus-within .more-info {
      opacity: 1;
    }
  }
  @media (min-width: 576px) {
    .profile {
      width: 280px;
    }
  }
  @media (max-width: 575px) {
    .profile {
      float: none !important;
      width: 220px;
      margin: 0 0 1rem;
    }
  }
</style>

Hi! I’m Liyan. I’m a fourth-year Ph.D. candidate at CityU DS, advised by [Prof. Kaidi Xu](https://kaidixu.com/).

My research focuses on post-training for LLMs, especially personalized preference alignment.

I previously obtained my Master’s degree from Southeast University and my undergraduate degree from Xidian University.

In my free time, I enjoy painting in the Western style (watercolor and charcoal drawing) and playing Chinese chess. You can check out my [portfolio]({{ '/portfolio/' | relative_url }}). If you’re also interested in chess, feel free to challenge me to a game!
