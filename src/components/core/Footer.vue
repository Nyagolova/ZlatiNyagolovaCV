<template>
  <v-footer
    height="88"
    class="justify-center"
  >
  Zlatina Nyagolova ® 2020
    <social-media large />
  </v-footer>
</template>

<script>
export default {
  components: {
    SocialMedia: () => import('@/components/SocialMedia')
  }
}
</script>
