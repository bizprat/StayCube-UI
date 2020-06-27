<template>
  <div class="my-6">
    <h1>Popular Mess</h1>
    <v-row>
      <v-col v-for="(mess, i) in 3" :key="i" lg="4">
        <v-card dark>
          <v-img
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
            height="200px"
          >
            <v-card-title>Supriya Mess</v-card-title>
          </v-img>
          <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
            <div>Whitsunday Island, Whitsunday Islands</div>
          </v-card-text>
          <v-card-actions>
            <v-btn color="red">Open</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Mess',
}
</script>

<style></style>
