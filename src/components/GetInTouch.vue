<template>
  <section
    id="get-in-touch"
    class="hide-overflow"
  >
    <v-layout
      teal lighten-3
      white--text
    >
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/bees2.jpg')"
          height="100%"
        />
      </v-flex>
      <v-flex
        xs12
        md6
        pa-5
      >
        <!-- <base-bubble-1 /> -->
        <base-heading class="mb-5">
          Get In Touch
        </base-heading>

        <!-- Social Media - stackoverflow, linkedin, github, instagram, facebook -->

        <a  href="mailto:zlatina.nyagolova@gmail.com" target="_blank"  >
          <v-avatar tile  style="margin: 1em;"  size="62"> 
            <v-img
              :src="require('@/assets/gmail.png')"
            /> 
          </v-avatar>
        </a>

        <a  href="https://stackoverflow.com/users/5312065/nyagolova" target="_blank"  >
          <v-avatar tile  style="margin: 1em;"  size="62"> 
            <v-img
              :src="require('@/assets/stackoverflow.png')"
            /> 
          </v-avatar>
        </a>
        <a  href="https://www.linkedin.com/in/zlatina-nyagolova-56b44a93/" target="_blank"  >
          <v-avatar tile  style="margin: 1em;"  size="62">
            <v-img
              :src="require('@/assets/linkedin.png')"
            /> 
          </v-avatar>
        </a>
        <a  href="https://github.com/Nyagolova" target="_blank"  >
          <v-avatar tile  style="margin: 1em;"  size="62">
            <v-img
              :src="require('@/assets/github.png')"
            /> 
          </v-avatar>
        </a>
        <a  href="https://www.instagram.com/zlati_chan/" target="_blank"  >
          <v-avatar  tile style="margin: 1em;"  size="62">
            <v-img
              :src="require('@/assets/instagram.png')"
            /> 
          </v-avatar>
        </a>
        <a  href="https://www.facebook.com/zlatinanyagolovafeng" target="_blank"  >
          <v-avatar tile  style="margin: 1em;" color="white" size="62">
            <v-img
              :src="require('@/assets/facebook.png')"
            /> 
          </v-avatar>
        </a>

        <!-- <v-sheet
          max-width="600"
          color="transparent"
        >
          <v-text-field
            color="info"
            label="Name"
            solo
            flat
          />
          <v-text-field
            color="info"
            label="Email"
            solo
            flat
          />
          <v-text-field
            color="info"
            label="Subject"
            solo
            flat
          />
          <v-textarea
            color="info"
            label="Message"
            solo
            flat
          />
          <base-btn>Send</base-btn>
        </v-sheet> -->
      </v-flex>
    </v-layout>
  </section>
</template>
