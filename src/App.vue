<template>
<div id="app">
  <div class="header">
    <router-link to="/">
      <div class="logo">
        <img src="/insta.svg">
      </div>
    </router-link>
    <div class="title">
      <h1>Pandemagram</h1>
      <p> -- "A way for everyone to laugh during these hard times." </p>
    </div>
  </div>

  <div class ="instructions">
    <p> Upload your funniest pandemic-related photos to help other's relieve
    their stress and anxiety! </p>
  </div>

  <div class="content">
    <router-view />
  </div>
  <div class="footer">
    <router-link to="/admin">Share Your Photos</router-link>
    <div>
      <a href="https://github.com/BYU-CS-260-Winter-2020/lab-4-museum-of-ordinary-objects-bparker23">Github</a>
    </div>
  </div>
</div>
</template>

<style>
html {
  box-sizing: border-box;
}
body {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  background: #fff;
  padding: 0px;
  margin: 0px;
}
/* Header */
.header {
  display: flex;
  padding: 10px 100px 0px 100px;
  background-color: #FFFD81;
  color: #1C454F;
}
.title {
  margin-top: 5px;
}
.title h1 {
  font-size: 30px;
}
.content {
  padding: 20px 100px;
  min-height: 500px;
}

.instructions {
display: flex;
padding: 10px 100px 0px 100px;
background: #FFDF82;
color: #1C454F;
}
/* Footer */
.footer {
  height: 50px;
  padding: 20px 100px 0px 100px;
  background: #FFFD81;
  font-size: 12px;
}
.footer a {
  color: #000;
}
h1 {
  font-size: 20px;
}
h2 {
  font-size: 14px;
}
</style>
