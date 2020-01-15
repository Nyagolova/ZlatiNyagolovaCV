<template>
  <v-app>

    <core-view />

    <core-footer />
  </v-app>
</template>

<script>
export default {
  components: {
    CoreFooter: () => import('@/components/core/Footer'),
    CoreView: () => import('@/components/core/View')
  }
}
</script>
