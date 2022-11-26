<script>
import TitleHead from "../global/TitleHead.vue";

export default {
  name: "listProducts",
  components: { TitleHead },
  data() {
    return {
      data: {
        title: "Equipments",
        image1: "logo-titlt.png",
        image2: "Asset 19ldpi.png",
      },
    };
  },
};
</script>

<template>
  <div class="products">
    <title-head
      :title="data.title"
      :image1="data.image1"
      :image2="data.image2"
    />

    <div class="filter">
      <ul>
        <li>
          sort by:
          <label>
            <select>
              <option>Default</option>
              <option>Manufacturer,Model,Year</option>
              <option>Model,Manufacturer,Year</option>
              <option>Most Recently Updated Listings</option>
              <option>Year</option>
              <option>Manufacturer</option>
              <option>Type</option>
              <option>Equipment Type</option>
            </select>
          </label>
        </li>
        <li>
          show as:
          <label>
            <select>
              <option>Grid view</option>
              <option>List view</option>
            </select>
          </label>
        </li>
        <li>
          Res. per page:
          <label>
            <select>
              <option>50</option>
              <option>100</option>
              <option>150</option>
            </select>
          </label>
        </li>
        <li>
          Equipment type:
          <label>
            <select>
              <option>All</option>
              <option>Asphalt</option>
              <option>Attachment</option>
              <option>Compactor</option>
              <option>Crane</option>
              <option>Dozer</option>
              <option>Drill</option>
              <option>Dump Truck</option>
              <option>ex</option>
              <option>Excavator</option>
              <option>Generator Set</option>
              <option>Grader</option>
              <option>Lift</option>
              <option>Loader</option>
              <option>Lowboy ( Trailer )</option>
              <option>Motor Grader</option>
              <option>Pipe Layer</option>
              <option>Roller</option>
              <option>Scraper</option>
              <option>Spare parts</option>
              <option>Sweeper</option>
              <option>Transit Mixer</option>
            </select>
          </label>
        </li>
        <li>
          <button id="btn9" class="btn-9"><span>Go</span></button>
        </li>
      </ul>
    </div>

    <div class="list-products">
      <div class="col-md-4">
        <div class="card mb-3" style="width: 20rem; margin: auto">
          <img
            class="card-img-top"
            src="../../public/assets/images/موقع2-09.jpg"
            height="380"
            alt="Card image cap"
          />
          <div class="product-detail">
            <h5 class="card-title heading text-center">PURE COTTON T-SHIRT</h5>
            <span class="subheading">Model : D6R</span>
            <!-- <blockquote>
            <p>
              'Little Bit Of Description About The Product Like Size Color And
              Care.'
            </p>
          </blockquote> -->
            <NuxtLink to="/equipments/1"
              ><button type="button" class="btn btn-outline-dark">
                View Details
              </button></NuxtLink
            >
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card mb-3" style="width: 20rem; margin: auto">
          <img
            class="card-img-top"
            src="../../public/assets/images/موقع2-08.jpg"
            height="380"
            alt="Card image cap"
          />
          <div class="product-detail">
            <h5 class="card-title heading text-center">STYLISH T-SHIRT</h5>
            <span class="subheading">Model : D6R</span>
            <!-- <blockquote>
            <p>
              'Little Bit Of Description About The Product Like Size Color And
              Care.'
            </p>
          </blockquote> -->
            <NuxtLink to="/equipments/1"
              ><button type="button" class="btn btn-outline-dark">
                View Details
              </button></NuxtLink
            >
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card mb-3" style="width: 20rem; margin: auto">
          <img
            class="card-img-top"
            src="../../public/assets/images/موقع2-07.jpg"
            height="380"
            alt="Card image cap"
          />
          <div class="product-detail">
            <h5 class="card-title heading text-center">DESIGNER T-SHIRT</h5>
            <span class="subheading">Model : D6R</span>
            <!-- <blockquote>
            <p>
              'Little Bit Of Description About The Product Like Size Color And
              Care.'
            </p>
          </blockquote> -->
            <NuxtLink to="/equipments/1">
              <button type="button" class="btn btn-outline-dark">
                View Details
              </button>
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
