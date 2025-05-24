<script setup>
defineProps({
  title: String,
  price: String,
  location: String,
  mainImage: String,
  galleryImages: Array
})
</script>

<template>
  <div class="listing-details">
    <div class="listing-header">
      <section class="listing-header-details">
        <h1>{{ title }}</h1>
        <p>From <span class="price">{{ price }}</span><small>/day</small></p>
      </section>
      <span class="location-mobile">
        <img src="/src/images/Location icon.svg" alt="" />
        {{ location }}
      </span>
      <section class="listing-header-icons">
        <div class="icon">
          <img src="/src/images/Save Icon (listing page & Header).svg" alt="" />
        </div>
        <div class="icon">
          <img src="/src/images/Share icon.svg" alt="" />
        </div>
      </section>
    </div>

    <section class="gallery">
      <div class="main-image">
        <img :src="mainImage" alt="Main Tour Image" />
      </div>
      <div class="side-images">
        <img v-for="(img, index) in galleryImages" :key="index" :src="img" :alt="'Image ' + (index + 1)" />
      </div>
    </section>
  </div>
</template>
