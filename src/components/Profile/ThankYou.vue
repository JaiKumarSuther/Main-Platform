<template>
  <main>
    <div class="profile-container">
      <h1 class="title">My Profile</h1>
      <div class="profile-wrapper">
        <aside class="sidebar">
          <ul>
            <li>
              <span class="icon"
                ><img src="/src/images/my account icon.svg" alt=""
              /></span>
              My account
            </li>
            <li class="active">
              <span class="icon"
                ><img src="/src/images/My bookings icon.svg" alt=""
              /></span>
              My bookings
            </li>
            <li>
              <span class="icon"
                ><img src="/src/images/messages icon.svg" alt=""
              /></span>
              Messages <span class="badge">2</span>
            </li>
            <li>
              <span class="icon"
                ><img
                  src="/src/images/Save Icon (listing page & Header).svg"
                  alt=""
              /></span>
              My saved
            </li>
            <li>
              <span class="icon"
                ><img src="/src/images/support icon.svg" alt=""
              /></span>
              My support requests
            </li>
          </ul>
        </aside>

        <div class="mybooking-container">
          <h2>My Bookings</h2>

          <div class="filter-bar">
            <div class="tabs">
              <button class="tab active">upcoming</button>
              <button class="tab">completed</button>
            </div>
            <button class="sort-btn">
              <span class="icon"
                ><img src="/src/images/sort by icon.svg" alt=""
              /></span>
              sort by
            </button>
          </div>

          <div class="booking-card">
            <div class="details">
              <div class="label tour">Tour</div>
              <div class="header">
                <span class="name"
                  >14 Day Full Board Expedition to the K2 Base Camp</span
                >
              </div>
              <div class="info">
                <span><strong>Date</strong> 25 Sep 2025</span>
                <span><strong>Amount</strong> 434,000</span>
                <span
                  ><strong>Status</strong>
                  <span class="status pending">Pending</span></span
                >
              </div>
            </div>
          </div>

          <div class="booking-card">
            <div class="details">
              <div class="label hotel">Hotel</div>
              <div class="header">
                <span class="name">Shangrila Resort</span>
              </div>
              <div class="info">
                <span><strong>Date</strong> 25 Sep 2025</span>
                <span><strong>Amount</strong> 23,800</span>
                <span
                  ><strong>Status</strong>
                  <span class="status completed">Completed</span></span
                >
              </div>
              <div class="leave-review">
                <p>
                  Help others by sharing your experience with
                  <span>Eventica Travels.</span>
                </p>
                <div class="stars">
                  <img src="/src/images/boder star.svg" alt="" />
                  <img src="/src/images/boder star.svg" alt="" />
                  <img src="/src/images/boder star.svg" alt="" />
                  <img src="/src/images/boder star.svg" alt="" />
                  <img src="/src/images/boder star.svg" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="review-popup" class="leave-review-popup-overlay">
      <div class="popup-content">
        <div class="review-header">
          <h2>Leave a review</h2>
          <svg
            class="close-btn"
            width="100"
            height="100"
            viewBox="0 0 100 100"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <!-- Circle outline -->
            <circle cx="50" cy="50" r="45" stroke="#5A6783" stroke-width="4" />

            <!-- Cross line 1 -->
            <line
              x1="35"
              y1="35"
              x2="65"
              y2="65"
              stroke="#5A6783"
              stroke-width="4"
              stroke-linecap="round"
            />

            <!-- Cross line 2 -->
            <line
              x1="65"
              y1="35"
              x2="35"
              y2="65"
              stroke="#5A6783"
              stroke-width="4"
              stroke-linecap="round"
            />
          </svg>
        </div>

        <div class="thankyou-message">
          <img
            src="/src/images/celebration-party-winter-svgrepo-com.svg"
            alt=""
          />
          <h3>Thank you for sharing your experience!</h3>
          <p>
            Your review helps fellow travelers and strengthens our global travel
            community.
          </p>
        </div>
      </div>
    </div>
  </main>
</template>
