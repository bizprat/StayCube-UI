<template>
  <div>
    <v-app>
      <navbar></navbar>

      <home-body></home-body>
    </v-app>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import Body from '@/components/Body'

export default {
  components: {
    Navbar,
    'home-body': Body,
  },
  data() {
    return {}
  },
}
</script>
