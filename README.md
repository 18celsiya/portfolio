<!-- Ribbon -->
<div style="width:100%; background:#0078D7; color:white; padding:10px; display:flex; align-items:center; gap:20px; font-family:sans-serif;">
  <strong style="font-size:16px;">My Portfolio</strong>
  <button onclick="showDataViz()" 
          style="background:white; color:#0078D7; border:none; padding:5px 12px; border-radius:4px; cursor:pointer; font-weight:bold;">
    📊 Data Viz
  </button>
  <button onclick="showDSBlogs()" 
          style="background:white; color:#0078D7; border:none; padding:5px 12px; border-radius:4px; cursor:pointer; font-weight:bold;">
    ✍️ DS Blogs
  </button>
</div>

<!-- Modal for Data Viz -->
<div id="dataVizModal" style="display:none; position:fixed; z-index:1000; left:0; top:0; width:100%; height:100%; background-color: rgba(0,0,0,0.7); justify-content:center; align-items:center;">
  <div style="background:white; padding:20px; border-radius:10px; max-width:800px; text-align:center; position:relative;">
    <span onclick="closeDataViz()" style="position:absolute; top:10px; right:15px; cursor:pointer; font-size:24px;">&times;</span>
    <h3>Data Viz Projects</h3>
    <!-- Project Images -->
    <img src="Financial_Analysis.jpg" alt="Dashboard" style="width:90%; border-radius:8px; margin-top:10px;"/>
  </div>
</div>

<script>
function showDataViz() {
  document.getElementById('dataVizModal').style.display = 'flex';
}

function closeDataViz() {
  document.getElementById('dataVizModal').style.display = 'none';
}

// Placeholder function for DS Blogs (you can add modal for blogs similarly)
function showDSBlogs() {
  alert('DS Blogs modal coming soon!');
}
</script>



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

