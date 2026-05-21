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
  
  /* DEBUG: Turn the menu bright red so we can see it */
  .menu-column ul {
    background: red !important;
    column-count: 2 !important;
    column-gap: 2rem !important;
  }
  
  /* Photo styles */
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

  /* Method 1: Style the theme's existing navigation menu */
  .site-nav ul,
  .menu ul,
  nav:first-of-type ul {
    column-count: 2 !important;
    column-gap: 2rem !important;
    list-style: none !important;
    padding-left: 0 !important;
    margin-bottom: 1rem !important;
  }
  
  .site-nav li,
  .menu li,
  nav:first-of-type li {
    break-inside: avoid !important;
    margin-bottom: 0.5rem !important;
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
