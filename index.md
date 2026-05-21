---
layout: home
title: Home
---

<style>
  /* Main two-column layout */
  .two-column {
    display: flex;
    gap: 3rem;
    flex-wrap: wrap;
  }
  
  .photo-column, .menu-column {
    flex: 1;
    min-width: 250px;
  }
  
  /* Multi-column menu - THIS IS THE NEW ADDITION */
  .menu-column .menu {
    column-count: 2;
    column-gap: 2rem;
    list-style: none;
    padding-left: 0;
  }
  
  .menu-column .menu li {
    break-inside: avoid;
    margin-bottom: 0.5rem;
  }
  
  /* Your existing photo styles */
  .profile-photo {
    width: 100%;
    height: auto;
    border-radius: 8px;
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
    <h1>Hi, I'm Cooper</h1>
    <p>Welcome to my portfolio. I'm passionate about [your interests].</p>
    
    <hr>
    
    <h2>Featured Projects</h2>
    <ul>
      <li><a href="/project1/">Project 1</a></li>
      <li><a href="/project2/">Project 2</a></li>
      <li><a href="/project3/">Project 3</a></li>
    </ul>
    
    <hr>
    
    <p><a href="/projects/">View all projects →</a></p>
  </div>
</div>
