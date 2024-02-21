<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="header">
      <q-toolbar>
        <q-toolbar-title> </q-toolbar-title>

         <q-btn outline rounded color="primary" label="Say Hello" />

      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";
import Contact from 'src/components/ContactPage.vue';

export default defineComponent({
  name: "MainLayout",

  components: {
    Contact
  },

  setup() {
    const leftDrawerOpen = ref(false);
  },
});
</script>
<style scoped>
.header{
  background-color: rgb(238, 238, 238);
}
</style>
