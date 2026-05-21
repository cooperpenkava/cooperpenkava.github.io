---
layout: home
title: Home
---

<style>
  .two-column {
    display: flex;
    gap: 3rem;
    flex-wrap: wrap;
  }
  
  .photo-column, .menu-column {
    flex: 1;
    min-width: 250px;
  }
  
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

  /* Make the menu items display in two columns */
  .menu-column .menu {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.5rem 1rem;
    list-style: none;
    padding-left: 0;
  }
  
  /* Remove default bullet points */
  .menu-column .menu li {
    margin: 0;
    padding: 0;
  }
  
  /* Optional: Add a subtle border between columns */
  .menu-column .menu li:nth-child(even) {
    border-left: 1px solid #ddd;
    padding-left: 1rem;
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
