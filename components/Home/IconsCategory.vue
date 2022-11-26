<template>
  <div class="icons-category">
    <div class="category">
      <div class="items text show-more-height">
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 23ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Equipments</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 22ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Construction & Mining Equipment</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 23ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Lifting & Material Handling</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 23ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Miscellaneous & Parts</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 21ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Dozer</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 20ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Dump Truck</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 20ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Excavator</h3>
          </div>
        </div>
        <div class="item">
          <div class="image">
            <img
              src="../../public/assets/images/icon/Asset 20ldpi.png"
              alt=""
            />
          </div>
          <div class="title">
            <h3>Loader</h3>
          </div>
        </div>
      </div>
      <div class="btn-items show-more">
        <button>show more</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IconsCategory",
  mounted() {
    $(".show-more").click(function () {
      if ($(".text").hasClass("show-more-height")) {
        $(this).text("(Show Less)");
      } else {
        $(this).text("(Show More)");
      }

      $(".text").toggleClass("show-more-height");
    });
  },
};
</script>

<style scoped>
.show-more-height {
  height: 240px;
  overflow: hidden;
}
</style>
