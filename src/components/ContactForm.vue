<template>
  <div>
    <h3 class="teal--text">New Contact</h3>
    <v-form>
      <v-text-field outlined label="First Name" v-model="form.firstName" />
      <v-text-field outlined label="Last Name" v-model="form.lastName" />
      <v-text-field type="number" outlined label="Phone" v-model="form.phone" />
      <v-select outlined label="Phone Type" :items="phoneTypeOptions" v-model="form.type" />
      <v-text-field outlined label="Email" v-model="form.email" />
    </v-form>
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
      },
      phoneTypeOptions: ["Home", "Cell", "Office"]
    };
  }
};
</script>

<style></style>