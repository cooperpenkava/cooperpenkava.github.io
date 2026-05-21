---
layout: home
title: Home
---

<style>
  /* Hide the theme's default navigation */
  .site-nav, 
  .main-nav,
  header nav,
  .header nav,
  .site-header nav {
    display: none !important;
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
  
  /* Custom navigation styles - vertical layout */
  .custom-nav ul {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    list-style: none;
    padding: 0;
    margin: 0 0 1.5rem 0;
  }
  
  .custom-nav li {
    margin: 0;
  }
  
  .custom-nav a {
    display: inline-block;
    padding: 0.25rem 0;
    text-decoration: none;
  }
  
  .custom-nav a:hover {
    text-decoration: underline;
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
    <!-- Navigation pulled from _config.yml -->
    <nav class="custom-nav">
      <ul>
        {% for item in site.navigation %}
          <li><a href="{{ item.url }}">{{ item.title }}</a></li>
        {% endfor %}
      </ul>
    </nav>
    
    {% include random-photo.html %}
  </div>
  
  <div class="menu-column">
    <p>Hey! I'm Cooper Penkava, and I'm a Mechanical Engineer studying at Olin College of Engineering. I want to make tools that help build a better world.</p>
    
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
