---
layout: home
title: Home
---

<style>
  /* Drastically reduce navigation menu space */
  .site-nav, 
  .menu,
  nav {
    margin: 0 !important;
    padding: 0 !important;
    line-height: 1 !important;
  }
  
  .site-nav ul,
  .menu ul,
  nav ul {
    margin: 0 !important;
    padding: 5px 0 !important;
    display: flex !important;
    flex-wrap: wrap !important;
    gap: 10px 20px !important;
    justify-content: flex-start !important;
  }
  
  .site-nav li,
  .menu li,
  nav li {
    margin: 0 !important;
    padding: 0 !important;
  }
  
  .site-nav a,
  .menu a,
  nav a {
    padding: 0 !important;
    font-size: 0.9rem !important;
  }
  
  /* Remove any containers that add space */
  .wrapper,
  .main,
  .content,
  header {
    margin-top: 0 !important;
    padding-top: 0 !important;
  }
  
  /* Main two-column layout */
  .two-column {
    display: flex;
    gap: 3rem;
    flex-wrap: wrap;
    margin-top: 10px !important;
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
