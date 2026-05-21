---
layout: home
title: Home
---

<style>
  /* Main two-column layout for content */
  .two-column {
    display: flex;
    gap: 3rem;
    flex-wrap: wrap;
  }
  
  .photo-column, .menu-column {
    flex: 1;
    min-width: 250px;
  }
  
  /* METHOD 1: Style the existing theme navigation menu in two columns */
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
  
  /* Photo styles */
  .profile-photo {
    width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  }
  
  .refresh-button {
    margin-top: 1rem;
    padding: 0.5rem 1rem;
    cursor: pointer;
    background: #f0f0f0;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .refresh-button:hover {
    background: #e0e0e0;
  }
  
  /* Optional: Add some spacing for better readability */
  .menu-column h1:first-of-type {
    margin-top: 0;
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
