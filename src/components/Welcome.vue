<template>
  <section
    id="welcome"
    class="hide-overflow"
  >
    <v-layout>
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/welcome3-small.jpg')"
          height="100vh"
        />
      </v-flex>

      <v-flex
        xs12
        md6
        align-content-space-between
        layout
        :pa-5="$vuetify.breakpoint.smAndDown"
        wrap
      >
        <base-bubble-1/>

        <v-layout
          align-center
          justify-center
        >
          <v-flex
            xs10
            md6
            
          >
            <base-text>
              Hey there! <br> My name is
            </base-text>
            <div class="mainheading display-3 v-heading mb-3 font-weight-light">ZLATINA NYAGOLOVA</div>
            <base-text>
              FRONT-END WEB DEVELOPER with passion for writing beautiful and functional UI/UX
            </base-text>

<!-- 
            <base-btn class="mt-4">
              Learn More!
            </base-btn> -->

            
          </v-flex>
        </v-layout>

        <base-bubble-2 />
        <!-- <base-bubble-3 /> -->
 
      </v-flex>
    </v-layout>
  </section>
</template>
 
<script>
export default {

}
</script>

<style scoped>
 .mainheading {
  color:teal !important;
  font-weight: bold !important;
 }
</style>
