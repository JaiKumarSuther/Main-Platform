<script setup>
import SelectDetails from "../components/UI/SelectDetails.vue";
import Map from "../components/UI/Map.vue";
import MobileMap from "../components/UI/MobileMap.vue";
import OperatorCard from "../components/UI/OperatorCard.vue";
import OperatorCardMobile from "../components/UI/OperatorCardMobile.vue";
import OperatingHours from "../components/UI/OperatingHours.vue";
import OperatingHoursMobile from "../components/UI/OperatingHoursMobile.vue";
import ChatWithOperator from "../components/UI/ChatWithOperator.vue";
import ChatWithOperatorMobile from "../components/UI/ChatWithOperatorMobile.vue";
import ProtectedBookingCard from "../components/UI/ProtectedBookingCard.vue";
import ProtectedBookingCardMobile from "../components/UI/ProtectedBookingCardMobile.vue";
import SidebarMobile from "../components/UI/SidebarMobile.vue";
import ListingDetails from "../components/UI/ListingDetails.vue";
import Header from "../components/UI/Header.vue";
import Details from "../components/UI/Details.vue";
import Included from "../components/UI/Included.vue";
import MoreDetails from "../components/UI/MoreDetails.vue";
import FAQs from "../components/UI/FAQs.vue";
import ReviewCount from "../components/UI/ReviewCount.vue";
import FreeCancellation from "../components/UI/FreeCancellation.vue";

const bikeData = {
  title: "Fuego Tekken 250",
  price: "Rs 8,400",
  location: "Islamabad",
  mainImage: "/src/images/Bike.png",

  galleryImages: [
    "/src/images/avatar.png",
    "/src/images/avatar.png",
    "/src/images/avatar.png",
    "/src/images/avatar.png",
  ],
};
</script>

<template>
  <main>
    <SidebarMobile />
    <ListingDetails
      :title="bikeData.title"
      :price="bikeData.price"
      :location="bikeData.location"
      :mainImage="bikeData.mainImage"
      :galleryImages="bikeData.galleryImages"
    />

    <div class="listing-info-details">
      <div class="listing-info">
        <Header location="Islamabad" />

        <Details
          :items="[
            {
              label: 'Model',
              value: '2017',
              icon: '/src/images/vehicmode.svg',
            },
            { label: 'CCs', value: '250', icon: '/src/images/CC icon.svg' },
            {
              label: 'Transmission',
              value: 'Automatic',
              icon: '/src/images/Transmission icon.svg',
            },
            {
              label: 'Type',
              value: 'Adventure',
              icon: '/src/images/Vehicle type icon.svg',
            },
          ]"
        />

        <MobileMap
          mapSrc="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3326.2070127821403!2d73.0897425!3d33.522003000000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38dfed2e048746c1%3A0x244a446ba063d544!2sPakistan%20Bikers!5e0!3m2!1sen!2s!4v1745253279331!5m2!1sen!2s"
        />

        <OperatorCardMobile
          logo="/src/images/pakistanbikers.jpg"
          name="Pakistan Bikers"
          rating="4.5"
          reviewScore="4.2"
          reviewCount="15"
        />

        <OperatingHoursMobile
          name="Pakistan Bikers"
          hours="8AM - 9PM Monday to Sunday"
        />

        <ChatWithOperatorMobile name="Pakistan Bikers" />

        <ProtectedBookingCardMobile
          title="Your booking is safe"
          description="We will step in if any issues arise with your booking."
        />

        <Included
          :includedItems="['Helmet', 'Box', 'Side Bags', 'Spare Tire']"
          :notIncludedItems="['Insurance', 'Additional Services', 'Fuel']"
        />

        <MoreDetails
          :items="[
            {
              title: 'Important Information',
              text: 'A valid CNIC or passport and license is mandatory.',
            },
            {
              title: 'Payment Policy',
              text: 'Full payment required before vehicle pickup.',
            },
          ]"
        />

        <FAQs
          :items="[
            {
              question: 'What documents do I need to rent a bike?',
              answer:
                'Valid CNIC or passport and a driving license are required.',
            },
            {
              question: 'Is fuel included in the rental price?',
              answer: 'No, fuel charges are borne by the customer.',
            },
            {
              question: 'Can I take the bike off-road?',
              answer: 'Yes, but prior approval from the operator is needed.',
            },
            {
              question: 'What happens in case of breakdown?',
              answer:
                'Call our 24/7 support; we will dispatch help immediately.',
            },
          ]"
        />

        <ReviewCount
          :overallRating="4.0"
          :totalReviews="21"
          :ratingBreakdown="[
            { rating: 5, count: 16 },
            { rating: 4, count: 5 },
            { rating: 3, count: 0 },
            { rating: 2, count: 0 },
            { rating: 1, count: 0 },
          ]"
          :reviews="[
            {
              name: 'Wamiq Ahmed',
              date: '27 July 2025',
              rating: 5,
              comment: 'Had a great experience...',
              images: [
                '/src/images/thhunzagalleryimg4.jpg',
                '/src/images/hunzagalleryimg1.jpg',
                '/src/images/hunzagalleryimg2.jpg',
                '/src/images/hunzagalleryimg3.jpg',
                '/src/images/hunzagalleryimg5.jpg',
              ],
            },
            {
              name: 'Faisal',
              date: '8 Jun 2025',
              rating: 5,
              comment:
                'Book with them, they\'re probably the best in Pakistan.',
              reply: {
                name: 'Eventica Travels',
                message: 'Thank you so much for the kind words...',
              },
            },
          ]"
          :icons="{
            filledStar: '/src/images/Review icon.svg',
            emptyStar: '/src/images/boder star.svg',
            avatar: '/src/images/avatar.png',
          }"
        />
      </div>
      <div class="sidebar">
        <SelectDetails
          :withDriverLabel="'With Driver'"
          :withoutDriverLabel="'Without Driver'"
          :selectedDate="'7 July 2025'"
          :pickupTime="'13:00'"
          :dropoffTime="'17:00'"
          :addOns="[
            { label: 'Passenger Helmet', price: 'Rs 1,200' },
            { label: 'Top Box', price: 'Rs 1,200' },
          ]"
          :rentalSummary="{
            days: 8,
            total: 'Rs 86,400',
            breakdown: [
              { label: '8 Days Rental', amount: 'Rs 67,200' },
              { label: 'Passenger Helmet', amount: 'Rs 9600' },
              { label: 'Top Box', amount: 'Rs 9600' },
            ],
          }"
          cancellationNote="Free cancellation until"
          cancellationDeadline="6th May, 23:59 PM"
        />

        <Map
          map-url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3326.2070127821403!2d73.0897425!3d33.522003000000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38dfed2e048746c1%3A0x244a446ba063d544!2sPakistan%20Bikers!5e0!3m2!1sen!2s!4v1745253279331!5m2!1sen!2s"
        />

        <OperatorCard
          image="/src/images/pakistanbikers.jpg"
          name="Pakistan Bikers"
          rating="4.5"
          reviewScore="4.2"
          :totalReviews="15"
        />

        <OperatingHours hours="8AM - 9PM Monday to Sunday" />

        <ChatWithOperator
          icon="/src/images/chat after booking.svg"
          title="Chat with XYZ Rentals"
          message="You can chat with our support team directly after confirming your booking."
        />

        <ProtectedBookingCard
          icon="/src/images/protec.svg"
          title="Secure Payment"
          message="Your transaction is secured and fully refundable under our protection policy."
        />
      </div>
    </div>

    <FreeCancellation />
  </main>
</template>
