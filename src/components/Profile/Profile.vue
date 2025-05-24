<script setup>
import Sidebar from "./Sidebar.vue";
import Messages from "./Messages.vue";
import Account from './Account.vue';
import Bookings from './Bookings.vue'
import Saved from './Saved.vue'
import SupportRequest from './SupportRequest.vue'
import CreateSupportRequest from './CreateSupportRequest.vue'
import OpenSupportRequest from './OpenSupportRequest.vue'
import CloseSupportRequest from './CloseSupportRequest.vue'
import Refunds from './Refunds.vue'
</script>

<template>
  <div class="profile-container">
    <h1 class="title">My Profile</h1>
    <div class="profile-wrapper">
        <Sidebar/>
        <CloseSupportRequest/>
    </div>
  </div>
</template>
