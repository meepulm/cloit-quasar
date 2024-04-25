<template>
  <q-layout view="hhh lpr fff">
    <TemplateNavbar />
    <q-page-container class="no-padding">
      <router-view />
    </q-page-container>
    <TemplateFooter />
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";
import TemplateNavbar from "components/template/TemplateNavbar.vue";
import TemplateFooter from "components/template/TemplateFooter.vue";

export default defineComponent({
  name: "MainLayout",

  components: {
    TemplateNavbar,
    TemplateFooter,
  },
});
</script>
