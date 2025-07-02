<script setup lang="ts">
// import { ref } from 'vue'

const currentYear = new Date().getFullYear()
const age = currentYear - 1997 // Assuming birth year is 1997 based on your CV
import heroBg from '@/assets/img/img-bg-1.jpg'
// const resultMessage = ref('')

// Import the image so Vite/Webpack handles it correctly in production
</script>

<template>
  <!-- Navigation -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">Benjamin Otchere Boakye</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#projects">Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
    <header
      class="bg-primary text-white py-10"
      :style="{
        backgroundImage: `url('${heroBg}')`,
        backgroundSize: 'cover',
        backgroundPosition: 'center',
        borderRadius: '1rem',
      }"
    >
      <div
        class="container py-5 card"
        style="background: rgba(255, 255, 255, 0.75); backdrop-filter: blur(8px); border: none"
      >
        <div class="row align-items-center">
          <div class="col-lg-6">
            <div class="ms-4">
              <h1 class="display-4 fw-bold mb-4 text-dark">Benjamin Otchere Boakye</h1>
              <h2 class="h4 mb-4 text-dark">Full Stack Software Engineer</h2>
              <p class="lead mb-4 text-dark">
                5+ years of experience designing, developing, and scaling enterprise-level web
                applications.
              </p>
              <div class="d-flex gap-3">
                <a href="#contact" class="btn btn-light btn-md px-4">Contact Me</a>
                <a href="#" class="btn btn-outline-secondary btn-md px-4">Download CV</a>
              </div>
            </div>
          </div>
          <div class="col-lg-6 mt-5 mt-lg-0">
            <div class="d-flex justify-content-center align-items-center" style="height: 300px">
              <img
                src="/src/assets/img/avatar.png"
                alt="Benjamin Otchere Boakye"
                class="img-fluid rounded-circle"
              />
            </div>
          </div>
        </div>
      </div>
    </header>
  </nav>

  <!-- About Section -->
  <section id="about" class="py-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <h2 class="fw-bold mb-4">About Me</h2>
          <p class="lead">
            Passionate about building secure, scalable, and high-performance solutions using modern
            web technologies, cloud computing, and microservices architecture.
          </p>
          <p>
            Experienced in mentoring teams, leading projects, and implementing Agile methodologies
            to deliver efficient solutions that align with business needs and user satisfaction.
          </p>

          <div class="row mt-4">
            <div class="col-md-6">
              <ul class="list-unstyled">
                <li class="mb-2"><strong>Age:</strong> {{ age }}</li>
                <li class="mb-2"><strong>Location:</strong> London, UK</li>
                <li class="mb-2"><strong>Email:</strong> nanaboakyeyiadom18@gmail.com</li>
              </ul>
            </div>
            <div class="col-md-6">
              <ul class="list-unstyled">
                <li class="mb-2"><strong>Phone:</strong> +44 7796 005063</li>
                <li class="mb-2"><strong>Freelance:</strong> Available</li>
                <li class="mb-2">
                  <strong>Social:</strong>
                  <span class="ms-1">
                    <a
                      href="https://github.com/NABY-Inc"
                      target="_blank"
                      class="me-2 text-dark"
                      title="GitHub"
                    >
                      <i class="bi bi-github"></i>
                    </a>
                    <a
                      href="https://www.linkedin.com/in/benjamin-otchere-boakye-204b96160"
                      target="_blank"
                      class="me-2 text-primary"
                      title="LinkedIn"
                    >
                      <i class="bi bi-linkedin"></i>
                    </a>
                    <a
                      href="https://wakatime.com/@naby"
                      target="_blank"
                      class="text-info"
                      title="Wakatime"
                    >
                      <i class="bi bi-bar-chart"></i>
                    </a>
                  </span>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="card shadow-sm">
            <div class="card-body">
              <h3 class="h5 mb-4">Technical Expertise</h3>
              <div class="mb-3">
                <h4 class="h6">Programming Languages</h4>
                <div class="d-flex flex-wrap gap-2 mt-2">
                  <span class="badge bg-primary">PHP</span>
                  <span class="badge bg-primary">JavaScript</span>
                  <span class="badge bg-primary">Python</span>
                  <span class="badge bg-primary">SQL</span>
                  <span class="badge bg-primary">C#</span>
                  <span class="badge bg-primary">.NET</span>
                </div>
              </div>

              <div class="mb-3">
                <h4 class="h6">Frameworks & Libraries</h4>
                <div class="d-flex flex-wrap gap-2 mt-2">
                  <span class="badge bg-success">Laravel</span>
                  <span class="badge bg-success">Vue.js</span>
                  <span class="badge bg-success">React.js</span>
                  <span class="badge bg-success">Django</span>
                  <span class="badge bg-success">Bootstrap</span>
                  <span class="badge bg-success">Tailwind</span>
                </div>
              </div>

              <div class="mb-3">
                <h4 class="h6">Cloud & DevOps</h4>
                <div class="d-flex flex-wrap gap-2 mt-2">
                  <span class="badge bg-info">AWS</span>
                  <span class="badge bg-info">Azure</span>
                  <span class="badge bg-info">Docker</span>
                  <span class="badge bg-info">Linux</span>
                  <span class="badge bg-info">Git</span>
                </div>
              </div>

              <div class="mb-3">
                <h4 class="h6">Databases</h4>
                <div class="d-flex flex-wrap gap-2 mt-2">
                  <span class="badge bg-warning text-dark">MySQL</span>
                  <span class="badge bg-warning text-dark">MongoDB</span>
                  <span class="badge bg-warning text-dark">PostgreSQL</span>
                  <span class="badge bg-warning text-dark">GraphQL</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="py-5 bg-light">
    <div class="container">
      <h2 class="fw-bold text-center mb-5">Technical Skills</h2>

      <div class="row">
        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5 mb-4">Frontend Development</h3>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>React.js</span>
                  <span>90%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-primary" role="progressbar" style="width: 90%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>Vue.js</span>
                  <span>85%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-primary" role="progressbar" style="width: 85%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>JavaScript/TypeScript</span>
                  <span>95%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-primary" role="progressbar" style="width: 95%"></div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5 mb-4">Backend Development</h3>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>PHP/Laravel</span>
                  <span>95%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-success" role="progressbar" style="width: 95%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>Python/Django</span>
                  <span>85%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-success" role="progressbar" style="width: 85%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>C#/.NET</span>
                  <span>80%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-success" role="progressbar" style="width: 80%"></div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5 mb-4">DevOps & Cloud</h3>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>AWS Services</span>
                  <span>85%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-info" role="progressbar" style="width: 85%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>Docker</span>
                  <span>80%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-info" role="progressbar" style="width: 80%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>CI/CD Pipelines</span>
                  <span>75%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-info" role="progressbar" style="width: 75%"></div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5 mb-4">Database & Architecture</h3>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>SQL Databases</span>
                  <span>90%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-warning" role="progressbar" style="width: 90%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>NoSQL Databases</span>
                  <span>80%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-warning" role="progressbar" style="width: 80%"></div>
                </div>
              </div>
              <div class="skill-item mb-3">
                <div class="d-flex justify-content-between mb-1">
                  <span>Microservices Architecture</span>
                  <span>85%</span>
                </div>
                <div class="progress" style="height: 8px">
                  <div class="progress-bar bg-warning" role="progressbar" style="width: 85%"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Experience Section -->
  <section id="experience" class="py-5">
    <div class="container">
      <h2 class="fw-bold text-center mb-5">Work Experience</h2>

      <div class="timeline">
        <!-- Benogis Innovations -->
        <div class="timeline-item">
          <div class="timeline-date">June 2022 – Present</div>
          <div class="timeline-content card shadow-sm">
            <div class="card-body">
              <h3 class="h5">Benogis Innovations, Co-Founder & Lead Software Engineer</h3>
              <p class="text-muted">London</p>
              <ul>
                <li>
                  Spearheaded the development of EduLink Network, a multi-service platform using
                  Laravel, Vue.js, MySQL, and GraphQL.
                </li>
                <li>
                  Designed and deployed scalable microservices architectures with Docker and AWS
                  (RDS, EC2, ECS, S3, Lambda).
                </li>
                <li>
                  Led code reviews, mentored junior developers, and established Agile best
                  practices.
                </li>
                <li>
                  Implemented advanced security measures (user authentication, data encryption) to
                  align with industry standards.
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Route to Transition -->
        <div class="timeline-item">
          <div class="timeline-date">May 2024 – Present</div>
          <div class="timeline-content card shadow-sm">
            <div class="card-body">
              <h3 class="h5">
                Route to Transition, IT Systems Administrator
                <span class="text-muted">(Part-time)</span>
              </h3>
              <p class="text-muted">London</p>
              <ul>
                <li>
                  Managed critical IT infrastructure, ensuring system reliability and security in
                  compliance with OFSTED regulations.
                </li>
                <li>
                  Provided technical training for staff, enhancing productivity with new IT systems
                  and automation.
                </li>
                <li>
                  Optimized workflow processes with innovative solutions, contributing to
                  organizational efficiency.
                </li>
                <li>
                  Optimized internal processes using Microsoft Intune and cloud-based solutions.
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Africa Systems Ltd -->
        <div class="timeline-item">
          <div class="timeline-date">Mar 2024 – May 2024</div>
          <div class="timeline-content card shadow-sm">
            <div class="card-body">
              <h3 class="h5">Africa Systems Ltd, Software Engineer (Laravel Framework)</h3>
              <p class="text-muted">South Africa, Remote</p>
              <ul>
                <li>
                  Developed and Optimized the SWITCH Network using Laravel's .NET Core One
                  framework.
                </li>
                <li>
                  Enhanced fintech capabilities by implementing distributed ledger technology and
                  database optimizations.
                </li>
                <li>
                  Worked closely with UI/UX designers and development teams to ensure seamless
                  integration of features.
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Banko City University -->
        <div class="timeline-item">
          <div class="timeline-date">Jan 2023 – Jun 2023</div>
          <div class="timeline-content card shadow-sm">
            <div class="card-body">
              <h3 class="h5">Banko City University, Software Developer</h3>
              <p class="text-muted">Ghana</p>
              <ul>
                <li>
                  Led the design and development of software programs that optimized university
                  processes.
                </li>
                <li>
                  Developed an automated data entry system for receipt processing, reducing manual
                  workload and decreasing data entry errors by 30%.
                </li>
                <li>Implemented strategic automation, saving an estimated 20+ hours weekly.</li>
                <li>
                  Designed and deployed scalable database architectures in MySQL, optimizing query
                  performance.
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Smart-Tech Solutions -->
        <div class="timeline-item">
          <div class="timeline-date">Sep 2022 – Dec 2022</div>
          <div class="timeline-content card shadow-sm">
            <div class="card-body">
              <h3 class="h5">Smart-Tech Solutions, Software Developer</h3>
              <p class="text-muted">Ghana</p>
              <ul>
                <li>
                  Developed a web application using PHP (Laravel) and React.js, enhancing user
                  experience and improving system performance by over 40%.
                </li>
                <li>
                  Applied Agile methodologies to streamline project delivery and maintained detailed
                  documentation.
                </li>
                <li>Conducted software testing and documentation for long-term maintainability.</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="py-5 bg-light">
    <div class="container">
      <h2 class="fw-bold text-center mb-5">Key Projects</h2>

      <div class="row g-4">
        <!-- EduLink Network -->
        <div class="col-md-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5">EduLink Network</h3>
              <p class="text-muted">All-in-one educational platform for schools in Ghana</p>
              <p>
                Built with Laravel, Vue, GraphQL, and AWS. Provides comprehensive school management
                solutions including student records management, academic performance tracking,
                financial tracking, attendance tracking, and communication tools.
              </p>
              <div class="d-flex flex-wrap gap-2 mt-3">
                <span class="badge bg-primary">Laravel</span>
                <span class="badge bg-primary">React.js</span>
                <span class="badge bg-primary">GraphQL</span>
                <span class="badge bg-primary">AWS</span>
              </div>
            </div>
          </div>
        </div>

        <!-- Strenuous Effort Mini Banking System -->
        <div class="col-md-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5">Strenuous Effort Mini Banking System</h3>
              <p class="text-muted">
                Micro-banking solution with robust financial security features
              </p>
              <p>
                Engineered a secure banking platform with transaction processing, account
                management, and financial reporting capabilities.
              </p>
              <div class="d-flex flex-wrap gap-2 mt-3">
                <span class="badge bg-success">PHP</span>
                <span class="badge bg-success">MySQL</span>
                <span class="badge bg-success">JavaScript</span>
                <span class="badge bg-success">Security</span>
              </div>
            </div>
          </div>
        </div>

        <!-- Project Collaboration System -->
        <div class="col-md-4">
          <div class="card h-100 shadow-sm">
            <div class="card-body">
              <h3 class="h5">Project Collaboration System</h3>
              <p class="text-muted">Real-time collaboration platform</p>
              <p>
                Developed a project management tool to enhance team collaboration with task
                tracking, document sharing, and real-time communication features.
              </p>
              <div class="d-flex flex-wrap gap-2 mt-3">
                <span class="badge bg-info">Vue.js</span>
                <span class="badge bg-info">Node.js</span>
                <span class="badge bg-info">WebSockets</span>
                <span class="badge bg-info">MongoDB</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Education & Certifications -->
  <section id="education" class="py-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 mb-5 mb-lg-0">
          <h2 class="fw-bold mb-4">Education</h2>
          <div class="card shadow-sm">
            <div class="card-body">
              <h3 class="h5">University of Education, Winneba</h3>
              <p class="text-muted">BSc in Information Technology</p>
              <p>July 2021</p>
              <p>
                Specialized in Information Technology with a strong focus on software engineering,
                database systems, networking, and IT project management. Developed practical skills
                in programming, systems analysis, and deploying technology solutions to solve
                real-world business challenges.
              </p>
            </div>
          </div>
        </div>

        <div class="col-lg-6">
          <h2 class="fw-bold mb-4">Certifications</h2>
          <div class="card shadow-sm">
            <div class="card-body">
              <ul class="list-group list-group-flush">
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Backend & Frontend Development
                  <span class="badge bg-primary rounded-pill">Dec 2024</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Active Directory Basics
                  <span class="badge bg-primary rounded-pill">Oct 2024</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Introduction to AWS
                  <span class="badge bg-primary rounded-pill">Oct 2024</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Understanding Cloud Computing
                  <span class="badge bg-primary rounded-pill">Sept 2024</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Cybersecurity
                  <span class="badge bg-primary rounded-pill">Aug 2019</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-center">
                  Internet of Things
                  <span class="badge bg-primary rounded-pill">June 2019</span>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-5 bg-dark text-white">
    <div class="container">
      <h2 class="fw-bold text-center mb-5">Get In Touch</h2>

      <div class="row">
        <div class="col-lg-6 mb-5 mb-lg-0">
          <div class="card bg-secondary text-white shadow-sm">
            <div class="card-body">
              <h3 class="h4 mb-4">Contact Information</h3>
              <ul class="list-unstyled">
                <li class="mb-3">
                  <i class="bi bi-envelope me-3"></i>
                  <a href="mailto:nanaboakyeyiadom18@gmail.com" class="text-white"
                    >nanaboakyeyiadom18@gmail.com</a
                  >
                </li>
                <li class="mb-3">
                  <i class="bi bi-phone me-3"></i>
                  <a href="tel:+447796005063" class="text-white">+44 7796 005063</a>
                </li>
                <li class="mb-3">
                  <i class="bi bi-linkedin me-3"></i>
                  <a
                    href="https://www.linkedin.com/in/benjamin-otchere-boakye-204b96160"
                    target="_blank"
                    class="text-white"
                    >LinkedIn Profile</a
                  >
                </li>
                <li class="mb-3">
                  <i class="bi bi-geo-alt me-3"></i>
                  London, United Kingdom
                </li>
              </ul>

              <div class="mt-5">
                <h4 class="h5 mb-3">Connect With Me</h4>
                <div class="d-flex gap-3">
                  <a href="#" class="text-white"><i class="bi bi-github fs-4"></i></a>
                  <a href="#" class="text-white"><i class="bi bi-linkedin fs-4"></i></a>
                  <a href="#" class="text-white"><i class="bi bi-twitter fs-4"></i></a>
                  <a href="#" class="text-white"><i class="bi bi-facebook fs-4"></i></a>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-lg-6">
          <div class="card bg-secondary text-white shadow-sm">
            <div class="card-body">
              <h3 class="h4 mb-4">Send Me a Message</h3>
              <form>
                <div class="mb-3">
                  <label for="name" class="form-label">Name</label>
                  <input type="text" class="form-control bg-dark text-white" id="name" required />
                </div>
                <div class="mb-3">
                  <label for="email" class="form-label">Email</label>
                  <input type="email" class="form-control bg-dark text-white" id="email" required />
                </div>
                <div class="mb-3">
                  <label for="subject" class="form-label">Subject</label>
                  <input
                    type="text"
                    class="form-control bg-dark text-white"
                    id="subject"
                    required
                  />
                </div>
                <div class="mb-3">
                  <label for="message" class="form-label">Message</label>
                  <textarea
                    class="form-control bg-dark text-white"
                    id="message"
                    rows="4"
                    required
                  ></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Send Message</button>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="py-4 bg-black text-white">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-6 text-center text-md-start">
          <p class="mb-0">&copy; {{ currentYear }} Benjamin Otchere Boakye. All rights reserved.</p>
        </div>
        <div class="col-md-6 text-center text-md-end">
          <div class="d-flex justify-content-center justify-content-md-end gap-3">
            <a href="#" class="text-white"><i class="bi bi-github"></i></a>
            <a href="#" class="text-white"><i class="bi bi-linkedin"></i></a>
            <a href="#" class="text-white"><i class="bi bi-twitter"></i></a>
            <a href="#" class="text-white"><i class="bi bi-facebook"></i></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
/* Custom Timeline Styles */
.timeline {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 50px;
}

.timeline::after {
  content: '';
  position: absolute;
  width: 2px;
  background-color: #0d6efd;
  top: 0;
  bottom: 0;
  left: 25px;
  margin-left: -3px;
}

.timeline-item {
  padding: 10px 0;
  position: relative;
}

.timeline-content {
  padding: 20px;
  position: relative;
  border-radius: 6px;
}

.timeline-date {
  text-align: right;
  font-weight: bold;
  color: #0d6efd;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .timeline {
    padding-left: 25px;
  }

  .timeline::after {
    left: 15px;
  }

  .timeline-item::after {
    left: 5px;
  }

  .timeline-date {
    position: relative;
    left: 0;
    text-align: left;
    width: auto;
    margin-bottom: 10px;
  }
}

/* Smooth scrolling */
html {
  scroll-behavior: smooth;
}

/* Navbar active link highlight */
.navbar-nav .nav-link.active {
  color: #0d6efd;
  font-weight: bold;
}

/* Section padding */
section {
  padding-top: 80px;
  padding-bottom: 80px;
}

/* Hero section */
header {
  padding-top: 100px;
  padding-bottom: 100px;
}

/* Card hover effect */
.card {
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}
</style>
