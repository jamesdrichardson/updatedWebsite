<template>
  <div class="about" id=right_panel_grid>
    <h1 id = "name" class="subtitle">James Richardson</h1>
            <h2 id = "desc" class="subtitle">Skilled Full Stack Software Developer and IT Expert</h2>
            <img src = "../assets/Headshot.jpeg" class="headshot" id="headshot">
            <div id="bio">
                <p>
                    My interests include writing, software development, philosophy, and music.
                     Previously I worked as a Senior IT Support Engineer at AlphaSights and 
                     currently I work at Netflix as an IT Support Specialist. I am now looking 
                     to break into the Software Development field, which has always been one of 
                     my passions. I am a hard worker, as well as a team player. I am also inquisitive
                      and will continue to work my hardest until the task in front of me is completed.
                </p>
            </div>
            <div id="skills">
                <h3 class="subtitle">Skills</h3>
                <p>
                    I have worked with the following software development technologies: Java, JavaScript, 
                    TypeScript, C#, .NET, PostgreSQL, Vue.JS, Spring Boot, HTML, and CSS.
                    My non development skills and technologies include: Microsoft Suite, SaaS platform 
                    administration (ie: Slack, Zoom, Google, and Microsoft), Public Speaking, Leadership, and Management.
                </p>
            </div>
            <div id="education">
                <h3 class="subtitle">Education and Experience</h3>
                <p>
                    Most recently I graduated from <a href="https://www.techelevator.com/">Tech Elevator</a> completing their Full Stack Java development course.
                    <br>
                    Previously, I graduated from <a href="https://www.bucknell.edu/">Bucknell University</a> in 2017 with a BA in Classics and Ancient
                    Mediterranean Studies. <br> 
                    My current position is as an IT support speicalist at Netflix. Before working at Netflix and beginning Tech Elevator, I worked as a 
                    Senior IT Support Engineer at AlphaSights. Prior to that I was a Technical Specialist at Apple. You can find more information about those postions
                    on my resume, linked to the left of this section!
                </p>
            </div>
  </div>
</template>

<style scoped>

#right_panel_grid {
  /*grid-area: right; */
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-areas:
      "name headshot"
      "desc desc"
      "bio bio"
      "skills edu";
  gap: 15px;
  align-content: center;
  height: 100vh;
  justify-content: center;
  justify-items: end;
  align-items: start;
}

#name {
    grid-area: name;
    font-size: 4em;
    margin-top: 0%;
    margin-bottom: 0%;
}

#desc {
    grid-area: desc;
    margin-top: 0%;
    margin-bottom: 0%;
    text-align: end;
    font-size: 1.5em;
}

#bio {
    grid-area: bio;
}

#skills {
    grid-area: skills;
}

#education {
    grid-area: edu;
}


#headshot{
  width: 200px;
  height: auto;
  grid-area: headshot;

}

.subtitle{
  font-weight: bolder;
}

@media (min-width: 1024px) {
  .about {
    display: flex;
    align-items: center;
  }
}
</style>
