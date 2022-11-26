<template>
<header class="main-header">

        <div class="logo">
            <a href=""><img src="../../public/assets/images/icon/logo-header.png" alt=""></a>
        </div>

        <input type="checkbox" class="menu-btn" id="menu-btn">
        <label for="menu-btn" class="menu-icon">
            <span class="menu-icon_line"></span>
        </label>

        <ul class="nav-links">

            <li class="nav-link"><NuxtLink to="/">Home</NuxtLink></li>
            <li class="nav-link"><NuxtLink to="/about">About Us</NuxtLink></li>
            <li class="nav-link"><NuxtLink to="/equipments">Equipments</NuxtLink></li>
            <li class="nav-link"><a href="#">Construction & Mining Equipment</a></li>
            <li class="nav-link"><a href="#">Lifting & Material Handling</a></li>
            <li class="nav-link"><a href="#">Miscellaneous & Parts</a></li>
            <li class="nav-link"><a href="#">Inquiry</a></li>
            <li class="nav-link">
              <a href="#" class="drop dropdown-toggle">Media Center</a>
              <div class="dropdown-menu p-0 m-0">
                <a class="dropdown-item" href="">News</a>
                <a class="dropdown-item" href="">Photo Gallery</a>
                <a class="dropdown-item" href="">Videos</a>
              </div>
            </li>
            <li class="nav-link"><NuxtLink to="/contact">Contact Us</NuxtLink></li>
        </ul>
        <div class="contact">
            <!-- <div class="phone"><img src="../../public/assets/images/icon/whats.png"/> +9710000000</div> -->
            <div class="search"><img src="../../public/assets/images/Asset 13ldpi.png"/></div>
            <div class="lang">
                <img src="../../public/assets/images/icon/Asset 3ldpi.png" alt="">
            </div>
        </div>

</header>
</template>

<script>

export default {
    name: "Header"
};
</script>

<style lang="scss" scoped>
</style>
