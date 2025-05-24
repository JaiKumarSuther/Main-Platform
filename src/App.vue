<script setup>
  import Footer from "./components/Footer.vue";
  import Header from "./components/Header.vue";
  import Hotel from "./components/Hotel.vue";
  import Trek from "./components/Trek.vue";
  import Activity from "./components/Activity.vue";
  import Search from "./components/Search.vue";
  import Bike from "./components/Bike.vue";
  import BookingConfirm from "./components/BookingConfirm.vue";
  import Car from "./components/Car.vue";
  import SmartSearch from "./components/SmartSearch.vue";
  import SelectDate from "./components/UI/SelectDate.vue";
  import ConfirmRoom from "./components/ConfirmRoom.vue";
  import Checkout from "./components/Checkout.vue";
  import FilterMobile from "./components/FilterMobile.vue";
  import GuidedExperience from "./components/GuidedExperience.vue";
  import PrivateTour from "./components/PrivateTour.vue";
  import GroupTour from "./components/GroupTour.vue";
  import TourGuideProfile from "./components/TourGuideProfile.vue";
  import Profile from "./components/Profile/Profile.vue";
  import Auth from "./components/auth/Auth.vue";
</script>

<template>
  <main>
    <Header />
      <SmartSearch/>
    <Footer />
  </main>
</template>
