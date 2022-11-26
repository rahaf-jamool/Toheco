<script>
import TitleHead from "../global/TitleHead.vue";
export default {
  components: { TitleHead },
  name: "ProductDetails",
  data() {
    return {
      data: {
        title: "PURE COTTON T-SHIRT",
        image1: "logo-titlt.png",
      },
      brands: [
        {
          id: "1",
          image: "image1.jpg",
          url: "#",
        },
        {
          id: "2",
          image: "image2.jpg",
          url: "#",
        },
        {
          id: "3",
          image: "image3.jpg",
          url: "#",
        },
        {
          id: "4",
          image: "image4.jpg",
          url: "#",
        },
        {
          id: "5",
          image: "image5.jpg",
          url: "#",
        },
        {
          id: "6",
          image: "image6.jpg",
          url: "#",
        },
      ],
      swiperOptions: {
        loop: true,
        slidesPerView: 2,
        slidesPerView: "auto",
        centeredSlides: true,
        spaceBetween: 30,
        pagination: {
          el: ".swiper-pagination",
          dynamicBullets: false,
        },
        breakpoints: {
          550: {
            slidesPerView: 3,
          },
          768: {
            slidesPerView: 4,
          },
          1200: {
            slidesPerView: 5,
          },
        },
      },
    };
  },
  methods: {
    onSwiperRedied(swiper) {
      console.log("Swiper redied!", swiper);
    },
    onSwiperClickSlide(index, reallyIndex) {
      console.log("Swiper click slide!", reallyIndex);
    },
  },
};
</script>

<template>
  <div class="product-details">
    <title-head
      :title="data.title"
      :image1="data.image1"
    />
    <div class="specifications">
      <div class="slider">
        <div
          id="carouselExampleControls"
          class="carousel slide"
          data-bs-ride="carousel"
        >
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img
                src="../../public/assets/images/موقع2-05.jpg"
                class="d-block w-100"
                alt="..."
              />
            </div>
            <div class="carousel-item">
              <img
                src="../../public/assets/images/موقع2-06.jpg"
                class="d-block w-100"
                alt="..."
              />
            </div>
          </div>
          <button
            class="carousel-control-prev"
            type="button"
            data-bs-target="#carouselExampleControls"
            data-bs-slide="prev"
          >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button
            class="carousel-control-next"
            type="button"
            data-bs-target="#carouselExampleControls"
            data-bs-slide="next"
          >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
        <div class="photos-video">
          <h3>Photos Videos</h3>
          <swiper
            class="swiper images-slider"
            id="images-slider"
            :options="swiperOptions"
            @ready="onSwiperRedied"
            @clickSlide="onSwiperClickSlide"
          >
            <swiper-slide v-for="item in brands" :key="item.id">
              <div class="item">
                <div class="image">
                  <img
                  :src="require('../../public/assets/images/' + item.image)"
                  alt=""
                />
                </div>
              </div>
            </swiper-slide>
          </swiper>
        </div>
        <div class="social-media-products">
          <img
            src="../../public/assets/images/icon/save.png"
            alt=""
            width="5%"
          />
          <img
            src="../../public/assets/images/icon/send.png"
            alt=""
            width="5%"
          />
          <img
            src="../../public/assets/images/icon/twitter.png"
            alt=""
            width="5%"
          />
          <img
            src="../../public/assets/images/icon/google.png"
            alt=""
            width="5%"
          />
          <img
            src="../../public/assets/images/icon/facebook.png"
            alt=""
            width="5%"
          />
          <img
            src="../../public/assets/images/icon/pdf.png"
            alt=""
            width="5%"
          />
        </div>
      </div>
      <div class="spacific">
        <h3>Specifications</h3>
        <ul>
          <li>Year <small>2011</small></li>
          <li>Stock no. <small>DZ1001</small></li>
          <li>Model <small>D6R</small></li>
          <li>Serial Number <small>S6T00268</small></li>
          <li>Condition <small>Used</small></li>
          <li>Location <small>JAFZA, Dubai, UAE</small></li>
          <li>Working Hours <small>10,350</small></li>
        </ul>
      </div>
    </div>
    <div class="row details">
      <div class="col-md-6 col-sm-12 shippin">
        <h4>Shipping Dimensions</h4>
      </div>
      <div class="col-md-6 col-sm-12">
        <ul>
          <li>Length: <b>4.90</b> M</li>
          <li>Width: <b>2.44</b> M</li>
          <li>Height: <b>3.19</b> M</li>
          <li>Weight: <b>18143.7</b> KG</li>
        </ul>
      </div>
    </div>
    <form>
      <div class="row">
        <div class="col-6">
          <input type="text" class="form-control" placeholder="Name" />
        </div>
        <div class="col-6">
          <input type="text" class="form-control" placeholder="Phone Number" />
        </div>
        <div class="col-6 mt-4">
          <input type="text" class="form-control" placeholder="E-mail" />
        </div>
        <div class="col-6 mt-4">
          <input type="text" class="form-control" placeholder="Company Name" />
        </div>
        <div class="col-6 mt-4">
          <input
            type="text"
            class="form-control"
            placeholder="Contact Number"
          />
        </div>
        <div class="col-6 mt-4">
          <input type="text" class="form-control" placeholder="Notes" />
        </div>
      </div>
      <div class="row">
        <button id="btn9" class="btn-9"><span>Add Inquiry</span></button>
      </div>
    </form>
  </div>
</template>

<style scoped></style>
