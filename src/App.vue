<template>
  <app-header />
  <router-view/>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'

export default {
  components: {
    AppHeader
  }
}
</script>
