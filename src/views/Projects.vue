<template>
    <div class="about">
      <h1>Coming Soon.</h1> 
      <project-card v-bind:project="project1"/>
    </div>
   
</template>

<script>
    import ProjectCard from '../components/ProjectCard.vue';

    export default {
        name: "projects-view",
        components: {
            ProjectCard
        },
        data() {
            return {
                project1: {
                    title: 'Incrementum: eLearning Platform',
                    description: 'An online K-12 education portal that enables teachers and students to manage courses, lessons, assignments, and grades.',
                    tech: 'Java, Vue.js, PostgreSQL, Spring Boot',
                    demo: 'https://incrementum-learning.netlify.app/login',
                    repo: 'https://github.com/jackieodonnell/eLearningPortal',
                }
            }
        }
    }

</script>


<style scoped>
    .about h1 {
        color: rgb(244, 194, 101);
        font-family: "Poppins-Regular";
        font-weight: 300;
    }
</style>