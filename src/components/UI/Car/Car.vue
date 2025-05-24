<script setup>
import SelectDetails from '../SelectDetails.vue';
import Map from '../Map.vue';
import MobileMap from '../MobileMap.vue';
import OperatorCard from '../OperatorCard.vue';
import OperatorCardMobile from '../OperatorCardMobile.vue';
import OperatingHours from '../OperatingHours.vue';
import OperatingHoursMobile from '../OperatingHoursMobile.vue';
import ChatWithOperator from '../ChatWithOperator.vue';
import ChatWithOperatorMobile from '../ChatWithOperatorMobile.vue';
import ProtectedBookingCard from '../ProtectedBookingCard.vue';
import ProtectedBookingCardMobile from '../ProtectedBookingCardMobile.vue';
import SidebarMobile from '../SidebarMobile.vue';
import ListingDetails from '../ListingDetails.vue';
import Header from '../Header.vue';
import Details from '../Details.vue';
import Included from '../Included.vue';
import MoreDetails from '../MoreDetails.vue';
import FAQs from '../FAQs.vue';
import ReviewCount from '../ReviewCount.vue';
import FreeCancellation from '../FreeCancellation.vue';

const carData = {
  title: 'Honda Civic 2021',
  price: 'Rs 4,900',
  location: 'Islamabad',
  mainImage: '/src/images/Car.png',
  galleryImages: [
    '/src/images/avatar.png',
    '/src/images/avatar.png',
    '/src/images/avatar.png',
    '/src/images/avatar.png',
  ]
};
</script>

<template>
  <main>
    <SidebarMobile />
    <ListingDetails
      :title="carData.title"
      :price="carData.price"
      :location="carData.location"
      :mainImage="carData.mainImage"
      :galleryImages="carData.galleryImages"
    />

    <div class="listing-info-details">
      <div class="listing-info">
        <Header location="Islamabad" />

        <Details
          :items="[
            { label: 'Model', value: '2017', icon: '/src/images/vehicmode.svg' },
            { label: 'CCs', value: '250', icon: '/src/images/CC icon.svg' },
            { label: 'Transmission', value: 'Automatic', icon: '/src/images/Transmission icon.svg' },
            { label: 'Type', value: 'Sedan', icon: '/src/images/Vehicle type icon.svg' },
          ]"
        />

        <MobileMap
          mapSrc="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
        />

        <OperatorCardMobile
          logo="/src/images/fast track.jpg"
          name="Fast Track Car Rental"
          rating="4.5"
          reviewScore="4.2"
          reviewCount="15"
        />

        <OperatingHoursMobile
          name="Fast Track Car Rental"
          hours="8AM - 9PM Monday to Sunday"
        />

        <ChatWithOperatorMobile name="Fast Track Car Rental" />

        <ProtectedBookingCardMobile
          title="Protected booking"
          description="In case of issues, we've got your back. We'll intervene and protect your money."
        />

        <Included
          :includedItems="['Car', 'Driver', 'Pickup', 'Unlimited Mileage', 'Spare Tire']"
          :notIncludedItems="['Insurance', 'Additional Services', 'Fuel']"
        />

        <MoreDetails
          :items="[
            { title: 'Important Information', text: 'A valid CNIC or passport and license is mandatory.' }
          ]"
        />

        <FAQs
          :items="[
            {
              question: 'What if the car breaks down during my trip?',
              answer: 'Call our 24/7 support. Roadside assistance or a replacement will be arranged.'
            },
            {
              question: 'What documents do I need to rent a car?',
              answer: 'You need CNIC/passport and a valid driving license.'
            },
            {
              question: 'Is there a security deposit required, and how much is it?',
              answer: 'Yes. Details vary by vehicle type and rental duration.'
            },
            {
              question: 'Can I pick up the car from one location and return it to another?',
              answer: 'Yes, with prior coordination.'
            }
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
                '/src/images/hunzagalleryimg5.jpg'
              ]
            },
            {
              name: 'Faisal',
              date: '8 Jun 2025',
              rating: 5,
              comment: 'Book with them, they\'re probably the best in Pakistan.',
              reply: {
                name: 'Eventica Travels',
                message: 'Thank you so much for the kind words...'
              }
            }
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
          :withDriverLabel="'With Driver'"
          :withoutDriverLabel="'Without Driver'"
          :selectedDate="'7 July 2025'"
          :pickupTime="'13:00'"
          :dropoffTime="'17:00'"
          :addOns="[
            { label: 'Passenger Helmet', price: 'Rs 1,200' },
            { label: 'Top Box', price: 'Rs 1,200' }
          ]"
          :rentalSummary="{
            days: 8,
            total: 'Rs 86,400',
            breakdown: [
              { label: '8 Days Rental', amount: 'Rs 67,200' },
              { label: 'Passenger Helmet', amount: 'Rs 9600' },
              { label: 'Top Box', amount: 'Rs 9600' }
            ]
          }"
          cancellationNote="Free cancellation until"
          cancellationDeadline="6th May, 23:59 PM"
        />

        <Map
          map-url="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
        />

        <OperatorCard
          image="/src/images/fast track.jpg"
          name="Fast Track Car Rental"
          rating="4.5"
          reviewScore="4.2"
          :totalReviews="15"
        />

        <OperatingHours hours="8AM - 9PM Monday to Sunday" />

        <ChatWithOperator
          icon="/src/images/chat after booking.svg"
          title="Chat with Fast Track Car Rental"
          message="You'll get access to direct chat after booking. Ask anything, confirm plans, stay connected."
        />

        <ProtectedBookingCard
          icon="/src/images/protec.svg"
          title="Protected booking"
          message="We’ll intervene if anything goes wrong with your booking."
        />
      </div>
    </div>

    <FreeCancellation />
  </main>
</template>
