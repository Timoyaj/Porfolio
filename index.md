---
layout: default
---

<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li>
      <a href="#about">About</a>
      <ul>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#certifications">Certifications</a></li>
      </ul>
    </li>
    <li><a href="#portfolio">Portfolio</a></li>
    <li>
      <a href="#experience">Experience</a>
      <ul>
        <li><a href="#education">Education</a></li>
      </ul>
    </li>
    <li><a href="#services">Services</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<section id="home">
  <div class="container">
    <img src="./Images/intro.jpg" alt="Profile Picture of Yaji Timothy Terungwa">
    <h1>Yaji Timothy Terungwa</h1>
    <h2>Data Scientist | Web Developer | Lecturer</h2>
    <a href="#contact" class="btn">Hire Me</a>
    <a href="#" class="btn">Download CV</a>
  </div>
</section>

<section id="about">
  <div class="container">
    <h2>About Me</h2>
    <p>Welcome to my portfolio. I am Yaji Timothy Terungwa, a passionate Data Scientist, Web Developer, and Lecturer. My mission is to empower businesses with advanced analytics, custom web applications, and comprehensive digital services to drive growth and success.</p>
    <p>With a strong background in statistics and computer science, I have extensive experience in data analysis, web development, and project management. I am committed to delivering high-quality solutions that meet the unique needs of each client.</p>
    
    <h3 id="skills">Skills</h3>
    <ul>
      <li>Data Analysis: R, Python, SPSS, Tableau, PowerBI</li>
      <li>GIS: QGIS, ArcGIS Pro</li>
      <li>Web Development: SQL, Django</li>
      <li>Data Visualization: StreamLit, Dash-plotly</li>
    </ul>
    
    <h3 id="certifications">Certifications</h3>
    <ul>
      <li><a href="http://example.com/cert1">Data Analyst Nano-Degree</a> - ALX-Udacity, November 2022</li>
      <li><a href="http://example.com/cert2">Planning for Monitoring and Evaluation</a> - Philanthropy University, November 2020</li>
      <li><a href="http://example.com/cert3">The Fundamentals of Digital Marketing</a> - Google Digital Garage, October 2020</li>
      <li><a href="http://example.com/cert4">Jobberman Certified Soft Skills</a> - Coursera, September 2021</li>
    </ul>
  </div>
</section>

<section id="portfolio">
  <div class="container">
    <h2>Portfolio</h2>
    <div class="carousel">
      <div class="carousel-inner">
        <div class="carousel-item">
          <img src="./Images/Power%20BI%20Project.jpg" alt="Customer Churn Analysis">
          <h3>Customer Churn Analysis by Demography</h3>
          <p>Analyzed customer churn data by various demographic factors using Power BI. Developed interactive visualizations to identify patterns and insights to help reduce churn.</p>
          <a href="http://example.com/project1" class="btn">View Project</a>
        </div>
        <div class="carousel-item">
          <img src="./Images/project2.jpg" alt="Project 2">
          <h3>Project 2 Title</h3>
          <p>Brief description of Project 2.</p>
          <a href="http://example.com/project2" class="btn">View Project</a>
        </div>
        <div class="carousel-item">
          <img src="./Images/project3.jpg" alt="Project 3">
          <h3>Project 3 Title</h3>
          <p>Brief description of Project 3.</p>
          <a href="http://example.com/project3" class="btn">View Project</a>
        </div>
      </div>
      <a href="#" class="carousel-control prev">&lt;</a>
      <a href="#" class="carousel-control next">&gt;</a>
    </div>
  </div>
</section>

<!-- The rest of the sections (Experience, Services, Contact) remain largely the same, 
     but you may want to add appropriate container divs and classes for consistent styling -->

<script>
  // JavaScript for carousel functionality
  const carousel = document.querySelector('.carousel-inner');
  const items = document.querySelectorAll('.carousel-item');
  const prevBtn = document.querySelector('.carousel-control.prev');
  const nextBtn = document.querySelector('.carousel-control.next');
  let currentIndex = 0;

  function showItem(index) {
    carousel.style.transform = `translateX(-${index * 100}%)`;
  }

  prevBtn.addEventListener('click', (e) => {
    e.preventDefault();
    currentIndex = (currentIndex - 1 + items.length) % items.length;
    showItem(currentIndex);
  });

  nextBtn.addEventListener('click', (e) => {
    e.preventDefault();
    currentIndex = (currentIndex + 1) % items.length;
    showItem(currentIndex);
  });
</script>
