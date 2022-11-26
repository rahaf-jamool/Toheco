<script>
import MainSlider from './MainSlider';
import IconsCategory from './IconsCategory';
import ResentArrivals from './ResentArrivals';
import ContactAbout from './ContactAbout';
import PhotoGallery from './PhotoGallery';
import AboutUs from './AboutUs';

export default {
  name: "home",
  components: {
    MainSlider,
    IconsCategory,
    ResentArrivals,
    AboutUs,
    ContactAbout,
    PhotoGallery
  }
};
</script>

<template>
<main>
  <MainSlider/>
  <IconsCategory/>
  <ResentArrivals/>
  <AboutUs/>
  <ContactAbout/>
  <PhotoGallery/>
</main>
</template>

<style scoped>
</style>
