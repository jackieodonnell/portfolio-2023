<template>
  <div class="projects">
    <project-card class="animate pop" v-bind:project="project1" />
    <project-card class="animate pop delay-1" v-bind:project="project2" />
    <project-card class="animate pop delay-2" v-bind:project="project3" />
    <project-card class="animate pop delay-3" v-bind:project="project4" />
  </div>
</template>

<script>
import ProjectCard from "../components/ProjectCard.vue";

export default {
  name: "projects-view",
  components: {
    ProjectCard,
  },
  data() {
    return {
      project1: {
        title: "Incrementum: eLearning Platform",
        description:
          "A browser-based K-12 online education portal that enables teachers and students to manage courses, lessons, assignments, and grades.",
        tech: ["Java", "Vue.js", "PostgreSQL", "Spring Boot"],
        demo: "https://incrementum-learning.netlify.app/",
        repo: "https://github.com/jackieodonnell/eLearningPortal",
        imgName: "elearning.png",
      },
      project2: {
        title: "PayBack: Money Lending App",
        description:
          "A responsive web application that allows users to manage lending and borrowing money with friends and family. Awarded 'Most Creative App' at the GDI 2022 Hackathon.",
        tech: ["Express.js", "React Native", "Typescript", "PostgreSQL"],
        demo: "",
        repo: "https://github.com/jackieodonnell/PayBack-App",
        imgName: "payback-app.png",
      },
      project3: {
        title: "PayBack: Admin Analytics Dashboard",
        description:
          "A real-time KPI dashboard that leverages the PayBack live database to analyze users, loans, and application usage data.",
        tech: ["Express.js", "Vue.js", "Apexcharts", "PostgreSQL"],
        demo: "",
        repo: "https://github.com/jackieodonnell/PayBack-AdminDashboard",
        imgName: "payback-dashboard.png",
      },
      project4: {
        title: "Wordcraft",
        description:
          "An original word game developed with Vue.js and optimized for mobile screens. The objective is to use all letters on the board in as few 5-letter words as possible.",
        tech: ["JavaScript", "Vue.js"],
        demo: "https://wordcraft.netlify.app/",
        repo: "https://github.com/jackieodonnell/Wordcraft",
        imgName: "wordcraft.png",
      },
    };
  },
};
</script>

<style scoped>
.projects {
  max-width: 1200px;
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
}
.animate {
  animation-duration: 1s;
  animation-delay: 0.25s;
  animation-name: animate-fade;
  animation-timing-function: cubic-bezier(0.26, 0.53, 0.74, 1.48);
  animation-fill-mode: backwards;
  margin-bottom: 10px;
  border-top: 2px solid #3c3a3a7d;
  box-shadow: 13px 4px 22px 6px rgba(47, 46, 46, 0.937);
  transition: all 0.2s ease-in-out;
}

.animate:hover {
  transform: scale(1.05);
}

.animate.pop {
  animation-duration: 0.5s;
  animation-name: animate-pop;
  animation-timing-function: cubic-bezier(0.26, 0.53, 0.74, 1.48);
}
.delay-1 {
  animation-delay: 0.5s;
}
.delay-2 {
  animation-delay: 0.75s;
}
.delay-3 {
  animation-delay: 1s;
}

@keyframes animate-pop {
  0% {
    opacity: 0;
    transform: scale(0.5, 0.5);
  }

  100% {
    opacity: 1;
    transform: scale(1, 1);
  }
}
</style>
