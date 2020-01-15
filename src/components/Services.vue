<template>
  <section
    id="services"
    class="hide-overflow"
  
  >
    <v-layout  
>
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/laptop.jpg')"
          height="100%"
          max-height="800px"
        />
      </v-flex>
      <v-flex
        xs12
        md6
        text-xs-center
        pa-5
      >
        <v-layout
          align-center
          justify-center
          fill-height
          wrap
        >
          <v-flex xs12 >
            <!-- <base-bubble-2
              style="transform: translateX(55%)"
            /> -->
            <!-- <base-heading>
              Experience and skillset
            </base-heading> -->

            <div class="mainheading display-3 v-heading mb-3 font-weight-light">Career Timeline and Certification</div>

            <base-text class="mb-5">
              My professional experience over the years
            </base-text>

                <v-timeline :dense="true" white>
                <v-timeline-item
                  v-for="(year, i) in years"
                  :key="i"
                  :color="year.color"
                  small
                >
                  <div class="py-4">
                    <h2 :class="`headline font-weight-light mb-4 ${year.color}--text`">{{year.title}}</h2>
                    <div>
                      {{year.text}}
                    </div>
                  </div>
                </v-timeline-item>
              </v-timeline>

          </v-flex>

          <v-flex xs12 >
            <v-avatar tile style="margin-left: 1.6em;">
              <v-img
                :src="require('@/assets/Softuni.png')"
              />
              <!-- 2019 - VueJS Fundamentals, Software University  -->
            </v-avatar>
              <a  href="http://www.slideshare.net/slideshow/embed_code/key/sJ017KIWNLjWx4" target="_blank"  > 2019 - VueJS Fundamentals, Software University</a>  
          </v-flex>

          <v-flex xs12>
            <v-avatar tile style="margin-left: 1.6em;">
              <v-img
                :src="require('@/assets/MS.png')"
              /> 
            </v-avatar>
             <a  href="http://www.slideshare.net/slideshow/embed_code/key/BKKy2Tgn1c6GQy" target="_blank"  > 2017 - Programming in HTML5 with JavaScript and CSS3, Microsoft</a> 
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    years: [
      {
        color: 'cyan',
        title: 'Front-End Web Developer, Shopmetrics Ltd.',
        text: '2015 - Present'
      },
      {
        color: 'green',
        title: 'Marketing expert, MicroAcount Ltd.',
        text: '2012 - 2015'
      },
      {
        color: 'pink',
        title: 'Technical University of Varna, Bachelor\'s Degree, Computer Software Engineering',
        text: '2009 - 2013'
      }
    ],
    services: [
      {
        name: 'Research',
        icon: 'mdi-clipboard-text-outline',
        blurb: 'Curabitur et nisi semper,<br> pellent e sque '
      },
      {
        name: 'Design',
        icon: 'mdi-pencil-outline',
        blurb: 'Curabitur et nisi semper, <br>pellent.'
      },
      {
        name: 'Development',
        icon: 'mdi-settings-outline',
        blurb: 'Curabitur et nisi semper, <br>pellent.'
      },
      {
        name: 'Support',
        icon: 'mdi-account',
        blurb: 'Curabitur et nisi semper, <br>pellent.'
      }
    ]
  })
}
</script>
<style scoped>
 a {
   margin-left: 1.3em; 
   text-decoration: none;
 }
</style>