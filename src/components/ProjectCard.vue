<template>
  <div class="project-card">
    <h1> {{project.title}} </h1>
    <p> {{project.description}} </p>
    <p> {{project.tech}} </p>
    <button>Demo</button>
    <button>Source Code</button>
  </div>
</template>

<script>
export default {
    name: "project-card",
    props: ["project"]
}
</script>

<style>
.project-card {
    background-color: #ecebebe5;
    padding: 10px;
    width: 90%;
    border-radius: 10px;
    border: 1.5px solid rgba(135, 135, 135, 0.539);
    box-shadow: 1px 4px 12px 6px rgba(47, 46, 46, 0.73);
    margin-left: 5%;
    text-align: left;
    color:#313030;
}

.project-card h1 {
    font-size: 1.5rem;
}


</style>