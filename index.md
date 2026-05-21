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
  
  /* Optional: make sure images fit */
  .profile-photo {
    max-width: 100%;
    height: auto;
  }
</style>

<div class="two-column">
  <div class="photo-column" markdown="1">
    <!-- {% include random-photo.html %} -->
    <p>Photo will go here</p>
  </div>
  
  <div class="menu-column" markdown="1">
    
    # Hi, I'm Cooper
    
    Welcome to my portfolio. I'm a [your role] passionate about [your interests].
    
    ---
    
    ## Featured Projects
    
    - [Project Name 1](/project1/)
    - [Project Name 2](/project2/)
    - [Project Name 3](/project3/)
    
    ---
    
    [View all projects →](/projects/)
  </div>
</div>
