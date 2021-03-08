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
  mounted() {
    const existingContacts = JSON.parse(localStorage.getItem("contacts"));
    this.contacts = existingContacts || [];
  },
  methods: {
    addContact(newContact) {
      this.contacts.push(newContact);

      localStorage.setItem("contacts", JSON.stringify(this.contacts));
    }
  }
};
</script>

<style></style>