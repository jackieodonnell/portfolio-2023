<template>
  <div class="home">
    <div class="name">
      <h1 id="first-name">jackie o'donnell.</h1>
    </div>
    <h2 id="about-me">about me:</h2>
    <p id="bio">Full-stack  web  developer  with  a  knack  for  finding  and  solving  problems. 
      Self-motivated,  detail-oriented,  and  always learning.</p>
    <h2 id="tech-stack">tech stack:</h2>
    <p id="skills">Java, JavaScript, SQL, Python, HTML, CSS, Spring Boot, Vue.js, PostgreSQL, 
      jQuery, Git, JUnit, Cypress, Maven</p>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  }
}
</script>

<style scoped>


.name {
  display: flex;
  flex-direction: row;
  margin-top: 15%;
  justify-content: center;
}
#first-name{  
  font-family: monospace;
  font-size: 4rem;
  font-weight: 400;
  color: white;
  margin-bottom: 10%;
  position: relative
}

#first-name::before,
#first-name::after{
  content: ''; 
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}

#first-name::before{
  background: hsl(285, 6%, 14%);
  animation: typewriter 3s steps(17) 1s forwards;
}
#first-name::after{
  width: .125em;
  background: rgba(243, 187, 83, 0.937);
  animation: typewriter 3s steps(17) 1s forwards,
  blink 750ms steps(2, start) infinite;
}

@keyframes typewriter {
  to {
    left: 100%;
  }
}

@keyframes blink {
  to {
    visibility: hidden;
  }
}

#about-me, #bio {
  font-family: monospace;
  font-size: 1.8rem;
  font-weight: 400;
  color: white;
  text-transform: lowercase;
  text-align: left;
  margin-left: 10%;
}

#bio{
  margin-right: 50%;
  font-size: 1rem;
  margin-bottom: 0px;
}

#tech-stack, #skills {
  margin-top: 0px;
  font-family: monospace;
  font-size: 1.8rem;
  font-weight: 400;
  color: white;
  text-transform: lowercase;
  text-align: right;
  margin-right: 10%;
}

#skills {
  text-align: right;
  margin-left: 50%;
  font-size: 1rem;
}
</style>
