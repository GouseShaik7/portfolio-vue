<template>
  <nav>
    <NuxtLink to="/">About</NuxtLink>
    <NuxtLink to="/skills">Skills</NuxtLink>
    <NuxtLink to="/projects">Projects</NuxtLink>
    <NuxtLink to="/contact">Contact</NuxtLink>
  </nav>
</template>

<style scoped>

nav {
  display: flex;
  justify-content: space-around;
  padding: 1rem;
  background-color: #333;
}
nav a {
  color: white;
  text-decoration: none;
  padding: 0.5rem;
}
nav a:hover {
  text-decoration: underline;
}
</style>

<template>
  <div class="about">
    <h1>About Me</h1>
    <p>
     Hello, I'm <b>Mohammed Gouse Shaik</b>, a passionate learner with a strong background in <b>Software and Civil Engineering</b>. I am dedicated to creating meaningful and innovative projects that leave a positive impact on the world. With a strong foundation in <b>Software and Civil Engineering</b>, I am constantly exploring new opportunities to expand my knowledge and skill set.
               I'm an Entrepreneur by my passion
               I'm always eager to connect with fellow professionals, potential collaborators. Feel free to reach out to me, and let's embark on new and exciting ventures together.
               Thank you for visiting my portfolio website, and I look forward to the opportunity to work with you.
    </p>
  </div>
</template>

<style scoped>
.about {
  text-align: center;
  padding: 2rem;
  background-color: blue;
}
</style>

<template>
  <div class="skills">
    <h1>Skills</h1>
    <ul>
      <li>HTML, CSS, JavaScript</li>
      <li>JAVA</li>
      <li>SQL</li>
      <li>Git, GitHub</li>
    </ul>
  </div>
</template>

<style scoped>
.skills {
  text-align: center;
  padding: 2rem;
}
.skills ul {
  list-style-type: none;
}
</style>

<template>
  <div class="projects">
    <h1>Projects</h1>
    <div class="project">
            <h2>RESUME BUILDER</h2>
            <p>The Full-Stack Resume Builder is a comprehensive web application designed to help individuals create and manage their professional resumes with ease. In today's competitive job market, having a well-crafted resume is essential for career success. This project aims to provide users, especially job seekers and professionals, with a user-friendly platform to build, customize, and download professional resumes effortlessly.</p>
            <a href="https://github.com/GouseShaik7/Resumebuilder" target="_blank">Source Code</a>
          </div>
          <div class="project">
            <h2>UNIT CONVERTER</h2>
            <p>The Java Unit Converter is a versatile console-based application designed to simplify unit conversions across various categories, including length, area, volume, weight, and temperature. It offers a convenient and efficient way for users to convert measurements from one unit to another within these categories. Whether it's converting kilometers to miles, square meters to square feet, liters to gallons, kilograms to pounds, or Celsius to Fahrenheit, this project provides a user-friendly and comprehensive solution for handling everyday unit conversions.</p>
            <a href="https://github.com/GouseShaik7/Unit-converter" target="_blank">Source Code</a>
          </div>
          <div class="project">
            <h2>REAL-TIME OBJECT DETECTION</h2>
            <p>The Real-Time Object Detection project is a cutting-edge computer vision application developed in Python. It leverages state-of-the-art deep learning techniques to detect and track objects in real-time video streams from various sources, such as webcams, video files, or live camera feeds. This project offers a powerful and versatile tool for a wide range of applications, including security surveillance, autonomous vehicles, robotics, and more.</p>
            <a href="https://github.com/GouseShaik7?tab=repositories" target="_blank">Source Code</a>
          </div>
    </div>
  </div>
</template>

<style scoped>
.projects {
  padding: 2rem;
}
.project-list {
  display: flex;
  flex-wrap: wrap;
}
.project {
  margin: 1rem;
  padding: 1rem;
  border: 1px solid #ccc;
  width: 300px;
}
</style>


<template>
  <div class="contact">
   
    <div class="social-links">
     <div class="prof">
          <a class='email' target='_blank' href="mailto:shaikgouse760@gmail.com">Email: shaikgouse760@gmail.com</a>
          <a class='linkedin' target='_blank' href='https://www.linkedin.com/in/mohammedgouseshaik'>LinkedIn: Mohammed Gouse Shaik</a>
          <a class='github' target='_blank' href='https://github.com/GouseShaik7'>GitHub: GouseShaik7</a>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      message: ''
    };
  },
  methods: {
    submitForm() {
      alert(`Message from ${this.name} sent!`);
      // Implement your form handling here
    }
  }
}
</script>

<style scoped>
.contact {
  text-align: center;
  padding: 2rem;
}
.contact form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.social-links a:hover {
    text-decoration: underline;
  }
  .prof{
    margin-top: 30px;
    margin-left: auto;
  }
  .email{
    top: 50px;
    color: white;
    text-decoration: none;
    padding: 15px;
    background-color: 	#3e65cf;
    width: 200px;
  }
  
  .linkedin{
    color: white;
    padding: 15px;
    top: 50px;
    text-decoration: none;
    background-color: #0077B5;
  }
  .github{
    color: white;
    padding: 15px;
    top: 50px;
    text-decoration: none;
    margin-top: 120px;
    background-color: #000000;
  }
</style>

<style>
@media (max-width: 768px) {
    .projects {
      flex-direction: column;
    }
  }

  /* Extra small devices (phones, 600px and down) */
  @media only screen and (max-width: 600px) { 
    body{
            width: 100%;
    }
    .projects {
        flex-direction: column;
      }
}
  
  
  /* Small devices (portrait tablets and large phones, 600px and up) */
  @media only screen and (min-width: 600px) {  
    body{
        width: 100%;
}
.projects {
    flex-direction: column;
  }}
  
  /* Medium devices (landscape tablets, 768px and up) */
  @media only screen and (min-width: 768px) {  
    body{
      width: 100%;
    }}
  
  /* Large devices (laptops/desktops, 992px and up) */
  @media only screen and (min-width: 992px) {  
    body{
      width: 100%;
    }}
  
  /* Extra large devices (large laptops and desktops, 1200px and up) */
  @media only screen and (min-width: 1200px) { 
    body{
      width: 100%;
    }}</style>
