<template>
  <section
    id="about"
    class="hide-overflow"
  >
    <v-layout teal lighten-3


>
      <v-flex
        xs12
        md6
        pa-5
        white--text
      >
        <!-- <base-bubble-1
          style="transform: translate(5%, -5%)"
        /> -->
        <base-heading  >
          Skillset
        </base-heading>

        <!-- <base-text class="mb-5">
          Social media: stackoverflow, linkedin, github, instagram, facebook
        </base-text> -->

        <!-- <base-subheading  >
          Experience and Skillset
        </base-subheading> -->

        <!-- <base-text class="mb-5">
          stackoverflow, linkedin, github, instagram, facebook
        </base-text> -->

        <v-layout
          align-center
          justify-center
          fill-height
          wrap
        >
          <v-flex
            v-for="(service, i) in services"
            :key="i"
            md6
            text-xs-center
            mb-4
          >  <v-avatar

              size="64"
              tile
            >
               
              <v-img
                :src="require(`@/assets/${service.icon}`)"
              />
            </v-avatar>   <base-text>
               <base-subheading  > {{service.name}} </base-subheading>
              <div v-html="service.blurb" />
            </base-text>
          </v-flex>
        </v-layout>
        <!-- <v-alert
          outlined
          color="white"
        >
          <v-layout
            v-for="(skill, i) in skills"
            :key="i"
            style="color: white;"
            wrap
          >
            <v-flex
              xs6
              text-uppercase
              v-text="skill.name"
            />
            <v-flex
              xs6
              text-xs-right
              v-text="`${skill.value}%`"
            />
            <v-progress-linear
              :value="skill.value"
              color="white"
              height="8"
            />
          </v-layout>
        </v-alert> -->
      </v-flex>
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/photo_2020-01-15_02-01-25.jpg')"
          height="100%"
        />
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    services: [
      {
        name: 'JavaScript, jQuery, HTML, CSS, ExtJS',
        icon: 'js.png',
        blurb: 'Used for creating dynamic User Interfaces'
      },
      {
        name: 'VueJS, Vuex, NuxtJS, Vuetify, Lodash',
        icon: 'logo.png',
        blurb: 'Creating reactive and responsive UIs.'
      },
      {
        name: 'PowerShell, Python, C#',
        icon: 'powershel.png',
        blurb: 'Writing services and scripts for automating various tasks (API calls, requesting services, querying DB data, running tests, etc.)'
      },
      {
        name: 'T-SQL/SQL-Server',
        icon: 'SQL-Server-Logo.png',
        blurb: 'Basic experience on querying data, writing basic stored procedures and maintaining unit tests project'
      },
      {
        name: 'Adobe Photoshop, Adobe Illustrator, Adobe After Effects',
        icon: 'photoshop.png',
        blurb: 'Experience with graphic design: Creating advertisement materials like flyers, banners, newspaper and magazine posts'
      },
      {
        name: 'Google AdWords, Google Analytics, Webmaster Tools',
        icon: 'ga.png',
        blurb: 'SEO Support, online campaigns, and reports delivering'
      }
    ],
    skills: [
      {
        name: 'Web Design',
        value: 100
      },
      {
        name: 'Web Development',
        value: 75
      },
      {
        name: 'Web Support',
        value: 90
      }
    ]
  })
}
</script>
