<template>
  <ContactForm @contact-submit="addContact" />
</template>

<script>
import ContactForm from "./ContactForm";

export default {
  components: { ContactForm },
  data() {
    return {
      contacts: []
    };
  },
  methods: {
    addContact(newContact) {
      this.contacts.push(newContact);
    }
  }
};
</script>

<style></style>