---
layout: home
title: Home
---

<style>
  /* Your custom two-column styles */
  .two-column {
    display: flex;
    gap: 3rem;
    flex-wrap: wrap;
  }
  
  .photo-column, .menu-column {
    flex: 1;
    min-width: 250px;
  }
  
  .refresh-button {
    margin-top: 1rem;
    padding: 0.5rem 1rem;
    cursor: pointer;
  }
</style>

<div class="two-column">
  <div class="photo-column">
    {% include random-photo.html %}
  </div>
  
  <div class="menu-column">
    # Hi, I'm Cooper
    <!-- rest of your content -->
  </div>
</div>
