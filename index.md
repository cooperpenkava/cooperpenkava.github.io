---
layout: home
title: Home
---

<style>
  /* Force the navigation menu to be horizontal BUT contained */
  .site-nav ul,
  .menu ul,
  nav ul {
    display: flex !important;
    flex-wrap: wrap !important;
    gap: 1rem !important;
    list-style: none !important;
    padding: 0 !important;
    margin: 0 0 1rem 0 !important;
  }
  
  /* Make each bullet only as wide as its content */
  .site-nav li,
  .menu li,
  nav li {
    display: inline-block !important;
    width: auto !important;
    margin: 0 !important;
    padding: 0 !important;
  }
  
  /* Remove any block-level styling */
  .site-nav a,
  .menu a,
  nav a {
    display: inline-block !important;
    white-space: nowrap !important;
  }
  
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
  
  .menu-column h1:first-of-type {
    margin-top: 0;
  }
  
  /* Make navigation container respect column width */
  .photo-column nav:first-of-type {
    margin-bottom: 1.5rem;
  }
</style>

<div class="two-column">
  <div class="photo-column">
    <!-- Navigation moved here -->
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/engineering/">Engineering Projects</a></li>
        <li><a href="/creative/">Creative Endeavors</a></li>
        <!-- Add more navigation items as needed -->
      </ul>
    </nav>
    
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
