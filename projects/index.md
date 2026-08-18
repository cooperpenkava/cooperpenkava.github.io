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
    <a href="/projects/pump">Pump up the Jam!!! →</a>
    <img src="assets/pump-header.jpg" alt="Pump up the Jam!!!" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/teapot">The Case of the Leaky Teapot →</a>
    <img src="assets/teapot-header.jpg" alt="The Case of the Leaky Teapot" class="hover-image">
  </div>

  <div class="project-item">
    <a href="/projects/ode45">I (re)made ode45! →</a>
    <img src="assets/ode45-header.png" alt="I (re)made ode45!" class="hover-image">
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
  margin-bottom: 1.5rem;
  position: relative;
  display: flex;
  align-items: center;  /* this centers the image vertically */
  min-height: 80px;     /* ensures consistent spacing */
}

.hover-image {
  display: none;
  position: absolute;
  left: 100%;           /* appears to the right of the link */
  margin-left: 2rem;
  max-width: 500px;     /* bigger! */
  width: 100%;
  height: auto;
  border-radius: 8px;
  z-index: 100;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15); /* subtle shadow for depth */
  top: 50%;             /* center vertically */
  transform: translateY(-50%); /* perfect vertical centering */
}

.project-item:hover .hover-image {
  display: block;
}

/* For mobile responsiveness */
@media (max-width: 768px) {
  .project-item {
    display: block;     /* reset flex on mobile */
    min-height: auto;
  }
  
  .hover-image {
    position: static;
    margin-top: 0.5rem;
    margin-left: 0;
    max-width: 100%;
    transform: none;    /* reset transform */
    top: auto;
  }
}
  
</style>

<p><a href="/">← Back to Home</a></p>
