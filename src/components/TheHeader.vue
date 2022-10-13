<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand href="#">
        <!--<BootstrapIcon icon="house" aria-hidden="true"></BootstrapIcon> Checked Spot
          -->
          <img src="logo.png" height="40" width="100"/>
      </b-navbar-brand>
      Contact : 9686496343 for all your property needs.
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
  props: {
    msg: String,
  },
};
</script>