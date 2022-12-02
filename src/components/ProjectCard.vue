<template>
  <div class="project-card">
    <img
      :src="require('../assets/' + this.imgName + '')"
      alt="elearning-homepage"
      class="project-img"
    />
    <div class="project-content">
      <h1>{{ project.title }}</h1>
      <p>{{ project.description }}</p>
      <div class="project-tools">
        <p v-for="tool in project.tech" :key="tool">{{ tool }}</p>
      </div>
      <div class="project-action-btns">
        <button v-if="this.project.demo != ''" v-on:click="ViewProject()">
          View Project
        </button>
        <button v-on:click="ViewCode()">View Code</button>
        <p id="coming-soon" v-if="this.project.demo == ''">
          Live Site Coming Soon!
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "project-card",
  props: ["project"],
  data() {
    return {
      imgName: "",
    };
  },
  created() {
    this.imgName = this.project.imgName;
  },
  methods: {
    ViewProject() {
      window.open(this.project.demo);
    },
    ViewCode() {
      window.open(this.project.repo);
    },
  },
};
</script>

<style>
.project-card {
  padding: 10px;
  width: 90%;
  margin-left: 5%;
  text-align: left;
  display: flex;
  flex-wrap: wrap;
  column-gap: 20px;
  border-radius: 10px;
}

.project-content {
  color: #ecebeb;
  width: auto;
  max-width: 650px;
}

.project-card h1 {
  font-size: 1.5rem;
  font-weight: 500;
}

.project-tools {
  display: flex;
  flex-wrap: wrap;
  column-gap: 20px;
  text-transform: uppercase;
  font-weight: 600;
  color: #e26765;
}
.project-tools p {
  height: fit-content;
  margin-top: 0px;
  margin-bottom: 5px;
}

.project-action-btns {
  margin-top: 10px;
  margin-bottom: 20px;
  display: flex;
  gap: 5%;
}
.project-action-btns button {
  background-color: #ecebeb;
  padding: 5px;
  width: 120px;
  font-family: "Poppins-Regular";
  text-transform: uppercase;
  font-weight: 700;
  border-radius: 8px;
  border: none;
  box-shadow: 13px 4px 22px 3px rgba(30, 29, 29, 0.739);
  transition: all 0.2s ease-in-out;
}

.project-action-btns button:hover {
  background-color: #519cba;
  box-shadow: 13px 4px 22px 3px rgba(30, 29, 29, 0.875);
  transform: scale(1.05);
}

#coming-soon {
  text-transform: uppercase;
  font-weight: 400;
  color: #519cba;
  margin-top: 0;
  margin-bottom: 0;
}

.project-img {
  width: 50%;
  min-width: 320px;
  height: auto;
  box-shadow: 3px 24px 12px 6px rgba(47, 46, 46, 0.937);
  border-radius: 10px;
  -webkit-mask-image: linear-gradient(black 30%, transparent);
  mask-image: linear-gradient(black, transparent);
}

@media screen and (min-width: 1000px) {
  .project-card {
    flex-wrap: nowrap;
  }
}
</style>
