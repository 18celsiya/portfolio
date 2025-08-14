<!-- Collapsible Ribbon -->
<style>
  /* Ribbon container */
  .ribbon {
    background-color: #FFFACD; /* Light yellow */
    padding: 10px 20px;
    display: flex;
    justify-content: flex-end; /* buttons on the right */
    align-items: center;
    font-family: sans-serif;
    border-radius: 0 0 10px 10px;
    margin-bottom: 20px;
  }

  /* Ribbon buttons */
  .ribbon button {
    background-color: #FFD700; /* Yellow */
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
    background-color: #FFF8DC; /* Lighter yellow */
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
</style>

<div class="ribbon">
  <!-- Data Viz button: links to dashboards folder -->
  <button onclick="window.location.href='dashboards/'">Data Viz</button>
  
  <!-- DS Blogs button: shows placeholder content -->
  <button onclick="toggleRibbon('dsblogs')">DS Blogs</button>
</div>

<!-- DS Blogs Content (placeholder) -->
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

<!-- Hide default page title -->
<style>
.header, .site-title, .title, h1 {
  display: none !important;
}
</style>

<div style="display: flex; align-items: flex-start; gap: 40px;">

  <!-- Profile Picture -->
  <img src="My_pic.jpg" alt="Profile Picture" width="180" style="border-radius: 10px;"/>

  <!-- Info Column -->
  <div>
    <h1 style="margin:0"><strong>CELSIYA ANTONYSAMY</strong></h1>
    <h3 style="margin:5px 0">Data Scientist</h3>

    <!-- Space between title and icons -->
    <div style="margin: 10px 0;">
      <!-- Email Icon -->
      <a href="mailto:joescelsiya@gmail.com">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/gmail.svg" alt="Email" width="28" height="28"/>
      </a>
      &nbsp;&nbsp;
      <!-- LinkedIn Icon -->
      <a href="https://www.linkedin.com/in/celsiya-antonysamy/" target="_blank">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn" width="28" height="28"/>
      </a>
      &nbsp;&nbsp;
      <!-- GitHub Icon -->
      <a href="https://github.com/18celsiya" target="_blank">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub" width="28" height="28"/>
      </a>
    </div>

    <!-- Bio Paragraph -->
    <p style="max-width:600px;">
      I am a Data Scientist working at Verian Group on the Population Studies Data Team. With a 1st Class MSc in Data Science and hands-on experience in AI, machine learning, and deep learning, I specialize in building tools and dashboards that not only analyze data but also make life easier for teams and stakeholders. From automating repetitive workflows to creating AI-driven applications, I thrive on making data accessible, actionable, and impactful for real-world projects.
    </p>

    <!-- What I Do Section -->
    <h3>🚀 What I Do</h3>
    <ul>
      <li>Automate workflows and reporting to save teams significant time</li>
      <li>Clean, analyze, and visualize complex datasets for actionable insights</li>
      <li>Build AI and machine learning tools, including NLP and deep learning models</li>
      <li>Design interactive dashboards and build Shiny interfaces for non-technical stakeholders</li>
    </ul>

  </div> <!-- closes Info Column -->
</div> <!-- closes Flex Container -->
