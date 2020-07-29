<style lang="scss">
  @import "../style/themes.scss";

  a {
    color: $link-color;
    &:hover {
      color: rebeccapurple;
    }
  }

  .subheading {
    text-decoration: underline;
    margin: 1em 0 0;
  }
  .headline {
    margin:.6em 0 .7em;
  }
  .headline,
  .education-section {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
  }

  .job-title {
    font-weight: 300;
    margin: 1em 0 0;
  }
  .company-name {
    font-weight: 500;
    margin: 0.3em 0;
  }

</style>

<svelte:head>
  <title>Resume</title>
</svelte:head>

<h1>Resume</h1>

<div class="headline">
  <p class="byline">Full Stack – React/Vue and RoR flavors</p>
  <p class="resume-versions">
    <a target="_blank" href="SeanParker.pdf">PDF</a> |
    <a target="_blank" href="SeanParker.docx">DOC</a> versions
  </p>
</div>

<h2 class="subheading">Skills</h2>
<p>
  HTML5, CSS3/SASS, JavaScript, jQuery, Github, MySQL, VueJS, ReactJS, Ruby,
  Ruby on Rails, Docker, Webpack, Gulp, Vagrant, Composer, BootStrap, Chrome
  Inspector, Adobe Creative Suite
</p>

<h2 class="subheading">Work Experience</h2>

<div class="job-description">
  <h3 class="job-title">Full Stack Engineer</h3>
  <p class="company-name">Deloitte – May 2019 to Present</p>
  <ul>
    <li>
      Crafted a UI dashboard in VueJS to help analysts efficiently track supply
      chain anomalies
    </li>
    <li>
      Architected style and design patterns for a detailed supplier tracking app
      from the ground up
    </li>
    <li>
      Illustrated supplier data points from JSON with charts and graphs using D3
      and Canvas
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">Full Stack Developer</h3>
  <p class="company-name">Barquin Solutions – May 2018 to April 2019</p>
  <ul>
    <li>
      Troubleshooted feature and maintenance requests on older code base built
      in Rails and React
    </li>
    <li>
      Ensured maintainability of codebase using React Testing Library (Jest)
    </li>
    <li>
      Created detailed graphs of foreign aid data with D3 and SVGs to help
      inform policy decisions
    </li>
    <li>
      Improved 508 compliance and mobile responsiveness to provide a good
      experience for all users
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">Front End Developer</h3>
  <p class="company-name">
    Solutions By Design II, LLC – January 2018 to May 2018
  </p>
  <ul>
    <li>
      Created Medicare/Medicaid enrollment dashboard with ReactJS to match
      design specifications
    </li>
    <li>
      Integrated JavaScript (Jest) and ReactJS (Enzyme) testing for compliance
      with Jenkins pipeline
    </li>
    <li>
      Utilized Webpack, Sass, and Docker to simplify work flow in consistent
      team build environments
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">Senior Web Developer</h3>
  <p class="company-name">
    RIVA Solutions, Inc – October 2016 to January 2018
  </p>
  <ul>
    <li>
      Refined global resource library of Consular training tools via jQuery and
      DOM manipulation
    </li>
    <li>
      Simplified code bloat by over 50% with custom WordPress theme to modernize
      government site
    </li>
    <li>
      Picked and implemented new technologies to increase site stability for the
      future
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">Full Stack Rails Cohort (Bootcamp)</h3>
  <p class="company-name">
    DevPoint Labs – May 2016 to July 2016
  </p>
  <ul>
    <li>
      Developed web applications using Ruby on Rails and ReactJS on the frontend
    </li>
    <li>
      Built interactive components with JavaScript, jQuery, and state management
      with Redux
    </li>
    <li>
      Conducted automated testing of Rails applications with RSpec and Selenium
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">WordPress Developer/Integrator</h3>
  <p class="company-name">
    OBXtek – September 2015 to May 2016
  </p>
  <ul>
    <li>
      Implemented UX designer's recommendations into live WordPress multisite
      installation
    </li>
    <li>
      Built local sandbox with Vagrant, Composer, and GitHub to test changes
      before implementation
    </li>
    <li>
      Collaborated on an agile team, utilizing JIRA, Git branching, and version
      tagging
    </li>
  </ul>
</div>

<div class="job-description">
  <h3 class="job-title">Junior Web Developer</h3>
  <p class="company-name">
    Boostability – November 2012 to April 2015
  </p>
  <ul>
    <li>
      Developed over 30 responsive websites to design specifications in
      WordPress from scratch
    </li>
    <li>
      Built eCommerce sites and cleaned up CSV product sheets for mass import
    </li>
    <li>
      Identified priorities to finish maintenance requests and web builds within
      set deadlines
    </li>
  </ul>
</div>
<h2 class="subheading">Education</h2>
<section class="education-section">
  <div>
    <h3>
      Bachelor of Science in Communication, emphasis in Computer Information
      Science
    </h3>
    <p>Brigham Young University - Idaho – August 2008 to July 2012</p>
  </div>

  <div>
    <h3>Full Stack Rails Cohort</h3>
    <p>DevPoint Labs – May 2016 to July 2016</p>
  </div>
</section>
