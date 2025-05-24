<script setup>
import SidebarMobile from "../SidebarMobile.vue";
import ListingDetails from "../ListingDetails.vue";
import Header from "../Header.vue";
import Details from "../Details.vue";
import MobileMap from "../MobileMap.vue";
import OperatorCardMobile from "../OperatorCardMobile.vue";
import ChatWithOperatorMobile from "../ChatWithOperatorMobile.vue";
import ProtectedBookingCardMobile from "../ProtectedBookingCardMobile.vue";
import SummaryBox from "../SummaryBox.vue";
import Highlights from "../Highlights.vue";
import Included from "../Included.vue";
import Itinerary from "../Itinerary.vue";
import MoreDetails from "../MoreDetails.vue";
import FAQs from "../FAQs.vue";
import ReviewCount from "../ReviewCount.vue";
import SelectDetails from "../SelectDetails.vue";
import Map from "../Map.vue";
import OperatorCard from "../OperatorCard.vue";

const trekData = {
  title: "14 Day K2 Base Camp Trekking Expedition",
  price: "$1800",
  location: "From Islamabad",
  mainImage: "/src/images/17940.jpg",
  galleryImages: [
    "/src/images/avatar.png",
    "/src/images/avatar.png",
    "/src/images/avatar.png",
    "/src/images/avatar.png"
  ]
};
</script>

<template>
  <main>
    <SidebarMobile />
    <ListingDetails
      :title="trekData.title"
      :price="trekData.price"
      :location="trekData.location"
      :mainImage="trekData.mainImage"
      :galleryImages="trekData.galleryImages"
    />

    <div class="listing-info-details">
      <div class="listing-info">
        <Header :location="trekData.location" />

        <Details
          :items="[
            { label: 'Duration', value: '9 days', icon: '/src/images/Duration icon.svg' },
            { label: 'Trek Type', value: 'Group Trek', icon: '/src/images/Tour type icon.svg' },
            { label: 'For Ages', value: '3 to 48 years old', icon: '/src/images/For ages icon.svg' },
            { label: 'Languages', value: 'English, Urdu', icon: '/src/images/Language icon.svg' },
            { label: 'Difficulty', value: 'Hard', icon: '/src/images/Difficulty icon.svg' }
          ]"
        />

        <MobileMap
          mapSrc="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
        />

        <OperatorCardMobile
          logo="/src/images/Asset 1.png"
          name="Askoli Adventure Treks & Tours"
          rating="4.5"
          reviewScore="4.2"
          reviewCount="15"
        />

        <ChatWithOperatorMobile name="Askoli Adventure Treks & Tours" />

        <ProtectedBookingCardMobile
          title="Protected booking"
          description="In case of issues, we've got your back. We'll intervene and protect your money."
        />

        <SummaryBox
          title="Overview"
          text="Embark on an unforgettable 7-day adventure through the majestic valleys of northern Pakistan, taking you from the vibrant capital of Islamabad to the serene landscapes of Naran, Hunza, and Skardu. This carefully curated tour offers a perfect blend of cultural experiences, breathtaking natural beauty, and thrilling exploration."
        />

        <Highlights
          :items="[
            '7-day itinerary covering Islamabad, Naran, Hunza, and Skardu.',
            'Visit to Lake Saif ul Malook and Sheosar Lake.',
            'Experience the culture and history of Baltit Fort and Shigar Fort.',
            'Scenic drives through Kaghan Valley and Karakoram Highway.',
            'Accommodation in hand-picked, comfortable hotels.',
            'Fully guided tours, ensuring a smooth and enriching experience.'
          ]"
        />

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
            { question: 'Do you offer pickup from hotel?', answer: 'Yes, we will contact you to confirm details.' },
            { question: 'What meals will be provided during the tour?', answer: 'Breakfast, dinner and snacks included.' },
            { question: 'Which hotels will we stay in?', answer: 'Clean and comfortable 3-star accommodations.' },
            { question: 'Do you help with the supporting documents?', answer: 'Yes, we assist with necessary travel documentation.' }
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
            { rating: 1, count: 0 }
          ]"
          :reviews="[
            { name: 'Wamiq Ahmed', date: '27 July 2025', rating: 5, comment: 'Best value for money. Recommended.' },
            { name: 'Faisal', date: '8 Jun 2025', rating: 5, comment: 'Probably the best in Pakistan.' },
            { name: 'Michael', date: '24 May 2025', rating: 5, comment: 'Well crafted and satisfying trip.' }
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
            days: 14,
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

        <Map
          map-url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
        />

        <OperatorCard
          image="/src/images/Eventica-Color-Logo_Final-1536x961.png"
          name="Askoli Adventure Treks & Tours"
          rating="4.5"
          reviewScore="4.2"
          :totalReviews="15"
        />
      </div>
    </div>
  </main>
</template>
