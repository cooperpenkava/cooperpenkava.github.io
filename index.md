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
  
  .profile-photo {
    max-width: 100%;
    height: auto;
  }
</style>

<div class="two-column">
  <div class="photo-column">
    <!-- {% include random-photo.html %} -->
    <p>Photo will go here temporarily</p>
  </div>
  
  <div class="menu-column">
    <h1>Hi, I'm Cooper</h1>
    
    <p>Welcome to my portfolio.</p>
    
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
