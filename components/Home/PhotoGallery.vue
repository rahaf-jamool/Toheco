<template>
  <div class="photo-gallery mb-5">
    <div class="text-arrival">
      <h2>Photo Gallery</h2>
      <img src="../../public/assets/images/icon/Asset 19ldpi.png" alt="" />
    </div>
    <swiper
      class="swiper items-arrivals"
      id="photo-gallery"
      :slides-per-view="3"
      :breakpoints="swiperOptions.breakpoints"
      :speed="1000"
      navigation
      :pagination="{ clickable: true }"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide v-for="item in PhotoGallery" :key="item.id">
        <div class="item">
          <div class="image">
            <img
              :src="require('../../public/assets/images/' + item.image)"
              alt=""
            />
          </div>
        </div>
      </swiper-slide>
      <!-- <div class="swiper-button-prev" slot="button-prev"></div> -->
      <!-- <div class="swiper-button-next" slot="button-next"></div> -->
    </swiper>
  </div>
</template>

<script>
export default {
  name: "PhotoGallery",
  data() {
    return {
      PhotoGallery: [
        {
          id: "1",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
        {
          id: "2",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
        {
          id: "3",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
        {
          id: "4",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
        {
          id: "5",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
        {
          id: "6",
          image: "موقع2-09.jpg",
          subtitle: "HIGHLY EXPERIENCED LAWYERS",
          title: "WE FIGHT FOR RIGHT",
          text: "We Protect The Innocent And Help Our Clients Fight For Their Rights",
          url: "/resentarrival",
          shape1: "slider-shape-1.png",
          shape2: "slider-shape-2.png",
        },
      ],
      swiperOptions: {
        loop: true,
        slidesPerView: 3,
        centeredSlides: true,
        spaceBetween: 50,
        paginationClickable: true,
        autoplay: {
          delay: 10000,
        },
        pagination: {
          el: ".slider-paginations",
          clickable: true,
        },
        breakpoints: {
          300: {
            slidesPerView: 1,
            // spaceBetween: 50
          },
          576: {
            slidesPerView: 2,
            // spaceBetween: 50
          },
          767: {
            slidesPerView: 2,
            // spaceBetween: 50
          },

          991: {
            slidesPerView: 3,
            // spaceBetween: 50
          },
          1200: {
            slidesPerView: 3,
            // spaceBetween: 0
          },
        },
      },
    };
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log("slide change");
    };
    return {
      onSwiper,
      onSlideChange,
    };
  },
};
</script>
