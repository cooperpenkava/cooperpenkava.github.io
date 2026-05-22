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
    <p>I'm a Mechanical Engineer studying at Olin College of Engineering. I want to make tools that help build a better world. I'm also passionate about exploring the world through my creativity.</p>
    
    <hr>
    
    <h2>My Favorite Projects</h2>
    <ul>
      <li><a href="/projects/stirling-engine/">Custom-Built Stirling Engine</a></li>
      <li><a href="/projects/motor-tester/">Robotic Arm Test Fixture</a></li>
      <li><a href="/projects/swish/">Make a Basket Every Time!</a></li>
    </ul>
    
    <p><a href="/projects/">View all projects →</a></p>
    <p><a href="/creative/">See my creative endeavors →</a></p>
  </div>
</div>
