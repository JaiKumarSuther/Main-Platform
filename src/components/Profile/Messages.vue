<template>
  <div class="chat-app">
    <!-- Sidebar -->
    <div class="chat-sidebar">
      <h2>Messages</h2>
      <div class="conversation active">
        <div class="conv-header">
          <img
            src="/src/images/Eventica.png"
            alt="Eventica Logo"
            class="conv-avatar"
          />
          <div>
            <div class="conv-name">Eventica Travels</div>
            <div class="conv-preview unread-text">Sounds Great</div>
          </div>
        </div>
      </div>
      <div class="conversation">
        <div class="conv-header">
          <div class="circle-avatar"></div>
          <div>
            <div class="conv-name">Askoli Adventure Tou...</div>
            <div class="conv-preview">Okay great let’s grou...</div>
          </div>
        </div>
      </div>
    </div>

    <!-- Chat Section -->
    <div class="chat-section">
      <div class="chat-header">
        <div class="user-name">
          <img src="/src/images/Eventica.png" alt="" /> Eventica Travels
        </div>
      </div>

      <div class="messages">
        <div class="chat-date">25 Sep 2025</div>
        <div class="message-box">
          <div class="avatar">
            <img src="/src/images/auto-generate.jpg" alt="" />
          </div>
          <div class="message you">
            <p>
              Just booked your hingol national park tour for may 15th. Just
              wanted to confirm everything
            </p>
            <span class="timestamp">19:23</span>
          </div>
        </div>

        <div class="message-box">
          <div class="avatar">
            <img
              src="/src/images//Eventica-Color-Logo_Final-1536x961.png"
              alt=""
            />
          </div>
          <div class="message them">
            <p>
              Yes, i see your booking. Thanks for booking with us. Your spot is
              confirmed, and we’ll see you on may 15th
            </p>
            <span class="timestamp">19:46</span>
          </div>
        </div>

        <div class="message-box">
          <div class="avatar">
            <img src="/src/images/auto-generate.jpg" alt="" />
          </div>
          <div class="message you">
            <p>
              Also, i’ll be landing in karachi a day earlier. Do you offer
              airport pickup?
            </p>
            <span class="timestamp">19:48</span>
          </div>
        </div>

        <div class="message-box">
          <div class="avatar">
            <img
              src="/src/images//Eventica-Color-Logo_Final-1536x961.png"
              alt=""
            />
          </div>
          <div class="message them">
            <p>Yes we do!</p>
            <span class="timestamp">19:53</span>
          </div>
        </div>

        <div class="message-box">
          <div class="avatar">
            <img src="/src/images/auto-generate.jpg" alt="" />
          </div>
          <div class="media-message">
            <div class="media">
              <div class="image-media">
                <span>Image.jpeg</span>
                <img
                  class="download-icon"
                  src="/src/images/download icon.svg"
                  alt=""
                />
              </div>
              <div class="document-file">
                <span>Document.xls</span>
                <img
                  class="download-icon"
                  src="/src/images/download icon.svg"
                  alt=""
                />
              </div>
            </div>
            <div class="message them">
              <p>you can check out these files</p>
              <span class="timestamp">19:53</span>
            </div>
          </div>
        </div>

        <div class="message-box">
          <div class="avatar">
            <img src="/src/images/auto-generate.jpg" alt="" />
          </div>
          <div class="media-message">
            <div class="media">
              <div class="image-media">
                <span>Image.jpeg</span>
                <img
                  class="download-icon"
                  src="/src/images/download icon.svg"
                  alt=""
                />
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Message Input -->
      <div class="chat-input">
        <input type="text" placeholder="Send a message..." />
        <img class="attach-media" src="/src/images/attach-media.svg" alt="" />
        <button class="send-btn">
          <img src="/src/images/send-hor-svgrepo-com.svg" alt="" />
        </button>
      </div>
    </div>
  </div>
</template>
