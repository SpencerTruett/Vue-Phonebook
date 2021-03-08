<template>
  <v-app>
    <v-app-bar app color="teal" dark>
      <div class="d-flex align-center"></div>
      <h1>Phonebook</h1>
    </v-app-bar>

    <v-main class="ma-5">
      <Phonebook />
    </v-main>
  </v-app>
</template>

<script>
import Phonebook from "./components/Phonebook";

export default {
  components: {
    Phonebook
  }
};
</script>
