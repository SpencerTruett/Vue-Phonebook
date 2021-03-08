<template>
  <div>
    <ContactsTable :contacts="contacts" />
    <ContactForm @contact-submit="addContact" />
  </div>
</template>

<script>
import ContactForm from "./ContactForm.vue";
import ContactsTable from "./ContactsTable.vue";

export default {
  components: { ContactForm, ContactsTable },
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