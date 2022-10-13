<template>
  <div>
    <h3 class="mb-10">Checked and Verified <BootstrapIcon icon="check" aria-hidden="true"></BootstrapIcon></h3>
    <b-card
      title="Pinacle Green"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem"
      class="mb-2"
    >
      <b-card-text>
        A farm land in your city limits ...
        <h1>Details comming soon ......</h1>
      </b-card-text>

      <b-button href="#" variant="primary">
        View Details
      </b-button>
    </b-card>
  </div>
</template>
  
  <script>
export default {
  name: "VerifiedProjects",
  props: {
    msg: String,
  },
};
</script>