<template>
  <div>
    <head>
      <title>Acacia's Portfolio</title>
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <link href="../assets/style.css" rel="stylesheet" type="text/css">
      <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    </head>
    <body>
        <div id="home" class="homesection">
          <nav>
            <div class="leftnav">
              <a href="https://www.linkedin.com/in/acacia-kahananui-baker" target="_blank"><img src="../assets/acacia.png" alt="Acacia" height="80%" width="80%"></a>
            </div>
            <ul class="rightnav">
              <li class="navelement"><a href="#home">Home</a></li>
              <li class="navelement"><a href="#about">About</a></li>
              <li class="navelement"><a href="#projects">Projects</a></li>
              <li class="navelement"><a href="#contact">Contact</a></li>
            </ul>
          </nav>
          <div class="home">
            <div class="intro">
            <div id="profession">Full-Stack Developer</div>
            <div class="line1intro">
              <h2 class="hello">Hello, I'm </h2>
              <h1 id="acacia">Acacia</h1>
            </div>
            <div class="nextlines">
              <h2 id="baker">Kahananui-Baker</h2>
              <br> 
              <h2 class="line3intro">
                based in San Diego, California.
              </h2>
            </div>
            </div>
            <div id="graphics">
              <img src="../assets/background.png" alt="background image" height="90%" width="100%">
            </div>
          </div>
          
        </div>
        <div id="about" class="about">
          <div class="about-img">
            <img class="profile-img" src="../assets/acacia-pic.jpeg" alt="Cat">
          </div>
          <div class="about-info">
            <div>
              <h1 class="about-title">About Me</h1>
            </div>
            <div>
              <p class="about-description">
                Hi! My name is Acacia and I am a dedicated and hard working Software Developer seeking an entry-level position! I am fueled by my passion for my work, ability to adapt to my environment, desire to learn from my peers &#40;and Google of course&#41;, which makes me the ideal candidate for your position. This website is the first quality website I've built from beginning to end by myself and I wanted to try out some new things! Thank you for visiting and I hope to be in contact soon!  
              </p>
            </div>
            <div class="about-section-list">
              <p id="default-about" class="about-section-item" @click="openTab('experience')">Experience</p>
              <p class="about-section-item" @click="openTab('skills')">Skills</p>
              <p class="about-section-item" @click="openTab('education')">Education</p>
            </div>
            <div class="skills">
              <div id="experience" class="about-section-item-content"> 
                <h3 class="most-recent experience-header">Full Stack Developer</h3>
                <h4 class="experience-duration">February 2022 - March 2023</h4>
                <h3 class="experience-header">Information Technology Intern</h3>
                <h4 class="experience-duration">August 2021 - November 2021</h4>
                <h3 class="experience-header">Computer Science Tutor</h3>
                <h4 class="experience-duration">September 2020 - March 2021</h4>
              </div>
              <div id="skills" class="about-section-item-content">
                <h3 class="skills-header">Language Proficiency</h3>
                <ul class="skills-list">
                  <li class="individual-skills">Javascript</li>
                  <li class="individual-skills">HTML</li>
                  <li class="individual-skills">PHP</li>
                  <li class="individual-skills">Linux</li>
                  <li class="individual-skills">CSS</li>
                  <li class="individual-skills">Java</li>
                </ul>
              </div>
              <div id="education" class="about-section-item-content"> 
                <h3 class="education-header uvu">Utah Valley University</h3>
                <h4 class="major">Master's of Science in Cybersecurity</h4>
                <h3 class="education-header">Brigham Young University - Hawaii</h3>
                <h4 class="major">Bachelor's of Science in Computer Science</h4>
              </div>
            </div>  
          </div>
        </div>
        <div id="projects" class="project-section">
          <h3 class="personal-projects-header">Personal Projects</h3>
          <div class="project-div">
            <div class="project">
              <img class="project-img" src="../assets/coming-soon.png" alt="Image Coming Soon" height="90%" width="100%">
              <div class="project-description">
                <h3 class="project-title">Project 1</h3>
                <p class="fade-in">Coming Soon!</p>
              </div>
            </div>
            <div class="project">
              <img class="project-img" src="../assets/coming-soon.png" alt="Image Coming Soon" height="90%" width="100%">
              <div class="project-description">
                <h3 class="project-title">Project 2</h3>
                <p class="fade-in">Coming Soon!</p>
              </div>
            </div>
            <div class="project">
              <img class="project-img" src="../assets/coming-soon.png" alt="Image Coming Soon" height="90%" width="100%">
              <div class="project-description">
                <h3 class="project-title">Project 3</h3>
                <p class="fade-in">Coming Soon!</p>
              </div>
            </div>
          </div>
        </div>
      <footer id="contact">
        <div class="contact-me-section">
          <div class="footer-element-1">
            <h1 class="contact">Contact Me</h1>
            <h4 id="mail" class="contact-info">
              <span class="material-icons">mail</span>
              acacia.riana@gmail.com
            </h4>
            <h4 id="phoneNumber" class="contact-info">
              <span class="material-icons">dialpad</span>
              (619) 647-1002
            </h4>
            <a href="https://github.com/acaciariana/acacia-kahananui-baker.github.io.git" target="_blank"><img src="../assets/github-icon.png" alt="GitHub Icon" height="20%" width="13%"></a>
            <a href="https://www.linkedin.com/in/acacia-kahananui-baker" target="_blank"><img src="../assets/linkedin-icon.png" alt="LinkedIn Icon" height="20%" width="13%"></a>
          </div>
          <div class="footer-element-2">
            <form @submit.prevent="sendMail()">
              <input type="text" id="name" class="contact-me-field" placeholder="Name" name="name" required>
              <input type="text" id="email" class="contact-me-field" placeholder="Email" name="email" required>
              <input type="text" id="phone" class="contact-me-field" placeholder="Phone Number" name="phone">
              <textarea id="message" placeholder="Message" name="message" class="contact-me-field"></textarea>
              <input type="submit" id="submit" value="Send" placeholder="Enter text here">
            </form>
          </div>
        </div>
      </footer>
    </body>
  </div>
  </template>
  <script>
 import emailjs from '@emailjs/browser';
  
  export default {
    name: 'PortfolioMain',
    metaInfo: {
      script: [
        { src: "https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"}
      ]
    },
    data() {
      return {
        serviceId: "service_07daglk",
        templateId: "template_emnbr25"
      }
    },
    methods: {
      openTab(tab) {
        var i, tabcontent;
        tabcontent = document.getElementsByClassName("about-section-item-content");
        for(i = 0; i < tabcontent.length; i++){
          tabcontent[i].style.display = "none";
        }
        document.getElementById(tab).style.display = "block";
      },
      sendMail() {
        
        emailjs.init("syQxHKH-ihAPtbNZM");
        console.log("We got past init");
        var params = {
            name: document.getElementById("name").value,
            email: document.getElementById("email").value,
            phone: document.getElementById("phone").value,
            message: document.getElementById("message").value,
        }
        console.log(params);
        
        emailjs.send(this.serviceId, this.templateId, params)
          .then((res) => {
              document.getElementById("name").value = "";
              document.getElementById("email").value = "";
              document.getElementById("phone").value = "";
              document.getElementById("message").value = "";
              console.log(res);
              alert("Your message was sent");
              console.log("SOMETHING HAPPENED THE WAY WE WANTED IT TO");
          })
          .catch((err) => console.log(err));

      }
    }
  }
  </script>
  