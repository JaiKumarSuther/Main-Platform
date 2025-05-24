<template>
  <main>
    <div class="slider-mobile">
      <img class="slide" src="/src/images/northview.png" alt="Slide 1" />

      <!-- Arrows -->
      <div class="arrow left">&#10094;</div>
      <div class="arrow right">&#10095;</div>

      <!-- Dots -->
      <div class="dots">
        <div class="dot active"></div>
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
      </div>
    </div>
    <div class="listing-details">
      <div class="listing-header">
        <section class="listing-header-details listing-hotel-details">
          <div class="reviews">
            <img src="/src/images/Review icon.svg" alt="" />
            <span class="review-score">4.2</span>
            <span> 15 reviews</span>
          </div>
          <h1>North View Hotel</h1>
          <p>From <span class="price">PKR 4840</span></p>
        </section>
        <span class="location-mobile"
          ><img src="/src/images/Location icon.svg" alt="" /> Hunza, Gilgit
          Baltistan</span
        >
        <section class="listing-header-icons">
          <div class="icon">
            <img
              src="/src/images/Save Icon (listing page & Header).svg"
              alt=""
            />
          </div>
          <div class="icon">
            <img src="/src/images/Share icon.svg" alt="" />
          </div>
        </section>
      </div>
      <section class="gallery">
        <div class="main-image">
          <img src="/src/images/northview.png" alt="Main Tour Image" />
        </div>
        <div class="side-images">
          <img src="/src/images/avatar.png" alt="Image 1" />
          <img src="/src/images/avatar.png" alt="Image 2" />
          <img src="/src/images/avatar.png" alt="Image 3" />
          <img src="/src/images/avatar.png" alt="Image 4" />
        </div>
      </section>
    </div>
    <div class="hotel-info-details">
      <div class="hotel-info">
        <div class="header">
          <span class="location"
            ><img src="/src/images/Location icon.svg" alt="" /> Hunza</span
          >
        </div>
        <div class="hotel-header">
          <div class="amenities">
            <h2>Amenities <span> at the property</span></h2>
            <div class="amenities-list">
              <ul>
                <li>
                  <img src="/src/images/resturant icon.svg" alt="" />
                  <span>Restaurant</span>
                </li>
                <li>
                  <img src="/src/images/room service icon.svg" alt="" />
                  <span>Room service</span>
                </li>
                <li>
                  <img src="/src/images/Free parking icon.svg" alt="" />
                  <span>Free Parking</span>
                </li>
                <li>
                  <img src="/src/images/For ages icon.svg" alt="" />
                  <span>Family Friendly</span>
                </li>
              </ul>
              <ul>
                <li>
                  <img
                    src="/src/images/Places icon in mobile menu.svg"
                    alt=""
                  />
                  <span>Free Wi-fi</span>
                </li>
                <li>
                  <img src="/src/images/river view icon.svg" alt="" />
                  <span>River View</span>
                </li>
                <li>
                  <img src="/src/images/activity type icon.svg" alt="" />
                  <span>Lobby</span>
                </li>
                <li>
                  <a class="view-all" href="">view all amenities</a>
                </li>
              </ul>
            </div>
            <div class="check-in">
              <ul>
                <li>Check-in time: <span>12PM - Anytime</span></li>
                <li>Check-out time: <span>11AM</span></li>
              </ul>
            </div>
          </div>
          <div class="map">
            <iframe
              class="map"
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3214.7369973089967!2d74.6634475748222!3d36.318684172388274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38e8a08dbc639479%3A0xd65aede2afbf7944!2sTourist%20Cottage%20Hunza!5e0!3m2!1sen!2s!4v1744259797546!5m2!1sen!2s"
              width="600"
              height="450"
              style="border: 0"
              allowfullscreen=""
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
            ></iframe>
          </div>
        </div>

        <div class="select-room">
          <h2>Choose your room</h2>
          <div class="select-room-dropdown">
            <div class="left-dropdown">
              <div class="dropdown check">
                <img
                  src="/src/images/Date icon (select details).svg"
                  alt="People Icon"
                  class="icon"
                />
                <div class="dropdown-content">
                  <label>Dates</label>
                  <span>29 Aug - 2 Sep</span>
                </div>
              </div>
            </div>
            <div class="sort-container">
              <p>3 rooms available</p>
              <button id="sortBtn" class="border-button">
                <img src="/src/images/sort by icon.svg" alt="" />Sort by
              </button>
            </div>
          </div>
          <div class="room-list">
            <div class="room-card">
              <div class="image-slider">
                <img src="/src/images/room.png" alt="Deluxe Room" />
              </div>
              <div class="room-info">
                <h3>Deluxe Room</h3>
                <div class="info">
                  <div class="info-content">
                    <img
                      src="/src/images/People icon (select details).svg"
                      alt=""
                    />
                    <p>Sleeps 3</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Bed icon.svg" alt="" />
                    <p>1 Single Bed · 1 King Bed</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Room size icon.svg" alt="" />
                    <p>159 sq ft</p>
                  </div>
                </div>
                <p class="cancellation">
                  <img src="/src/images/Free cancellation icon.svg" alt="" />
                  Free cancellation until <span class="highlight">6th May</span>
                </p>
                <p class="price">PKR 4840 <span>(2 nights)</span></p>
                <p class="note">Breakfast included</p>
              </div>
            </div>
            <div class="room-card">
              <div class="image-slider">
                <img src="/src/images/avatar.png" alt="Deluxe Room" />
              </div>
              <div class="room-info">
                <h3>Deluxe Room</h3>
                <div class="info">
                  <div class="info-content">
                    <img
                      src="/src/images/People icon (select details).svg"
                      alt=""
                    />
                    <p>Sleeps 3</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Bed icon.svg" alt="" />
                    <p>1 Single Bed · 1 King Bed</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Room size icon.svg" alt="" />
                    <p>159 sq ft</p>
                  </div>
                </div>
                <p class="cancellation">
                  <img src="/src/images/Free cancellation icon.svg" alt="" />
                  Free cancellation until <span class="highlight">6th May</span>
                </p>
                <p class="price">PKR 4840 <span>(2 nights)</span></p>
                <p class="note">Breakfast included</p>
              </div>
            </div>
            <div class="room-card">
              <div class="image-slider">
                <img src="/src/images/avatar.png" alt="Deluxe Room" />
              </div>
              <div class="room-info">
                <h3>Deluxe Room</h3>
                <div class="info">
                  <div class="info-content">
                    <img
                      src="/src/images/People icon (select details).svg"
                      alt=""
                    />
                    <p>Sleeps 3</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Bed icon.svg" alt="" />
                    <p>1 Single Bed · 1 King Bed</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Room size icon.svg" alt="" />
                    <p>159 sq ft</p>
                  </div>
                </div>
                <p class="cancellation">
                  <img src="/src/images/Free cancellation icon.svg" alt="" />
                  Free cancellation until <span class="highlight">6th May</span>
                </p>
                <p class="price">PKR 4840 <span>(2 nights)</span></p>
                <p class="note">Breakfast included</p>
              </div>
            </div>
            <div class="room-card">
              <div class="image-slider">
                <img src="/src/images/avatar.png" alt="Deluxe Room" />
              </div>
              <div class="room-info">
                <h3>Deluxe Room</h3>
                <div class="info">
                  <div class="info-content">
                    <img
                      src="/src/images/People icon (select details).svg"
                      alt=""
                    />
                    <p>Sleeps 3</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Bed icon.svg" alt="" />
                    <p>1 Single Bed · 1 King Bed</p>
                  </div>
                </div>
                <div class="info">
                  <div class="info-content">
                    <img src="/src/images/Room size icon.svg" alt="" />
                    <p>159 sq ft</p>
                  </div>
                </div>
                <p class="cancellation">
                  <img src="/src/images/Free cancellation icon.svg" alt="" />
                  Free cancellation until <span class="highlight">6th May</span>
                </p>
                <p class="price">PKR 4840 <span>(2 nights)</span></p>
                <p class="note">Breakfast included</p>
              </div>
            </div>
          </div>
        </div>

        <div class="more-details">
          <h2>More details</h2>
          <ul class="more-details-list">
            <li>
              <div class="more-details-item">
                <img
                  src="/src/images/Important Information icon.svg"
                  alt=""
                  width="16"
                />
                <div class="more-detail-text">
                  <p>Important Information</p>
                </div>
                <img
                  src="/src/images/dropdown toggle.svg"
                  alt="Toggle Icon"
                  class="toggle-icon"
                />
              </div>
            </li>
          </ul>
        </div>
        <div class="questions">
          <h2>Questions you may have</h2>
          <ul class="question-list">
            <li>
              <div class="question-list-item">
                <img src="/src/images/Faq icon.svg" alt="" />
                <div class="question-list-text">
                  <h3>Do you offer pickup from hotel?</h3>
                  <p>
                    Yes, you can select the pickup add-on when booking, we will
                    contact you via the travelninja messaging system to confirm
                    details.
                  </p>
                </div>
                <img
                  src="/src/images/toggle up.svg"
                  alt="Toggle Icon"
                  class="toggle-icon"
                />
              </div>
            </li>
            <li>
              <div class="question-list-item">
                <img src="/src/images/Faq icon.svg" alt="" />
                <div class="question-list-text">
                  <h3>What meals will be provided during the tour?</h3>
                </div>
                <img
                  src="/src/images/dropdown toggle.svg"
                  alt="Toggle Icon"
                  class="toggle-icon"
                />
              </div>
            </li>
            <li>
              <div class="question-list-item">
                <img src="/src/images/Faq icon.svg" alt="" />
                <div class="question-list-text">
                  <h3>Which hotels will we stay in?</h3>
                </div>
                <img
                  src="/src/images/dropdown toggle.svg"
                  alt="Toggle Icon"
                  class="toggle-icon"
                />
              </div>
            </li>
            <li>
              <div class="question-list-item">
                <img src="/src/images/Faq icon.svg" alt="" />
                <div class="question-list-text">
                  <h3>Do you help with the supporting documents?</h3>
                </div>
                <img
                  src="/src/images/dropdown toggle.svg"
                  alt="Toggle Icon"
                  class="toggle-icon"
                />
              </div>
            </li>
          </ul>
        </div>
        <div class="review-cont">
          <h2>Reviews</h2>
          <div class="review-summary">
            <div class="review-heading">
              <h2>4.0</h2>
              <div class="review-no">
                <div class="review-stars">
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/boder star.svg" alt="" />
                </div>
                <small>21 Reviews</small>
              </div>
            </div>
            <div class="progress-bar">
              <div class="bar">
                <div class="fill-container">
                  <div class="fill" style="width: 80%"></div>
                </div>
                <span>5.0</span>
                <small>16 Reviews</small>
              </div>
              <div class="bar">
                <div class="fill-container">
                  <div class="fill" style="width: 30%"></div>
                </div>
                <span>4.0</span>
                <small>5 Reviews</small>
              </div>
              <div class="bar">
                <div class="fill-container">
                  <div class="fill" style="width: 0%"></div>
                </div>
                <span>3.0</span>
                <small>0 Reviews</small>
              </div>
              <div class="bar">
                <div class="fill-container">
                  <div class="fill" style="width: 0%"></div>
                </div>
                <span>2.0</span>
                <small>0 Reviews</small>
              </div>
              <div class="bar">
                <div class="fill-container">
                  <div class="fill" style="width: 0%"></div>
                </div>
                <span>1.0</span>
                <small>0 Reviews</small>
              </div>
            </div>
          </div>
          <div class="reviews">
            <div class="review-list">
              <div class="avatar">
                <img src="/src/images/avatar.png" alt="User Avatar" />
              </div>
              <div>
                <div class="review-info">
                  <div class="name">Wamiq Ahmed</div>
                  <div class="date">27 July 2025</div>
                </div>
                <div class="stars">
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                </div>
              </div>
            </div>
            <p>
              Had a great experience with this operator, everything went
              smoothly. From the pickup in Islamabad to the dropoff at the
              airport, they took great care of us. Best value for money.
              Recommended.
            </p>
            <div class="review-media">
              <img src="/src/images/thhunzagalleryimg4.jpg" alt="" />
              <img src="/src/images/hunzagalleryimg1.jpg" alt="" />
              <img src="/src/images/hunzagalleryimg2.jpg" alt="" />
              <img src="/src/images/hunzagalleryimg3.jpg" alt="" />
              <img src="/src/images/hunzagalleryimg5.jpg" alt="" />
              <img src="/src/images/10927.jpg" alt="" />
            </div>
          </div>
          <div class="reviews">
            <div class="review-list">
              <div class="avatar">
                <img src="/src/images/avatar.png" alt="User Avatar" />
              </div>
              <div>
                <div class="review-info">
                  <div class="name">Faisal</div>
                  <div class="date">8 Jun 2025</div>
                </div>
                <div class="stars">
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                </div>
              </div>
            </div>
            <p>Book with them, they're probably the best in Pakistan.</p>
            <div class="reply">
              <span><strong>Eventica Travels</strong> Replied</span>
              <p>
                Thank you so much for the kind words We're thrilled to hear that
                you enjoyed the mix of scenery, culture, and city experiences in
                Vietnam. Ensuring a smooth and safe journey for our travelers is
                our top priority
              </p>
            </div>
          </div>
          <div class="no-border reviews">
            <div class="review-list">
              <div class="avatar">
                <img src="/src/images/avatar.png" alt="User Avatar" />
              </div>
              <div>
                <div class="review-info">
                  <div class="name">Michael</div>
                  <div class="date">24 May 2025</div>
                </div>
                <div class="stars">
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                  <img src="/src/images/Review icon.svg" alt="" />
                </div>
              </div>
            </div>
            <p>
              A well crafted tour... you get to see everything and also alot of
              activities included in the tour. Satisfied witht the trip.
            </p>
          </div>
          <div class="pagination">
            <a class="active" href="#">1</a>
            <a href="#">2</a>
            <a href="#">3</a>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
