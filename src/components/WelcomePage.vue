<script setup lang="ts">

</script>

<template>
  <div class="greetings">
    <h1 class="home-head">Hi, Welcome to my website!</h1>
    <h3>
      Click one of the links on the left to learn more about me! CLick the icons below to access
      my GitHub and LinkedIn.
      <br/><br/>
    </h3>
    <div id="findme">
      <ul id="social_icons">
        <li><a href="https://www.github.com/jamesdrichardson"><img class="logo"
          src="../assets/github-mark.png"></a></li>
        <li><a href="https://www.linkedin.com/in/james-richardson-professional/"><img class="logo"
          src="../assets/LI-In-Bug.png"></a></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}
.logo {
    width: 50px;
}

.greetings{
  height: 100vh;
    align-items: stretch;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

#social_icons {
    list-style: none;
    display: flex;
    justify-content: space-evenly;
    margin: 20px 20px;
    padding: 0;
    padding-inline-start: 0px;
    margin-block-start: 0;
    margin-block-end: 0;
    
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
