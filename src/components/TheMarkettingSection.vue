<template>
  <carousel :items-to-show="1" :wrap-around="true" :autoplay="30000">
    <slide v-for="slide in slides" :key="slide" slideWidth="100%" autoplay=10>
      <div class="carousel__item slideContainer">
        <img :src="slide.imageURL" class="image"/>
        <b-button class="postAdd" variant="success">
            <h2>CLICK ME</h2>
            POST YOUR PROPERTY FOR 
            <H3>FREE</H3>
        </b-button>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>
  
  <script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
  name: "TheMarketting",
  data() {
    return {
      slides: [
        {
          imageURL: "https://picsum.photos/1024/480/?image=54",
        },
        {
          imageURL: "https://picsum.photos/1024/480/?image=58",
        },
        {
          imageURL: "https://picsum.photos/1024/480/?image=59",
        },
        {
          imageURL: "https://picsum.photos/1024/480/?image=54",
        },
      ],
    };
  },
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
};
</script>
<style scoped>
.postAdd {
  position: absolute;
  top: 200px;
  left: 40%;
  height: 150px;
}
.slideContainer {
  position: relative;
}

.carousel__item {
  min-height: 200px;
  width: 100%;
  background-color: #fff;
  color: var(--vc-clr-white);
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carousel__slide {
  padding: 0px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}
.image{
    width:100%
}
</style>