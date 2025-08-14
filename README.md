<style>
/* Hide the theme’s default page title */
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
      <a href="mailto:your.email@example.com">
        <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/gmail.svg" alt="Email" width="28" height="28"/>
      </a>
      &nbsp;&nbsp;
      <!-- LinkedIn Icon -->
      <a href="https://www.linkedin.com/in/your-linkedin-username/" target="_blank">
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

<h2 id="projects">📊 Data Viz Project</h2>

<!-- Project Thumbnail -->
<img src="Financial_Analysis.jpg" alt="Dashboard Thumbnail" 
     style="width:250px; cursor:pointer; border-radius:8px;" 
     onclick="openModal('Dashboard Project', 'path-to-dashboard-full.jpg')"/>

<!-- Modal Structure -->
<div id="modal" style="display:none; position:fixed; z-index:1000; left:0; top:0; width:100%; height:100%; background-color: rgba(0,0,0,0.7); justify-content:center; align-items:center;">
  <div style="background:white; padding:20px; border-radius:10px; max-width:600px; text-align:center; position:relative;">
    <span onclick="closeModal()" style="position:absolute; top:10px; right:15px; cursor:pointer; font-size:20px;">&times;</span>
    <h3 id="modalTitle"></h3>
    <img id="modalImage" src="" alt="Project Image" style="width:100%; border-radius:8px; margin-top:10px;"/>
  </div>
</div>

<script>
function openModal(title, imgSrc) {
  document.getElementById('modalTitle').innerText = title;
  document.getElementById('modalImage').src = imgSrc;
  document.getElementById('modal').style.display = 'flex';
}

function closeModal() {
  document.getElementById('modal').style.display = 'none';
}
</script>

