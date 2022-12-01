<template>
  <div class="home">
    <div class="name">
      <!-- <h1 id="first-name">jackie o'donnell.</h1> -->
      <vue-typed-js :strings="['Jacqueline', 'Jackie O\'Donnell.']" :smartBackspace="true" :typeSpeed="120" :backSpeed="80" :backDelay="50" :startDelay="1200">
        <h1 class="typed-name">Hi, I'm <span class="typing typed-name"></span></h1>
      </vue-typed-js>
    </div>

    <div class="details">
      <div class="bio">
        <h2>about me:</h2>
        <p>Full-stack  web  developer  with  a  knack  for  finding  and  solving  problems. 
          Self-motivated,  detail-oriented,  and  always learning.</p>    
      </div>
      <div class="skills">
        <h2>tech stack:</h2>
        <p>Java, JavaScript, SQL, Python, HTML, CSS, Spring Boot, Vue.js, PostgreSQL, 
          jQuery, Git, JUnit, Cypress, Maven</p>
      </div>
    </div>



  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'Home',
  components: {
  },
}
</script>

<style scoped>


.name {
  display: flex;
  flex-direction: row;
  justify-content: center;
  min-height: 50vh;
}
.typed-name{  
  font-family: "Poppins-Regular";
  font-size: 4rem;
  font-weight: 600;
  color:#ecebeb;
}

.typing {
  color:#e25250;
}

#about-me {
  margin-top: 30px;
}

.details {
  font-family: "Poppins-Regular";
  font-size: 1.8rem;
  font-weight: 400;
  color: #ecebeb;
  display: flex;
  flex-direction: column;
}

.bio, .skills {
  display: flex;
  flex-direction: column;
  color:  #ecebeb;
  text-transform: lowercase;
  align-items: flex-start;
  margin-left: 10%;
  margin-right: 10%;
  text-align: left;
  font-size: 1.3rem;
  }

.bio p {
  margin-right: 30%;
  font-size: 1.2rem;
  margin-top: 0;
}
.skills {
  align-items: flex-end;
  text-align: right;
}
.skills p {
  margin-left: 30%;
  font-size: 1.2rem;
  margin-top: 0;
  margin-bottom: 10%;
}



</style>
