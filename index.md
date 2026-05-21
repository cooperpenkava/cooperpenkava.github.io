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
  
  /* Method 2: Style the menu inside the right column */
  .menu-column nav ul {
    column-count: 2;
    column-gap: 2rem;
    list-style: none;
    padding-left: 0;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #eee;
  }
  
  .menu-column nav ul li {
    break-inside: avoid;
    margin-bottom: 0.5rem;
  }
  
  /* Optionally hide the original theme menu */
  .site-header nav, 
  .sidebar nav,
  .menu:not(.menu-column .menu) {
    display: none !important;
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
    background: #f0f0f0;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .refresh-button:hover {
    background: #e0e0e0;
  }
</style>

<div class="two-column">
  <div class="photo-column">
    {% include random-photo.html %}
  </div>
  
  <div class="menu-column">
    <!-- Method 2: Menu placed here -->
    <nav>
      <ul>
        {% for item in site.data.menu.entries %}
          <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
        {% endfor %}
      </ul>
    </nav>
    
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
