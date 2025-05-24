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
import SummaryBox from "../SummaryBox.vue";
import Included from "../Included.vue";
import Itinerary from "../Itinerary.vue";
import MoreDetails from "../MoreDetails.vue";
import FAQs from "../FAQs.vue";
import ReviewCount from "../ReviewCount.vue";
import SelectDetails from "../SelectDetails.vue";
import Map from "../Map.vue";
import OperatorCard from "../OperatorCard.vue";
import OperatingHours from "../OperatingHours.vue";
import ChatWithOperator from "../ChatWithOperator.vue";
import ProtectedBookingCard from "../ProtectedBookingCard.vue";
import FreeCancellation from "../FreeCancellation.vue";
import Highlights from "../Highlights.vue";

const groupTourData = {
  title: "9 Day Hunza Valley: A Cultural & Scenic Odyssey",
  price: "$1200",
  priceSuffix: "",
  location: "From Islamabad",
  mainImage: "/src/images/hunza tour.png",
  galleryImages: [
    "/src/images/2211.jpg",
    "/src/images/45497.jpg",
    "/src/images/17940.jpg",
    "/src/images/26240.jpg",
  ],
};
</script>

<template>
  <main>
    <SidebarMobile />
    <ListingDetails
      :title="groupTourData.title"
      :price="groupTourData.price"
      :location="groupTourData.location"
      :mainImage="groupTourData.mainImage"
      :galleryImages="groupTourData.galleryImages"
      :priceSuffix="groupTourData.priceSuffix"
    />

    <div class="listing-info-details">
      <div class="listing-info">
        <Header :location="groupTourData.location" />

        <Details
          :items="[
            { label: 'Duration', value: '9 days', icon: '/src/images/Duration icon.svg' },
            { label: 'Type', value: 'Group Tour', icon: '/src/images/Tour type icon.svg' },
            { label: 'For Ages', value: '3 to 48 years old', icon: '/src/images/For ages icon.svg' },
            { label: 'Languages', value: 'English, Urdu', icon: '/src/images/Language icon.svg' },
            { label: 'Theme', value: 'Cultural Tour', icon: '/src/images/Tour theme and experience type icon.svg' },
          ]"
        />
        <MobileMap
          mapSrc="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
        />

        <OperatorCardMobile
          logo="/src/images/Eventica.png"
          name="Eventica Travels"
          rating="4.5"
          reviewScore="4.2"
          reviewCount="15"
        />

        <OperatingHoursMobile name="Eventica Travels" hours="8AM - 9PM Monday to Sunday" />

        <ChatWithOperatorMobile name="Eventica Travels" />

        <ProtectedBookingCardMobile
          title="Protected booking"
          description="In case of issues, we've got your back. We'll intervene and protect your money."
        />

        <SummaryBox
          title="Summary"
          text="Embark on an unforgettable 7-day adventure through the majestic valleys of northern Pakistan taking you from the vibrant capital of Islamabad to the serene landscapes of Naran, Hunza, and Skardu. This carefully curated tour offers a perfect blend of cultural experiences, breathtaking natural beauty, and thrilling exploration. With expertly guided visits to iconic sites, including Naran’s Lake Saif ul Malook, the charming Baltit Fort in Hunza, and the serene Sheosar Lake in Skardu, this tour promises an unforgettable exploration of Pakistan’s most picturesque landscapes."
        />
        <Highlights/>

        <Included
          :includedItems="[
            'Guide',
            'Transportation (Bus, Jeep)',
            'Meals (Breakfast, Evening Snacks, Dinner)',
            'National Parks Entrance Fees',
            'Accommodations (3 Star)'
          ]"
          :notIncludedItems="['Insurance', 'Additional Services', 'Drinks']"
        />

        <Itinerary
          title="Itinerary"
          :items="[
            { label: 'Day 1', content: 'Islamabad to Naran', details: 'Scenic drive with river rafting in Naran.' },
            { label: 'Day 2', content: 'Naran to Babusar Top & Chilas' },
            { label: 'Day 3', content: 'Fairy Meadows & Nanga Parbat' },
            { label: 'Day 4', content: 'Hunza & Attabad Lake' },
            { label: 'Day 5', content: 'Skardu Exploration' },
            { label: 'Day 6', content: 'Return to Naran' },
            { label: 'Day 7', content: 'Drive back to Islamabad' }
          ]"
        />

        <MoreDetails
          :items="[
            { title: 'Important Information', text: 'Carry CNIC/Passport and weather-appropriate clothing.' },
            { title: 'Not Suitable For', text: 'Wheelchair users and people with major health issues.' }
          ]"
        />

        <FAQs
          :items="[
            { question: 'Do you offer hotel pickup?', answer: 'Yes, you can select the pickup add-on at booking.' },
            { question: 'What meals are included?', answer: 'Breakfast, evening snacks, and dinner are covered.' },
            { question: 'Which hotels will we stay in?', answer: 'Comfortable 3-star hotels are arranged.' },
            { question: 'Do you help with visa/support documents?', answer: 'Yes, we provide supporting travel documents upon request.' }
          ]"
        />

        <ReviewCount
          :overallRating="3.5"
          :totalReviews="21"
          :ratingBreakdown="[
            { rating: 5, count: 16 },
            { rating: 4, count: 5 },
            { rating: 3, count: 0 },
            { rating: 2, count: 0 },
            { rating: 1, count: 0 }
          ]"
          :reviews="[
            { name: 'Wamiq Ahmed', date: '27 July 2025', rating: 5, comment: 'Had a great experience, smooth trip.' },
            { name: 'Faisal', date: '8 Jun 2025', rating: 5, comment: 'Probably the best tour operator in Pakistan.' },
            { name: 'Michael', date: '24 May 2025', rating: 5, comment: 'Well crafted tour with diverse experiences.' }
          ]"
          :icons="{
            filledStar: '/src/images/Review icon.svg',
            emptyStar: '/src/images/boder star.svg',
            avatar: '/src/images/avatar.png'
          }"
        />
      </div>

      <div class="sidebar">
        <SelectDetails
          :showPeopleSelector="true"
          :selectedDate="'26 August 2025'"
          :addOns="[
            { label: 'Add On 1', price: 'Rs 3,000' },
            { label: 'Add On 2', price: 'Rs 4,200' }
          ]"
          :rentalSummary="{
            days: 9,
            total: 'Rs 543,000',
            breakdown: [
              { label: '2x Adults', amount: 'Rs 540,000' },
              { label: '1x Infant', amount: 'Rs 0' },
              { label: 'Add On 1', amount: 'Rs 3,000' }
            ]
          }"
          cancellationNote="Free cancellation until"
          cancellationDeadline="6th May"
        />

        <Map map-url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s" />

        <OperatorCard
          image="/src/images/Eventica.png"
          name="Eventica Travels"
          rating="4.5"
          reviewScore="4.2"
          :totalReviews="15"
        />

        <OperatingHours hours="8AM - 9PM Monday to Sunday" />

        <ChatWithOperator
          icon="/src/images/chat after booking.svg"
          title="Chat with Eventica Travels"
          message="Ask anything, confirm plans, stay connected."
        />

        <ProtectedBookingCard
          icon="/src/images/protec.svg"
          title="Protected booking"
          message="In case of issues, we'll intervene and protect your money."
        />
      </div>
    </div>

    <FreeCancellation />
  </main>
</template>
