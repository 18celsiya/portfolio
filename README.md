<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Celsiya Antonysamy - Portfolio</title>

<style>
  /* Ribbon container */
  .ribbon {
    background-color: #FFF9C4; /* Light yellow */
    padding: 10px 20px;
    display: flex;
    justify-content: flex-end; /* buttons on the right */
    align-items: center;
    font-family: sans-serif;
    border-radius: 0 0 10px 10px;
    margin-bottom: 20px; /* space between ribbon and profile */
  }

  /* Ribbon buttons */
  .ribbon button {
    background-color: #FFD700; /* yellow */
    color: #000;
    border: none;
    padding: 5px 12px;
    margin-left: 10px;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
  }

  /* Collapsible content */
  .ribbon-content {
    display: none;
    background-color: #FFF8DC; /* Light yellow */
    padding: 10px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    margin-bottom: 20px;
  }

  .ribbon-content img {
    width: 90%;
    border-radius: 8px;
    margin-top: 10px;
  }

  /* Hide default page titles */
  .header, .site-title, .title, h1 {
    display: none !important;
  }

  /* Profile section */
  .profile-container {
    display: flex;
    align-items: flex-start;
    gap: 40px;
    font-family: sans-serif;
  }

  .profile-container img {
    border-radius: 10px;
    width: 180px;
  }

  .icon-links img {
    width: 28px;
    height: 28px;
    margin-left: 10px;
  }

  .bio, .what-i-do {
    max-width: 600px;
  }

  .what-i-do ul {
    margin-top: 5px;
  }

</style>
</head>
<body>

<!-- Collapsible Ribbon -->
<div class="ribbon">
  <button onclick="toggleRibbon('dataviz')">Data Viz</button>
  <button onclick="toggleRibbon('dsblogs')">DS Blogs</button>
</div>

<!-- Data Viz Content -->
<div id="dataviz" class="ribbon-content">
  <h3>Data Viz Projects</h3>
  <a href="/dashboards" target="_blank">
    <img src="dashboards/Financial_Analysis.png" alt="Financial Analysis Dashboard"/>
  </a>
</div>

<!-- DS Blogs Content -->
<div id="dsblogs" class="ribbon-content">
  <h3>Data Science Blogs</h3>
  <p>Coming soon...</p>
</div>

<script>
  function toggleRibbon(id) {
    const content = document.getElementById(id);
    content.style.display = (content.style.display === "block") ? "none" : "block";
  }
</script>

<!-- Profile Section -->
<div class="profile-container">

  <!-- Profile Picture -->
  <img src="My_pic.jpg" alt="Profile Picture"/>

  <!-- Info Column -->
  <div>
    <h1><strong>CELSIYA ANTONYSAMY</strong></h1>
    <h3>Data Scientist</h3>

    <!-- Space between title and icons -->
    <div class="icon-links">
      <a href="mailto:joescelsiya@gmail.com">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/gmail.svg" alt="Email"/>
      </a>
      <a href="https://www.linkedin.com/in/celsiya-antonysamy/" target="_blank">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn"/>
      </a>
      <a href="https://github.com/18celsiya" target="_blank">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub"/>
      </a>
    </div>

    <!-- Bio Paragraph -->
    <p class="bio">
      I am a Data Scientist working at Verian Group on the Population Studies Data Team. With a 1st Class MSc in Data Science and hands-on experience in AI, machine learning, and deep learning, I specialize in building tools and dashboards that not only analyze data but also make life easier for teams and stakeholders. From automating repetitive workflows to creating AI-driven applications, I thrive on making data accessible, actionable, and impactful for real-world projects.
    </p>

    <!-- What I Do Section -->
    <div class="what-i-do">
      <h3>🚀 What I Do</h3>
      <ul>
        <li>Automate workflows and reporting to save teams significant time</li>
        <li>Clean, analyze, and visualize complex datasets for actionable insights</li>
        <li>Build AI and machine learning tools, including NLP and deep learning models</li>
        <li>Design interactive dashboards and build Shiny interfaces for non-technical stakeholders</li>
      </ul>
    </div>

  </div> <!-- Info Column -->
</div> <!-- Profile Container -->
</body>
</html>
