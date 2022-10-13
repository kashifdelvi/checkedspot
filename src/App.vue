<template>
  <div class="page">
    <b-container class="bv-example-row">
      <TheHeader />
      <TheMarkettingSection/>
      <VerifiedProjects/>
    </b-container>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheMarkettingSection from "./components/TheMarkettingSection.vue";
import VerifiedProjects from "./components/VerifiedProjects.vue";

export default {
  name: "App",
  components: { TheHeader,TheMarkettingSection,VerifiedProjects },
};
</script>

