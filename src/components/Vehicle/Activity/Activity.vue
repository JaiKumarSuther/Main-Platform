<script setup>
import SidebarMobile from "../SidebarMobile.vue";
import ListingDetails from "../ListingDetails.vue";
import Header from "../Header.vue";
import Details from "../Details.vue";
import MobileMap from "../MobileMap.vue";
import OperatorCardMobile from "../OperatorCardMobile.vue";
import OperatingHoursMobile from "../OperatingHoursMobile.vue";
import ChatWithOperatorMobile from "../ChatWithOperatorMobile.vue";
import ProtectedBookingCardMobile from "../ProtectedBookingCardMobile.vue";
import Included from "../Included.vue";
import MoreDetails from "../MoreDetails.vue";
import FAQs from "../FAQs.vue";
import ReviewCount from "../ReviewCount.vue";
import SummaryBox from "../SummaryBox.vue";
import Itinerary from "../Itinerary.vue";
import SelectDetails from "../SelectDetails.vue";
import Map from "../Map.vue";
import OperatorCard from "../OperatorCard.vue";
import OperatingHours from "../OperatingHours.vue";
import ChatWithOperator from "../ChatWithOperator.vue";
import ProtectedBookingCard from "../ProtectedBookingCard.vue";
import FreeCancellation from "../FreeCancellation.vue";

const activityData = {
  title: "Soar Above the Majestic Hunza valley",
  price: "Rs 12,000",
  location: "Hunza",
  mainImage: "/src/images/Activity.png",
  priceSuffix: "/person",
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
      :title="activityData.title"
      :price="activityData.price"
      :location="activityData.location"
      :mainImage="activityData.mainImage"
      :galleryImages="activityData.galleryImages"
      :priceSuffix="activityData.priceSuffix"
    />

    <div class="listing-info-details">
      <div class="listing-info">
        <Header :location="activityData.location" />

        <Details
          :items="[
            {
              label: 'Duration',
              value: '30 minutes',
              icon: '/src/images/Duration icon.svg',
            },
            {
              label: 'Activity Type',
              value: 'Paragliding',
              icon: '/src/images/Tour type icon.svg',
            },
            {
              label: 'For Ages',
              value: '14 to 50 years old',
              icon: '/src/images/For ages icon.svg',
            },
            {
              label: 'Languages',
              value: 'English, Urdu',
              icon: '/src/images/Language icon.svg',
            },
            {
              label: 'Min. people',
              value: '1',
              icon: '/src/images/Min people icon.svg',
            },
            {
              label: 'Difficulty',
              value: 'Moderate',
              icon: '/src/images/Difficulty icon.svg',
            },
          ]"
        />
        <MobileMap
          mapSrc="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3326.2070127821403!2d73.0897425!3d33.522003000000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38dfed2e048746c1%3A0x244a446ba063d544!2sPakistan%20Bikers!5e0!3m2!1sen!2s!4v1745253279331!5m2!1sen!2s"
        />
        <OperatorCardMobile
          logo="/src/images/Hunza paragliding club.png"
          name="Hunza Paragliding Club"
          rating="4.5"
          reviewScore="4.2"
          reviewCount="15"
        />

        <OperatingHoursMobile
          name="Hunza Paragliding Club"
          hours="8AM - 9PM Monday to Sunday"
        />

        <ChatWithOperatorMobile name="Hunza Paragliding Club" />

        <ProtectedBookingCardMobile
          title="Protected booking"
          description="In case of issues, we've got your back. We'll intervene and protect your money."
        />

        <SummaryBox
          title="Overview"
          text="Experience the thrill of flying over Hunza Valley’s breathtaking landscapes..."
        />

        <Included
          :includedItems="[
            'Professional tandem paragliding pilot',
            'Safety gear (helmet, harness)',
            'Gopro video footage of your flight',
            'Transportation to the takeoff site',
            'Complimentary refreshments',
          ]"
          :notIncludedItems="[
            'Insurance',
            'Additional Services',
            'Personal Expenses',
          ]"
        />

        <Itinerary
          title="Itinerary"
          :items="[
            {
              label: 'First 10 minutes',
              content: 'Meet at Launch Point (Eagle’s Nest)',
              details: 'General safety briefing & gear check',
            },
            {
              label: 'Next',
              content: 'Tandem Flight begins',
              details: 'Scenic glide over the valley',
            },
          ]"
        />

        <MoreDetails
          :items="[
            {
              title: 'Important Information',
              text: 'Wear comfortable clothing and bring ID.',
            },
            {
              title: 'Not Suitable For',
              text: 'People with heart conditions or pregnancy.',
            },
            {
              title: 'What to bring',
              text: 'Comfortable clothes, camera, sunscreen.',
            },
          ]"
        />

        <FAQs
          :items="[
            {
              question: 'Is paragliding safe for beginners?',
              answer:
                'Yes! Certified pilots ensure full safety with a pre-flight briefing.',
            },
            {
              question: 'What should I wear?',
              answer:
                'Comfortable sportswear and sturdy shoes are recommended.',
            },
            {
              question: 'Do I need experience?',
              answer:
                'No prior experience required. Tandem flight is beginner-friendly.',
            },
            {
              question: 'What if the weather is bad?',
              answer:
                'Flights may be rescheduled or refunded due to safety concerns.',
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
              ],
            },
            {
              name: 'Faisal',
              date: '8 Jun 2025',
              rating: 5,
              comment:
                'Book with them, they\'re probably the best in Pakistan.',
              reply: {
                name: 'Hunza Paragliding Club',
                message: 'We\'re thrilled to hear your feedback!',
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
          :showPeopleSelector="true"
          :selectedDate="'26 August 2025'"
          :addOns="[
            { label: 'Extended Flight', price: 'Rs 3,000' },
            { label: '4K GoPro Footage', price: 'Rs 4,200' },
          ]"
          :rentalSummary="{
            days: 1,
            total: 'Rs 543,000',
            breakdown: [
              { label: '2x Adults', amount: 'Rs 540,000' },
              { label: '1x Infant', amount: 'Rs 0' },
              { label: 'Add On 1', amount: 'Rs 3,000' },
            ],
          }"
          cancellationNote="Free cancellation until"
          cancellationDeadline="6th May"
        />

        <Map
          map-url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3326.2070127821403!2d73.0897425!3d33.522003000000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38dfed2e048746c1%3A0x244a446ba063d544!2sPakistan%20Bikers!5e0!3m2!1sen!2s!4v1745253279331!5m2!1sen!2s"
        />

        <OperatorCard
          image="/src/images/Hunza paragliding club.png"
          name="Hunza Paragliding Club"
          rating="4.5"
          reviewScore="4.2"
          :totalReviews="15"
        />

        <OperatingHours hours="8AM - 9PM Monday to Sunday" />

        <ChatWithOperator
          icon="/src/images/chat after booking.svg"
          title="Chat with Hunza Paragliding Club"
          message="Ask anything, confirm plans, stay connected."
        />

        <ProtectedBookingCard
          icon="/src/images/protec.svg"
          title="Protected booking"
          message="In case of issues, we\'ll intervene and protect your money."
        />
      </div>
    </div>

    <FreeCancellation />
  </main>
</template>
