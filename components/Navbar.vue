<template>
  <nav>
    <v-app-bar color="deep-purple accent-4" dense dark>
      <v-toolbar-title>StayCube</v-toolbar-title>

      <v-menu>
        <template>Mess</template>
      </v-menu>

      <v-spacer></v-spacer>

      <v-menu offset-x>
        <template v-slot:activator="{ on }">
          <v-btn color="green" v-on="on">
            <v-icon left>mdi-menu-down</v-icon>
            <span>Become partner</span>
          </v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(partner, i) in partners" :key="i">
            {{ partner.title }}
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      partners: [
        { title: 'Coaching', route: '' },
        { title: 'College', route: '' },
      ],
    }
  },
}
</script>

<style></style>
