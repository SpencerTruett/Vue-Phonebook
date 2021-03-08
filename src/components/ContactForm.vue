<template>
  <div>
    <h3 class="teal--text">New Contact</h3>
    <v-form></v-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        firstName: "",
        lastName: "",
        phone: "",
        type: "",
        email: ""
      }
    };
  }
};
</script>

<style></style>