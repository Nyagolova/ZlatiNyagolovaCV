<template>
  <section
    id="recent-projects"
    class="hide-overflow"
  >
    <v-layout>
      <v-flex
        xs12
        md6
        class="teal lighten-3"
        text-xs-center
        pa-5
        white--text
      >
        <!-- <base-bubble-1
          style="transform: rotate(180deg) translateX(25%)"
        /> -->
        <base-heading>
          About me
        </base-heading>

        <base-text class="mb-5">
          <!-- <p>Thank you for visiting my website. </p> -->
           <!-- <p><span style="color:black">My name is <strong>Zlatina</strong> and I work as a front-end web developer  in Varna, Bulgaria. </span> </p> -->
           <p>I have a passion for activities that require <strong>creativity</strong> since childhood. As a kid, I loved drawing, pottering, lego and puzzle, sewing, writing and going to various off school classes such as gardening, funny mathematics, computer science, and foreign languages.  
          I also loved going to the local library to rent books (mostly comics and gamebooks). 
          As an adult, I always try to make time for my hobbies, because I think they are <strong>important for my growth as a person</strong>, both personally and professionally. And also keeping me sane. :)   </p>

          <p>
          <ul>
            <li>I love <span class="emphasize">READING</span> because it's <b>relaxing</b> and develops your focus and expands your mindset. </li>
            <li>I love <span class="emphasize">DRAWING</span> because it's <b>creative</b> and develops your imagination and confidence. </li>
            <li>I love <span class="emphasize">COOKING</span> because it's <b>dynamic</b> and develops your skills in dealing with critical situations.  </li>
          </ul></p>

          <p><small>I also love traveling, camping, anime and the Asian culture, cats, dogs, and animals in general.</small></p>
        </base-text>

        <!-- <v-card color="grey darken-3">
          <v-container
            grid-list-md
            pa-2
          >
            <v-layout wrap>
              <v-flex
                v-for="project in projects"
                :key="project"
                xs12
                md6
              >
                <a href="#">
                  <v-img
                    :src="require(`@/assets/${project}.jpeg`)"
                    max-height="300"
                  />
                </a>
              </v-flex>
            </v-layout>
          </v-container>
        </v-card> -->
      </v-flex>
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/recentprojects.jpg')"
          height="100%"
        />
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    projects: [
      'project1',
      'project2',
      'project3',
      'project4'
    ]
  })
}
</script>
<style scoped>
.emphasize {
  color: black;
  font-weight: bold;
  font-size: 1.2em;
}

ul > li {
  color: black;
} 
</style>
