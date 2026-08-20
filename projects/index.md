---
layout: page
title: projects
permalink: /projects/
---

<div class="project-list">
  <div class="project-item">
    <a href="/projects/stirling-engine">Stirling Engine →</a>
    <img src="assets/stirling-engine-header.jpg" alt="Stirling Engine" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/COUCH">Control Oriented Universal Chassis Hub (COUCH) Lab →</a>
    <img src="assets/COUCH-header.jpg" alt="COUCH Lab" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/motor-tester">Robotic Arm Motor Test Rig →</a>
    <img src="assets/motor-tester-header.jpg" alt="Robotic Arm Motor Test Rig" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/sprocket">FSAE Car Sprocket Lightweighting →</a>
    <img src="assets/sprocket-header.jpg" alt="FSAE Car Sprocket Lightweighting" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/ode45">I (re)made ode45! →</a>
    <img src="assets/ode45-header.png" alt="I (re)made ode45!" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/pump">Pump up the Jam!!! →</a>
    <img src="assets/pump-header.jpg" alt="Pump up the Jam!!!" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/teapot">The Case of the Leaky Teapot →</a>
    <img src="assets/teapot-header.jpg" alt="The Case of the Leaky Teapot" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/swish">A swish, every time. →</a>
    <img src="assets/swish-header.JPG" alt="A swish, every time." class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/scanner">3D Scanner in 2 Weeks →</a>
    <img src="assets/scanner-header.jpg" alt="3D Scanner in 2 Weeks" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/grabber">Kinematic Arm Autonomous Weeding Robot →</a>
    <img src="assets/grabber-header.jpg" alt="Kinematic Arm Autonomous Weeding Robot" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/solar">Modular Solar System →</a>
    <img src="assets/solar-header.png" alt="Modular Solar System" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/clock">3D Printed Pendulum Clock →</a>
    <img src="assets/clock-header.jpg" alt="3D Printed Pendulum Clock" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/rollerskates">Make Your Own Rollerskates →</a>
    <img src="assets/rollerskate-header.jpg" alt="Make Your Own Rollerskates" class="hover-image">
  </div>
</div>

<style>
.project-item {
  margin-bottom: 0.5rem;
  position: relative;
  display: flex;
  align-items: center;
  min-height: 40px;
}

.hover-image {
  display: none;
  position: absolute;
  left: 100%;
  margin-left: 1rem;
  max-width: 350px;
  width: auto;
  max-height: 250px;
  height: auto;
  border-radius: 8px;
  z-index: 1000;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  top: 50%;
  transform: translateY(-50%);
}

.project-item:hover .hover-image {
  display: block;
}

/* If the image would go off the right edge, flip it to the left */
@media (max-width: 1400px) {
  .hover-image {
    left: auto;
    right: 100%;
    margin-right: 1rem;
    margin-left: 0;
    transform: translateY(-50%);
  }
}

/* For mobile - back to below the text */
@media (max-width: 768px) {
  .project-item {
    display: block;
    min-height: auto;
    margin-bottom: 1rem;
  }
  
  .hover-image {
    position: static;
    margin-top: 0.5rem;
    margin-right: 0;
    max-width: 100%;
    width: 100%;
    transform: none;
    box-shadow: none;
  }
}
  
</style>

<p><a href="/">← Back to Home</a></p>
