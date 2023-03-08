<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/projects">Projects</router-link> |
      <router-link to="/contact">Contact</router-link>
    </div>
    <router-view />
    <div id="footer">
      <p>Copyright © 2023 jackieodonnell. All Rights Reserved.</p>
      <a href="https://github.com/jackieodonnell/portfolio-2022" target="_blank"
        >View Portfolio Repo</a
      >
    </div>
  </div>
</template>

<style src="./assets/styles.css"></style>
