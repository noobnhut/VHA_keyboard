<template>
  <div class="bg-gray-50">
    <headerVue />
    <div class="container mx-auto">
      <banner />
      <service />
      <contact />
      
    </div>  
    <footerVue/>
  </div>

</template>

<script>
import headerVue from "../components/header.vue";
import banner from "../components/banner.vue";
import service from "../components/service.vue";
import contact from "../components/contact.vue";
import footerVue from "../components/footerVue.vue";
export default {
  data() {
    return {};
  },
  components: {
    headerVue,
    banner,
    service,
    contact,
    footerVue
  },
};
</script>
